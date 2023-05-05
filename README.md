# awesome-chemistry-datasets [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)


Contributions are very welcome - please follow the [guidelines](CONTRIBUTING.md) and the [Code of Conduct](code_of_conduct.md).


## text datasets

- [BC5CDR](https://paperswithcode.com/dataset/bc5cdr):1500 PubMed articles with 4409 annotated chemicals, 5818 diseases and 3116 chemical-disease interactions (named entity recognition)
- [BioCreative V](https://biocreative.bioinformatics.udel.edu/tasks/biocreative-v/track-3-cdr/): BC5CDR corpus consists of 1500 PubMed articles with 4409 annotated chemicals, 5818 diseases and 3116 chemical-disease interactions.
- [BioRxiv XML](https://www.biorxiv.org/tdm) - Bulk access to the full text of bioRxiv articles for the purposes of text and data mining (TDM) is available via a dedicated Amazon S3 resource.
- [ChemTables](https://doi.org/10.17632/g7tjh7tbrj.3): 788 chemical patent tables with labels of their content type. [Built for semantic classification of table type](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-021-00568-2#Abs1). Licensed under CC BY NC 3.0.
- [Elsevier Corpus](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/3): This is a corpus of 40k (40,001) open access (OA) CC-BY articles from across Elsevier’s journals represent the first cross-discipline research of data at this scale to support NLP and ML research.
- [Europe PMC](https://europepmc.org/downloads) - Bulk download of full text and SI of > 5 million articles.
- [IUPAC Gold Book](https://goldbook.iupac.org/)
- [LibreText](https://chem.libretexts.org/): Open-access chemistry textbook.
- [MedRxiv XML](https://www.medrxiv.org/tdm) - Text and data mining is possible via dedicated Amazon S3 resource.
- [NLM literature archive](https://ftp.ncbi.nlm.nih.gov/pub/litarch/): NLM LitArch (NLM Literature Archive) is a digital archive for books, documents, and articles in the fields of life science, medicine, and healthcare at the National Institutes of Health. Also accessible via [NCBI bookshelf](https://www.ncbi.nlm.nih.gov/books/). See also the [NLMChem](https://ftp.ncbi.nlm.nih.gov/pub/lu/NLMChem/), a manually annotated full-text resource on chemicals in the biomedical literature. It contains 150 full-text journal articles selected both to be rich in chemical mentions and for articles where human annotation was expected to be most valuable. However, I saw NLM literature archive already on the list but wasn't sure if it included this dataset
- [OpenStax](https://openstax.org/) Free textbooks, including [Chemistry 2e](https://openstax.org/details/books/chemistry-2e), which is released under CC-BY 4.0.
- [PubChemSTM](https://arxiv.org/abs/2212.10789): 281K chemical structure and text pairs
- [PubMed central](https://www.ncbi.nlm.nih.gov/pmc/): free full-text archive
- [PubMed](https://pubmed.ncbi.nlm.nih.gov/): abstracts and outlinks
- [PubMedQA](https://pubmedqa.github.io/): answer research questions with yes/no/maybe using abstracts (1k expert labeled, 61.2k unlabeled and 211.3k artificially generated QA instances).
- [S2ORC](https://github.com/allenai/s2orc): The Semantic Scholar Open Research Corpus.  81.1M English-language academic papers spanning many academic disciplines  largest publicly-available collection of machine-readable academic text). Released under CC BY-NC 4.0.

## structures 

- [COCONUT](https://coconut.naturalproducts.net/): is an open source project for Natural Products (NPs) storage, search and analysis.
- [Crystallography Open Database](http://www.crystallography.net/cod/): open-access collection of crystal structures of organic, inorganic, metal-organic compounds and minerals, excluding biopolymers. [They also derived SMILES for some compounds.](https://doi.org/10.1186/s13321-018-0279-6)
- [Enamine HTS collection](https://enamine.net/compound-collections/screening-collection/hts-collection):  1 930 980 diverse screening compounds (37 billion molecules in 2D and 4.5 billion in 3D)
- [GDB](https://gdb.unibe.ch/downloads/): enumeration of molecules according to simple (feasibility and stability) rules
- [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp): mass spectrometry database with focus on natural products, contains untargeted (unlabelled) data.
- [MoNA](https://mona.fiehnlab.ucdavis.edu/): mass spectrometry database of real and predicted spectra for known compounds.
- [nCov-Group Data Repository](https://2019-ncovgroup.github.io/data/#dataset-downloads): SMILES, fingerprints, descriptors, and images of millions of compounds.
- [nmrshiftdb2](https://nmrshiftdb.nmr.uni-koeln.de/): is database for organic structures and their nuclear magnetic resonance (NMR) spectra. 
- [zinc20](https://files.docking.org/zinc20-ML/): ZINC20 library prepared for Deep Docking-accelerated virtual screening
- [zinc22](https://cartblanche22.docking.org/): commercially-available compounds for virtual screening

## ml structure-property benchmark datasets 

- [ACNet](https://drugai.github.io/ACNet/): a benchmark for Activity Cliff Prediction, 400K Matched Molecular Pairs (MMPs) against 190 targets, including over 20K MMP-cliffs and 380K non-AC MMPs from ChEMBL (version 28).
- [Aquasoldb](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/OVHAW8): Curation of nine open source datasets on aqueous solubility. The authors also assigned reliability groups.
- [BigSolDB](https://zenodo.org/record/6984601): Molecular solubility in organic solvents and water in a wide range of temperatures. It contains 830 unique molecules and 138 unique solvents. Temperatures range from 243.15K to 403.15K. Published in [this paper](https://chemrxiv.org/engage/chemrxiv/article-details/6426c1d8db1a20696e4c947b).
- [BindingDB](https://www.bindingdb.org/rwd/bind/chemsearch/marvin/Download.jsp): molecular recognition database, contains 2.6M data for 1.1M Compounds and 8.10K Targets (Feb 2023)
- [ChEBI-20](https://paperswithcode.com/dataset/chebi-20): 33,010 molecule-description pairs (for molecule captioning task)
- [ESol](https://pubmed.ncbi.nlm.nih.gov/15154768/): Water solubility data(log solubility in mols per litre) for common organic small molecules.
- [Flashpoint](https://github.com/cheminfo/molecule-features/blob/main/data/flashpoint/meta.yaml#:~:text=https%3A//figshare.com/articles/dataset/Data_for_Assessing_Graph%2Dbased_Deep_Learning_Models_for_Predicting_Flash_Point/9275210): Sun et al. collected a dataset of the flashpoints of 10575 molecules from academic papers, the Gelest chemical catalogue, the DIPPR database, Lange's Handbook of Chemistry, the Hazardous Chemicals Handbook, and the PubChem database.
- [FreeSolv](https://github.com/MobleyLab/FreeSolv): Experimental and Calculated Small Molecule Hydration Free Energies
- [Harvard OPV](https://figshare.com/articles/dataset/HOPV15_Dataset/1610063/4): "experimental photovoltaic data from the literature, and corresponding quantum-chemical calculations performed over a range of geometries, each with quantum chemical results using a variety of density functionals and basis sets"
- [Hydrogen Storage Materials Database](https://datahub.hymarc.org/dataset/hydrogen-storage-materials-db): data on hydrogen storage materials (information such as chemical formula and hydrogen capacity)
- [ILThermo](https://ilthermo.boulder.nist.gov/): thermodynamic and transport properties of pure ionic liquids and mixtures of them.
- [Leffingwell Odor Dataset](https://zenodo.org/record/4085098): 3523 molecules associated with expert-labeled odor descriptors from the Leffingwell PMP 2001 database
- [Limiting activity coefficients](https://polybox.ethz.ch/index.php/s/kyVOt3pwHW26PP4): for different solvent/solute pairs, used to train a SMILES-based transformer.
- [Lipophilicty](https://deepchemdata.s3-us-west-1.amazonaws.com/datasets/Lipophilicity.csv): Experimental results of octanol/water distribution coefficient(logD at pH 7.4).
- [MoleculeNet](https://moleculenet.org/datasets-1) - Benchmark suite that contains multiple datasets listed here
- [oechem](https://ochem.eu/): On Feb 17 2023 OCHEM contained 3774118 records for 689 properties (with at least 50 records) collected from 20609 sources (user is granted a Creative Commons CC-BY (version 4.0) license to data submitted)
- [Papyrus](https://doi.org/10.4121/16896406.v3): A large scale curated dataset aimed at bioactivity predictions. Contains multiple large publicly available datasets such as ChEMBL and ExCAPE-DB combined with smaller datasets.
- [Photoswitch Dataset](https://github.com/Ryan-Rhys/The-Photoswitch-Dataset): Curated dataset of 405 photoswitch molecules.
- [QM Datasets](http://quantum-machine.org/datasets/): QM7, QM7b, QM8, QM9, MD Trajectories
- [SolProp](https://discord.com/channels/850068776544108564/1074753729955381298/1076099689184772116): Database of 1 million solvent/solute COSMO-RS calculations and 10145 experimental solvation free energies (originally published as part of [this paper](https://arxiv.org/abs/2012.11730)).
- [SOMAS](https://doi.org/10.6084/m9.figshare.14552697):  Experimental and calculated solubilities for small molecules. Originally proposed for the design of redox-flow batteries.
- [Therapeutic Data Commons](https://tdcommons.ai/overview/): ML tasks that cover small molecules and biologics, including antibodies, peptides, miRNAs, and gene editing therapies. Original data can be found [here](https://doi.org/10.7910/DVN/21LKWG).
- [ThermoML Archive](https://www.nist.gov/mml/acmd/trc/thermoml/thermoml-archive): experimental thermophysical and thermochemical property data (in ThermoML XML format)

## Target identification data

- [Open Targets](https://platform.opentargets.org/): is a large-scale resource that uses human genetics and genomics data for systematic drug target identification and prioritization.
- [Probes & Drugs Portal](https://www.probes-drugs.org/data_sources): is an interactive, open data resource for chemical biology. Overview of libraries of bioactive compounds (e.g., ChEMBL, Guide to PHARMACOLOGY), including commercial screening libraries.

## Pharmacology & ADME & Metabolism

- [Cell Effective Permeability (Caco-2) dataset](https://figshare.com/collections/ADME_Properties_Evaluation_in_Drug_Discovery_Prediction_of_Caco_2_Cell_Permeability_Using_a_Combination_of_NSGA_II_and_Boosting/2867641): by Wang et al. is a dataset used to measure the absorption of drugs through intestinal tissue by simulating it using a human colon epithelial cancer cell line (Caco-2).
- [Drug–Drug–Interaction (DDI)](https://paperswithcode.com/dataset/ddi): MedLine abstracts on drug-drug interactions as well as documents describing drug-drug interactions from the DrugBank database.
- [Drug Indications Database (DID)](https://figshare.com/articles/dataset/Additional_file_1_of_Toward_a_comprehensive_drug_ontology_extraction_of_drug-indication_relations_from_diverse_information_sources/4535021): is a dataset of structured drug-indication relations. It is intended to facilitate the building of practical, comprehensive, integrated drug ontologies.
- [EPA CompTox](https://comptox.epa.gov/dashboard): is a widely used resource for chemistry, toxicity, and exposure information for hundreds of thousands of chemicals including, but not limited to, chemical properties, environmental fate, and transport, hazard, in vitro to in vivo extrapolation (IVIVE), exposure, bioactivity (each data has its license).
- [Guide to PHARMACOLOGY](https://www.guidetopharmacology.org/): is an expert-curated resource of ligand-activity-target relationships. It includes activity data even for data with unknown bioactivity value (under CC BY-SA 4.0).
- [KD-DTI](https://github.com/microsoft/BioGPT): Drug-target-interaction triplets (12K training samples, 1K validation samples and 1.1K test samples). See [paper](https://academic.oup.com/bioinformatics/article/38/22/5100/6751771?rss=1#382115390).
- [KEGG PATHWAY Database(KEGG)](https://www.genome.jp/kegg/kegg2.html): a database resource for understanding high-level functions and utilities of the biological system, such as the cell, the organism and the ecosystem, from molecular-level information, especially large-scale molecular datasets generated by genome sequencing and other high-throughput experimental technologies.
- [LOTUS](https://zenodo.org/communities/the-lotus-initiative): harmonization, curation, validation and open dissemination of 750,000+ referenced structure-organism pairs (relationships between molecular structures and the living organisms from which they were identified).
- [MetXBioDB Metabolite Biotransformations](https://zenodo.org/record/4247792#.Y_uK3NJBypN): a comprehensive collection of biotransformation reactions and metabolite information from the BioTransformer database. It includes the transformation and metabolism of metabolites.
- [PAMPA Permeability and NCATS dataset](https://doi.org/10.1177/24725552211017520): is a dataset of commonly employed assay to evaluate drug permeability across the cellular membrane to help in ADME prediction.
- [PsychonautWiki](https://psychonautwiki.org/wiki/Psychoactive_substance_index): catalog of mind-altering substances
- [QSAR datasets - Meta-QSAR (phase I & II)](https://data.mendeley.com/datasets/spwgrcnjdg/1): Data (extracted from ChEMBL) used in Olier et al. Meta-QSAR: a large-scale application of meta-learning to drug design and discovery.
- [The Human Metabolome Database (HMDB)](https://hmdb.ca/): is a freely available electronic database containing detailed information about small molecule metabolites found in the human body.
- [The Metabolism and Transport Database ](https://www-metrabase.ch.cam.ac.uk/metrabaseui/pageview/download/): is a cheminformatics and bioinformatics resource that contains curated data related to human small molecule metabolism and transport.

## reactions 

- [USPTO](https://figshare.com/articles/dataset/Chemical_reactions_from_US_patents_1976-Sep2016_/5104873): Reactions extracted by text-mining from United States patents published between 1976 and September 2016.

## high-throughput screening data

- [Dreher-Doyle](https://github.com/leojklarner/gauche/blob/main/data/reactions/dreher_doyle_science_aar5169.csv): yields and conditions for 3955 Pd-catalysed Buchwald–Hartwig C–N crosscouplings
- [Perera](https://github.com/leojklarner/gauche/blob/main/data/reactions/suzuki_miyaura_data.csv): yields and conditions for 5760 Pd-catalysed Suzuki-Miyaura C-C cross-couplings

## eln data


- [AstraZeneca ELN](https://chemrxiv.org/engage/chemrxiv/article-details/6150143118be8575b030ad43)
- [Open Reaction Database](https://docs.open-reaction-database.org/en/latest/index.html)

# related list 

- [porous materials AI gym](https://github.com/SimonEnsemble/porous-material-AI-gym): open data sets for machine learning pertaining to porous materials.
- [awesome materials informatics](https://github.com/tilde-lab/awesome-materials-informatics/edit/master/README.md): overview of software, data and initatives in the field of materials informatics 




## License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
