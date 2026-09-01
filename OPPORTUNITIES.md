# Dataset Opportunities

This is a practical map of chemistry datasets that can be assembled now and of important data that remains hard to obtain. “Easy” here means that the sources offer bulk downloads or documented APIs, expose usable identifiers, and have terms that permit research reuse. It does **not** mean that records can be concatenated without chemical standardization, provenance tracking, or a license review.

## Best combinations to build now

| Priority | Dataset product | Sources to combine | Primary join keys | Why it is tractable | Main caveat |
| --- | --- | --- | --- | --- | --- |
| 1 | Chemical identity and synonym graph | [PubChem](https://pubchem.ncbi.nlm.nih.gov/docs/downloads), [ChEBI](https://www.ebi.ac.uk/chebi/downloads), and source cross-references | full InChIKey, standardized InChI, source accession | Bulk files already contain structures, synonyms, and cross-references | Salts, mixtures, tautomers, stereochemistry, and source-specific licenses must remain explicit |
| 2 | Unified small-molecule bioactivity table | [ChEMBL](https://www.ebi.ac.uk/chembl/), [BindingDB](https://www.bindingdb.org/rwd/bind/chemsearch/marvin/Download.jsp), [PubChem BioAssay](https://pubchem.ncbi.nlm.nih.gov/docs/bioassays), and [Guide to PHARMACOLOGY](https://www.guidetopharmacology.org/) | standardized compound + UniProt/target accession + assay provenance | All provide machine-readable activity data and external identifiers | Assay endpoints are not interchangeable; censoring, units, target constructs, and duplicated literature records require careful handling |
| 3 | Condition-aware solubility and solvation data | [AqSolDB](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/OVHAW8), [BigSolDB 2.0](https://zenodo.org/records/15094979), [FreeSolv](https://github.com/MobleyLab/FreeSolv), [ThermoML](https://www.nist.gov/mml/acmd/trc/thermoml/thermoml-archive), and [ILThermo](https://ilthermo.boulder.nist.gov/) | solute structure + solvent/components + temperature + pressure + property definition | The sources are downloadable and complementary across aqueous, organic-solvent, mixture, and free-energy regimes | Never merge values without retaining temperature, pH, solid form, method, units, uncertainty, and original citation |
| 4 | Structure-linked protein–ligand benchmark | [RCSB PDB](https://www.rcsb.org/docs/programmatic-access/file-download-services), ChEMBL, BindingDB, and [Open Targets](https://platform.opentargets.org/) | PDB chemical component, InChIKey, UniProt accession, publication DOI | PDB files and APIs are CC0 and bioactivity sources carry cross-references | A deposited ligand is not automatically the measured ligand; construct, mutation, binding-site, and assay context matter |
| 5 | Structure–spectrum corpus | [MassBank](https://massbank.eu/MassBank/), [GNPS](https://ccms-ucsd.github.io/GNPSDocumentation/api/), [MoNA](https://mona.fiehnlab.ucdavis.edu/), and [nmrshiftdb2](https://nmrshiftdb.nmr.uni-koeln.de/) enriched with PubChem identifiers | full InChIKey + ion/adduct + instrument and collision metadata | Records are already machine-readable and often include structure identifiers | Predicted and experimental spectra, stereoisomers, adducts, collision energies, and licenses must not be collapsed |
| 6 | Literature-grounded chemical knowledge graph | [Europe PMC](https://europepmc.org/downloads), [PubTator 3](https://www.ncbi.nlm.nih.gov/research/pubtator3/api), ChEBI, PubChem, and domain datasets | PMID/PMCID/DOI + normalized entity IDs + source accession | Full text, annotations, relations, and entity registries are accessible in bulk | Text-mined relations are hypotheses, not curated facts; keep passage-level evidence and model/version metadata |
| 7 | Reaction conditions and outcomes benchmark | [Open Reaction Database](https://docs.open-reaction-database.org/en/stable/overview.html), [USPTO](https://figshare.com/articles/dataset/Chemical_reactions_from_US_patents_1976-Sep2016_/5104873), Dreher–Doyle, and Perera | atom-mapped reaction + reactant/product structures + source record | ORD supplies a rich target schema and the other sources provide scale or dense condition screens | Patent extraction is noisy and success-biased; atom mappings, yields, roles, and duplicate reactions need independent validation |
| 8 | Computed–experimental materials bridge | [Materials Project](https://docs.materialsproject.org/downloading-data/using-the-api), [NOMAD](https://nomad-lab.eu/nomad-lab/), and [Crystallography Open Database](https://www.crystallography.net/cod/) | normalized structure match + composition + space group + provenance | All expose structures and machine-readable access routes | Formula matching alone is unsafe; polymorphs, disorder, calculation settings, and database terms require record-level treatment |

The first two products are the strongest foundations because they create reusable identity layers. The solubility and spectra products are relatively bounded projects with clear scientific payoffs. The reaction and materials products are valuable but need substantially more domain-specific normalization.

## A minimal integration contract

A combined release should use a small number of stable tables rather than one extremely wide CSV:

- `entities`: canonical internal ID, original structure, standardized structure, full InChIKey, formula, charge, stereochemistry status, and source accessions.
- `measurements`: entity or relationship ID, property, value, unit, uncertainty/censoring, method, and all relevant experimental conditions.
- `relationships`: typed subject–predicate–object assertions such as compound–target activity or structure–organism occurrence.
- `evidence`: source record, DOI/PMID, quoted location or assay record, extraction method, curator/model version, and confidence.
- `licenses`: license and terms URL for every source and, where necessary, every row.
- `release_manifest`: source versions, retrieval timestamps, checksums, transformations, rejected-record counts, and code commit.

Practical rules:

1. Keep immutable raw snapshots and make every transformation reproducible.
2. Preserve the submitted structure as well as the standardized structure. Record each standardization decision.
3. Treat exact stereochemical identity, connectivity-only identity, parent structure, and tautomer family as different join layers.
4. Normalize units, but never discard original values, units, qualifiers (`<`, `>`, ranges), conditions, or significant figures.
5. Do not average conflicting measurements by default. Conflicts are useful data when provenance and method are retained.
6. Deduplicate source records separately from deduplicating scientific observations; the same paper can be imported by several databases.
7. Publish source-aware, time-aware, and scaffold/structure-aware splits alongside random splits to expose leakage.
8. Apply the most restrictive compatible redistribution terms to derived bundles and retain per-source attribution.

## High-value data that remains untapped

| Gap | Why it matters | What blocks collection | A realistic first project |
| --- | --- | --- | --- |
| Failed and negative experiments | Calibrates feasibility and reduces publication/success bias | Mostly trapped in ELNs, notebooks, and unreported screening wells | Release one institution’s de-identified failed reactions or inactive wells in the ORD schema, including the decision threshold |
| Complete synthesis procedures | Enables condition prediction, scale-up reasoning, and reproducibility | Conditions, addition order, workup, purification, and analytical evidence are scattered through supporting information | Extract one permissively licensed journal or repository collection into ORD with passage-level provenance and human QA |
| Formulations and mixtures | Industrial chemistry depends on multicomponent systems rather than isolated molecules | No universal identifier for composition, processing history, or morphology; much data is proprietary | Define a mixture/formulation schema and curate one narrow domain such as battery electrolytes or coatings |
| Raw instrument data with QC | Supports reprocessing, uncertainty estimation, and foundation models | File formats, calibration metadata, storage volume, and sample identity are inconsistent | Pair open raw LC–MS/NMR files with reference structures, blanks, calibrants, and processing parameters |
| Replicates, uncertainty, and inter-lab variation | Separates measurement noise from chemical signal | Published tables often report only aggregate values and omit failed replicates | Collect repeated measurements for one property with method, lab, instrument, and uncertainty metadata |
| Polymer and macromolecular identity | Polymers, resins, and formulations dominate real materials use | Small-molecule identifiers do not encode distributions, topology, sequence, or processing history | Build a BigSMILES/HELM-centered crosswalk with monomers, architecture, dispersity, and measured properties |
| Synthesis–structure–property links for materials | Bridges predicted crystals to experimentally realizable materials | Structure matching, polymorphism, disorder, synthesis provenance, and sample history are difficult | Link a narrow family such as perovskites across COD, NOMAD, Materials Project, and open synthesis literature |
| Process, safety, cost, and sustainability data | Needed to rank viable chemistry, not merely possible chemistry | Supply chains and process measurements are proprietary, regional, and time-dependent | Combine public hazard classifications, measured properties, commodity prices, and process mass-intensity data with dated provenance |
| Temporal and causal chemical knowledge | Most databases flatten changing evidence into timeless facts | Database releases overwrite records and literature relations are often correlational | Maintain versioned assertions with valid-time, transaction-time, evidence type, and retraction/correction status |

## What not to combine blindly

- **Identifiers:** the first block of an InChIKey ignores stereochemistry and isotopes; it is useful for grouping, not exact identity.
- **Assays:** `IC50`, `EC50`, `Ki`, percent inhibition, and qualitative labels are different targets.
- **Solubility:** molar and mass solubility, intrinsic and apparent solubility, kinetic and thermodynamic measurements, and different solid forms are not interchangeable.
- **Spectra:** ion mode, adduct, collision energy, instrument type, derivatization, and predicted/experimental status define the observation.
- **Reactions:** a reaction SMILES commonly omits addition order, concentration, atmosphere, workup, purification, and failure criteria.
- **Materials:** identical formulae can describe different phases, polymorphs, defects, surfaces, and processing histories.
- **Licenses:** an accessible webpage or API is not evidence that a compiled dataset can be redistributed.

## Suggested repository next steps

1. Add a machine-readable catalog (`datasets.yaml`) with name, domain, landing page, access method, license, identifiers, update cadence, and last-verified date.
2. Generate the README lists from that catalog so metadata stays consistent and duplicates can be detected automatically.
3. Add a scheduled link-and-metadata audit that opens focused issues rather than silently dropping sources.
4. Implement one reference pipeline—the chemical identity graph is the best starting point—with a small checked-in sample, schema tests, and a versioned release manifest.
5. Track untapped areas as issues labeled `dataset-opportunity`, each with scope, candidate sources, licensing questions, and an acceptance test.
