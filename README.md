# Awesome Chemistry Datasets [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of chemistry datasets that are available for research, machine learning, and data integration. The list includes raw data sources, curated collections, and benchmarks; availability does not imply that every source permits unrestricted redistribution or commercial use.

**Looking to build rather than browse?** See [Dataset opportunities](OPPORTUNITIES.md) for combinations that are practical now, common integration traps, and high-value areas that remain largely untapped.

Contributions are very welcome—please follow the [guidelines](CONTRIBUTING.md) and the [Code of Conduct](code_of_conduct.md).

## Contents

- [Text and literature](#text-and-literature)
- [Chemical structures and spectra](#chemical-structures-and-spectra)
- [Molecular activity and benchmarks](#molecular-activity-and-benchmarks)
- [Molecular properties and benchmarks](#molecular-properties-and-benchmarks)
- [Target identification](#target-identification)
- [Pharmacology, ADME, and metabolism](#pharmacology-adme-and-metabolism)
- [Glycoscience](#glycoscience)
- [Reactions and high-throughput screening](#reactions-and-high-throughput-screening)
- [Electronic laboratory notebooks](#electronic-laboratory-notebooks)
- [Materials and solid state](#materials-and-solid-state)
- [Related lists](#related-lists)

## Text and literature

- [BC5CDR](https://paperswithcode.com/dataset/bc5cdr): 1,500 PubMed articles with 4,409 annotated chemicals, 5,818 diseases, and 3,116 chemical–disease interactions for named-entity recognition.
- [BioCreative V](https://biocreative.bioinformatics.udel.edu/tasks/biocreative-v/track-3-cdr/): BC5CDR corpus consists of 1500 PubMed articles with 4409 annotated chemicals, 5818 diseases and 3116 chemical-disease interactions.
- [BioRxiv XML](https://www.biorxiv.org/tdm) - Bulk access to the full text of bioRxiv articles for the purposes of text and data mining (TDM) is available via a dedicated Amazon S3 resource.
- [ChemTables](https://doi.org/10.17632/g7tjh7tbrj.3): 788 chemical patent tables with labels of their content type. [Built for semantic classification of table type](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00568-2#Abs1). Licensed under CC BY NC 3.0.
- [Elsevier Corpus](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/3): 40,001 open-access, CC BY articles from across Elsevier journals for large-scale NLP and ML research.
- [Europe PMC](https://europepmc.org/downloads) - Bulk download of full text and SI of > 5 million articles.
- [IUPAC Gold Book](https://goldbook.iupac.org/)
- [LibreText](https://chem.libretexts.org/): Open-access chemistry textbook.
- [MedRxiv XML](https://www.medrxiv.org/tdm) - Text and data mining is possible via dedicated Amazon S3 resource.
- [NLM Literature Archive](https://ftp.ncbi.nlm.nih.gov/pub/litarch/): books, documents, and articles in life science, medicine, and healthcare; also accessible through [NCBI Bookshelf](https://www.ncbi.nlm.nih.gov/books/). See [NLMChem](https://ftp.ncbi.nlm.nih.gov/pub/lu/NLMChem/) for 150 full-text articles with manually annotated chemical mentions.
- [OpenStax](https://openstax.org/) Free textbooks, including [Chemistry 2e](https://openstax.org/details/books/chemistry-2e), which is released under CC-BY 4.0.
- [PubChemSTM](https://arxiv.org/abs/2212.10789): 281K chemical structure and text pairs
- [PubMed central](https://www.ncbi.nlm.nih.gov/pmc/): free full-text archive
- [PubMed](https://pubmed.ncbi.nlm.nih.gov/): abstracts and outlinks
- [PubMedQA](https://pubmedqa.github.io/): answer research questions with yes/no/maybe using abstracts (1k expert labeled, 61.2k unlabeled and 211.3k artificially generated QA instances).
- [PubTator 3](https://www.ncbi.nlm.nih.gov/research/pubtator3/): PubMed and PMC text annotated with normalized chemicals, genes, diseases, variants, species, cell lines, and relations; available by API and bulk FTP download.
- [S2ORC](https://github.com/allenai/s2orc): Semantic Scholar Open Research Corpus of 81.1 million English-language academic papers across many disciplines. Released under CC BY-NC 4.0.

## Chemical structures and spectra

- [ChEBI](https://www.ebi.ac.uk/chebi/downloads): curated chemical entities, ontology terms, synonyms, structures, and cross-references; bulk SDF and database dumps are available under CC BY 4.0.
- [COCONUT](https://coconut.naturalproducts.net/): is an open source project for Natural Products (NPs) storage, search and analysis.
- [Crystallography Open Database](http://www.crystallography.net/cod/): open-access collection of crystal structures of organic, inorganic, metal-organic compounds and minerals, excluding biopolymers. [They also derived SMILES for some compounds.](https://doi.org/10.1186/s13321-018-0279-6)
- [Enamine HTS collection](https://enamine.net/compound-collections/screening-collection/hts-collection):  1 930 980 diverse screening compounds (37 billion molecules in 2D and 4.5 billion in 3D)
- [GDB](https://gdb.unibe.ch/downloads/): enumeration of molecules according to simple (feasibility and stability) rules
- [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp): mass spectrometry database with focus on natural products, contains untargeted (unlabelled) data.
- [MassBank](https://massbank.eu/MassBank/): open repository of reference mass spectra with machine-readable records and structure identifiers.
- [MoNA](https://mona.fiehnlab.ucdavis.edu/): mass spectrometry database of real and predicted spectra for known compounds.
- [nCov-Group Data Repository](https://2019-ncovgroup.github.io/data/#dataset-downloads): SMILES, fingerprints, descriptors, and images of millions of compounds.
- [nmrshiftdb2](https://nmrshiftdb.nmr.uni-koeln.de/): is database for organic structures and their nuclear magnetic resonance (NMR) spectra. 
- [PubChem](https://pubchem.ncbi.nlm.nih.gov/docs/downloads): chemical structures, identifiers, properties, substances, assays, and cross-references available through APIs and bulk FTP downloads; licensing can vary with the original depositor.
- [RCSB PDB](https://www.rcsb.org): experimentally determined 3D structures of proteins, nucleic acids, and complexes, released under CC0.
- [zinc20](https://files.docking.org/zinc20-ML/): ZINC20 library prepared for Deep Docking-accelerated virtual screening
- [zinc22](https://cartblanche22.docking.org/): commercially-available compounds for virtual screening

## Molecular activity and benchmarks

- [Bento](https://github.com/LigandPro/Bento): a protein-ligand docking benchmark covering rigid, flexible, de novo, blind, induced-fit, and covalent docking tasks.
- [ChEMBL](https://www.ebi.ac.uk/chembl/): manually curated compounds, targets, assays, and bioactivity measurements, with web services and full database downloads under CC BY-SA 3.0.
- [MPCD](https://github.com/bidd-group/MPCD/tree/main): molecular activity prediction benchmark with 9 low-sample, narrow-scaffold inhibitor datasets and 30 higher-sample, mixed-scaffold inhibitor datasets, each visualized with [TMAP](https://bidd-group.github.io/MPCD/dataset/HSSMS/MoleculeACE_benchmark/space/info/CHEMBL4792_Ki.html).
- [MoleculeACE](https://github.com/molML/MoleculeACE): a benchmark (30 HSSMS datasets in MPCD) for evaluating the predictive performance on activity cliff compounds of machine learning models.
- [PubChem BioAssay](https://pubchem.ncbi.nlm.nih.gov/docs/bioassays): deposited screening and assay records linked to PubChem substances and compounds; available through PUG REST and bulk downloads.

## Molecular properties and benchmarks

- [ACNet](https://drugai.github.io/ACNet/): a benchmark for Activity Cliff Prediction, 400K Matched Molecular Pairs (MMPs) against 190 targets, including over 20K MMP-cliffs and 380K non-AC MMPs from ChEMBL (version 28).
- [Aquasoldb](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/OVHAW8): Curation of nine open source datasets on aqueous solubility. The authors also assigned reliability groups.
- [BigSolDB 2.0](https://zenodo.org/records/15094979): Molecular solubility in organic solvents and water in a wide range of temperatures. It contains 103944 experimentally measured solubility values of 1448 organic compounds in 213 solvents reported in the 1595 literature peer-reviewed articles. Initially [BigSolDB](https://zenodo.org/record/6984601), posted in [this preprint](https://chemrxiv.org/engage/chemrxiv/article-details/6426c1d8db1a20696e4c947b). Recently (2025), updated to [BigSolDB 2.0](https://zenodo.org/records/15094979), published in [Scientific Data](https://doi.org/10.1038/s41597-025-05559-8).
- [BindingDB](https://www.bindingdb.org/rwd/bind/chemsearch/marvin/Download.jsp): molecular recognition database, contains 2.6M data for 1.1M Compounds and 8.10K Targets (Feb 2023)
- [BOOM](https://github.com/FLASK-LLNL/BOOM): **B**enchmarks for **O**ut-**o**f-distribution **M**olecules is an out-of-distribution benchmark for molecular property prediction based on QM9 and LLNL-10k properties.
- [ChEBI-20](https://paperswithcode.com/dataset/chebi-20): 33,010 molecule-description pairs (for molecule captioning task)
- [ESol](https://pubmed.ncbi.nlm.nih.gov/15154768/): aqueous solubility data (log mol/L) for common organic small molecules.
- [Flashpoint](https://github.com/cheminfo/molecule-features/blob/main/data/flashpoint/meta.yaml#:~:text=https%3A//figshare.com/articles/dataset/Data_for_Assessing_Graph%2Dbased_Deep_Learning_Models_for_Predicting_Flash_Point/9275210): Sun et al. collected a dataset of the flashpoints of 10575 molecules from academic papers, the Gelest chemical catalogue, the DIPPR database, Lange's Handbook of Chemistry, the Hazardous Chemicals Handbook, and the PubChem database.
- [FreeSolv](https://github.com/MobleyLab/FreeSolv): Experimental and Calculated Small Molecule Hydration Free Energies
- [Harvard OPV](https://figshare.com/articles/dataset/HOPV15_Dataset/1610063/4): "experimental photovoltaic data from the literature, and corresponding quantum-chemical calculations performed over a range of geometries, each with quantum chemical results using a variety of density functionals and basis sets"
- [Hydrogen Storage Materials Database](https://datahub.hymarc.org/dataset/hydrogen-storage-materials-db): data on hydrogen storage materials (information such as chemical formula and hydrogen capacity)
- [ILThermo](https://ilthermo.boulder.nist.gov/): thermodynamic and transport properties of pure ionic liquids and mixtures of them.
- [Leffingwell Odor Dataset](https://zenodo.org/record/4085098): 3523 molecules associated with expert-labeled odor descriptors from the Leffingwell PMP 2001 database
- [Limiting activity coefficients](https://polybox.ethz.ch/index.php/s/kyVOt3pwHW26PP4): for different solvent/solute pairs, used to train a SMILES-based transformer.
- [Lipophilicty](https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/Lipophilicity.csv): Experimental results of octanol/water distribution coefficient(logD at pH 7.4).
- [LLNL-10k-Dataset](https://github.com/FLASK-LLNL/LLNL-10k-Dataset): DFT-calculated density and solid heat-of-formation values for approximately 10,000 CHNO molecules.
- [MD simulated monomer properties](https://acdc.alcf.anl.gov/mdf/detail/elwood_md_v1.2/): density, cohesive energy, thermal expansion, heat of vaporization, compressibility, radius of gyration, glass transition, and diffusion constant for 410 monomers
- [MoleculeNet](https://moleculenet.org/datasets-1): benchmark suite containing multiple datasets listed here.
- [oechem](https://ochem.eu/): On Feb 17 2023 OCHEM contained 3774118 records for 689 properties (with at least 50 records) collected from 20609 sources (user is granted a Creative Commons CC-BY (version 4.0) license to data submitted)
- [Papyrus](https://doi.org/10.4121/16896406.v3): large-scale curated bioactivity dataset combining ChEMBL, ExCAPE-DB, and smaller public datasets.
- [minKLIFSAI](https://zenodo.org/records/13370507): 18.8 million activity records for 452 kinases and approximately 1.2 million unique compounds (300,000 active and 900,000 inactive), collected from PubChem in January 2023.
- [Photoswitch Dataset](https://github.com/Ryan-Rhys/The-Photoswitch-Dataset): Curated dataset of 405 photoswitch molecules.
- [QM Datasets](http://quantum-machine.org/datasets/): QM7, QM7b, QM8, QM9, MD Trajectories
- [SolProp](https://discord.com/channels/850068776544108564/1074753729955381298/1076099689184772116): Database of 1 million solvent/solute COSMO-RS calculations and 10145 experimental solvation free energies (originally published as part of [this paper](https://arxiv.org/abs/2012.11730)).
- [SOMAS](https://doi.org/10.6084/m9.figshare.14552697):  Experimental and calculated solubilities for small molecules. Originally proposed for the design of redox-flow batteries.
- [Therapeutic Data Commons](https://tdcommons.ai/overview/): ML tasks that cover small molecules and biologics, including antibodies, peptides, miRNAs, and gene editing therapies. Original data can be found [here](https://doi.org/10.7910/DVN/21LKWG).
- [ThermoML Archive](https://www.nist.gov/mml/acmd/trc/thermoml/thermoml-archive): experimental thermophysical and thermochemical property data (in ThermoML XML format)
- [LIT-PCBA](https://drugdesign.unistra.fr/LIT-PCBA/): virtual-screening benchmark with 15 target sets, 7,761 actives, and 382,674 unique inactives selected from high-confidence PubChem BioAssay data.


## Target identification

- [Open Targets](https://platform.opentargets.org/): is a large-scale resource that uses human genetics and genomics data for systematic drug target identification and prioritization.
- [Probes & Drugs Portal](https://www.probes-drugs.org/data_sources): is an interactive, open data resource for chemical biology. Overview of libraries of bioactive compounds (e.g., ChEMBL, Guide to PHARMACOLOGY), including commercial screening libraries.

## Pharmacology, ADME, and metabolism

- [SIDER](http://sideeffects.embl.de/download/): drugs, adverse reactions, and indications extracted from public documents and package inserts. Released under CC BY-NC-SA 4.0.
- [Cell Effective Permeability (Caco-2) dataset](https://figshare.com/collections/ADME_Properties_Evaluation_in_Drug_Discovery_Prediction_of_Caco_2_Cell_Permeability_Using_a_Combination_of_NSGA_II_and_Boosting/2867641): by Wang et al. is a dataset used to measure the absorption of drugs through intestinal tissue by simulating it using a human colon epithelial cancer cell line (Caco-2).
- [Clinical Trials](https://clinicaltrials.gov/ct2/resources/download): single zip file containing all study records (in XML) available on ClinicalTrials.gov
- [Drug–Drug–Interaction (DDI)](https://paperswithcode.com/dataset/ddi): MedLine abstracts on drug-drug interactions as well as documents describing drug-drug interactions from the DrugBank database.
- [Drug Indications Database (DID)](https://figshare.com/articles/dataset/Additional_file_1_of_Toward_a_comprehensive_drug_ontology_extraction_of_drug-indication_relations_from_diverse_information_sources/4535021): is a dataset of structured drug-indication relations. It is intended to facilitate the building of practical, comprehensive, integrated drug ontologies.
- [EPA CompTox](https://comptox.epa.gov/dashboard): is a widely used resource for chemistry, toxicity, and exposure information for hundreds of thousands of chemicals including, but not limited to, chemical properties, environmental fate, and transport, hazard, in vitro to in vivo extrapolation (IVIVE), exposure, bioactivity (each data has its license).
- [Guide to PHARMACOLOGY](https://www.guidetopharmacology.org/): is an expert-curated resource of ligand-activity-target relationships. It includes activity data even for data with unknown bioactivity value (under CC BY-SA 4.0).
- [KD-DTI](https://github.com/microsoft/BioGPT): Drug-target-interaction triplets (12K training samples, 1K validation samples and 1.1K test samples). See [paper](https://academic.oup.com/bioinformatics/article/38/22/5100/6751771?rss=1#382115390).
- [KEGG PATHWAY Database(KEGG)](https://www.genome.jp/kegg/kegg2.html): a database resource for understanding high-level functions and utilities of the biological system, such as the cell, the organism and the ecosystem, from molecular-level information, especially large-scale molecular datasets generated by genome sequencing and other high-throughput experimental technologies.
- [LOTUS](https://zenodo.org/communities/the-lotus-initiative): harmonization, curation, validation and open dissemination of 750,000+ referenced structure-organism pairs (relationships between molecular structures and the living organisms from which they were identified).
- [MetXBioDB Metabolite Biotransformations](https://zenodo.org/record/4247792#.Y_uK3NJBypN): a comprehensive collection of biotransformation reactions and metabolite information from the BioTransformer database. It includes the transformation and metabolism of metabolites.
- [ONSIDES](https://github.com/tatonetti-lab/onsides): A resource of adverse drug effects extracted from FDA structured product labels.
- [PAMPA Permeability and NCATS dataset](https://doi.org/10.1177/24725552211017520): is a dataset of commonly employed assay to evaluate drug permeability across the cellular membrane to help in ADME prediction.
- [PsychonautWiki](https://psychonautwiki.org/wiki/Psychoactive_substance_index): catalog of mind-altering substances
- [QSAR datasets - Meta-QSAR (phase I & II)](https://data.mendeley.com/datasets/spwgrcnjdg/1): Data (extracted from ChEMBL) used in Olier et al. Meta-QSAR: a large-scale application of meta-learning to drug design and discovery.
- [State of Peptides 2026](https://peptahub.com/state-of-peptides-2026): open reference dataset of 156 peptide and peptide-adjacent compounds with legal/regulatory status buckets, categories, routes of administration, half-life, molecular weight, CAS numbers, peer-reviewed reference counts, and external knowledge-graph identifiers (PubChem/DrugBank/Wikidata). Downloadable as CSV and JSON under CC BY 4.0.
- [The Human Metabolome Database (HMDB)](https://hmdb.ca/): is a freely available electronic database containing detailed information about small molecule metabolites found in the human body.
- [The Metabolism and Transport Database ](https://www-metrabase.ch.cam.ac.uk/metrabaseui/pageview/download/): is a cheminformatics and bioinformatics resource that contains curated data related to human small molecule metabolism and transport.

## Glycoscience

### Data and registries

- [Glycan Library](https://glycosciences.med.ic.ac.uk/data.html): a list of approximately 830 lipid-linked sequence-defined glycan probes derived from diverse natural sources or chemically synthesised 
- [GlyGen](https://data.glygen.org/): GlyGen is a data integration and dissemination project for carbohydrate and glycoconjugate related data. GlyGen retrieves information from multiple international data sources and integrates and harmonizes this data. The GlyGen web portal allows exploration of this data and execution of unique searches that cannot be performed using integrated databases in isolation. GlyGen also provides machine-readable APIs and a SPARQL endpoint to access the integrated data. Released under CC-BY-4.0 licence.
- [SugarBind](https://sugarbind.expasy.org/query): SugarBind covers knowledge of glycan binding of human pathogen lectins and adhesins. Information is collected by experts from articles published in peer-reviewed scientific journals. The data were compiled through an exhaustive search of literature published over the past 30 years by glycobiologists, microbiologists, and medical histologists.
- [UniCarb-DB](http://www.unicarb-db.org/): glycomics fragmentation database that stores, integrates, and processes manually annotated mass spectra.
- [GlyCosmos](https://glycosmos.org/download): is glycoscience data based on Semantic Web technology. Glycan-related data including genes, proteins, lipids, pathways, diseases and organisms. Released under CC-BY-4.0 license.
- [GlyTouCan](https://glytoucan.org/): international glycan structure registry assigning stable accessions at resolutions from monosaccharide composition to fully defined structures. Released under CC0.
- [GlycoNAVI](https://glyconavi.org/): is the Carbohydrate database to support carbohydrate research. Contains glycan structures, chemical synthesis, anomeric isomer proportion, NMR spectra, activity, 3D structures, and carbohydrate-protein interaction extracted from literature. Released under CC-BY licence.

### Reference resources and tools

- [CAZypedia](https://www.cazypedia.org/): community-driven encyclopedia of carbohydrate-active enzymes.
- [ENZYME](https://enzyme.expasy.org/): repository of enzyme nomenclature information.
- [ExplorEnz](https://www.enzyme-database.org/): interface to the approved IUBMB enzyme nomenclature and classification list.
- [GLIC](https://glic.glycoinfo.org/): centralized software repository for glycoscientists.
- [Glycopedia](https://www.glycopedia.eu/): educational resource and tools for glycoscience.
- [IntEnz](http://www.enzyme-database.org/): integrated relational database of IUBMB enzyme nomenclature recommendations.
- [SNFG](https://www.ncbi.nlm.nih.gov/glycans/snfg.html): Symbol Nomenclature for Glycans standard and drawing resources. Released under CC0.

## Reactions and high-throughput screening

- [USPTO](https://figshare.com/articles/dataset/Chemical_reactions_from_US_patents_1976-Sep2016_/5104873): Reactions extracted by text-mining from United States patents published between 1976 and September 2016.
- [RDB7](https://zenodo.org/record/6618262): Computational dataset with atom-mapped SMILES, barrier heights, and reaction enthalpies calculated at CCSD(T)-F12, which is known to be very accurate. Geometries are identified via the growing string method in this [paper](https://www.nature.com/articles/s41597-020-0460-4) while the high-quality energies are computed in this [paper](https://www.nature.com/articles/s41597-022-01529-6).
- [Dreher-Doyle](https://github.com/leojklarner/gauche/blob/main/data/reactions/dreher_doyle_science_aar5169.csv): yields and conditions for 3955 Pd-catalysed Buchwald–Hartwig C–N crosscouplings
- [Open Reaction Database](https://docs.open-reaction-database.org/en/stable/overview.html): openly licensed reaction records with a detailed schema for inputs, conditions, observations, workups, outcomes, and provenance.
- [Perera](https://github.com/leojklarner/gauche/blob/main/data/reactions/suzuki_miyaura_data.csv): yields and conditions for 5760 Pd-catalysed Suzuki-Miyaura C-C cross-couplings

## Electronic laboratory notebooks

- [AstraZeneca ELN](https://chemrxiv.org/engage/chemrxiv/article-details/6150143118be8575b030ad43)

## Materials and solid state

- [Materials Project](https://docs.materialsproject.org/downloading-data/how-do-i-download-the-materials-project-database): computed inorganic materials and molecular properties, structures, provenance, and contributed experimental data available through an API and open-data snapshots; an API key is required for the main API.
- [NOMAD](https://nomad-lab.eu/nomad-lab/): FAIR repository and archive for raw and normalized computational materials-science data with APIs and metadata-based search. Published data are available under CC BY 4.0.

## Related lists

- [porous materials AI gym](https://github.com/SimonEnsemble/porous-material-AI-gym): open data sets for machine learning pertaining to porous materials.
- [awesome materials informatics](https://github.com/tilde-lab/awesome-materials-informatics/edit/master/README.md): overview of software, data and initatives in the field of materials informatics 




## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
