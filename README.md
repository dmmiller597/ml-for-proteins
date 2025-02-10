# Machine Learning for Proteins Starter Kit

## Getting Started

*   **ML/DL project template:** [lightning-hydra-template](https://github.com/ashleve/lightning-hydra-template)

*   **Protein Data:**
    *   [Protein Data Bank (PDB)](https://www.rcsb.org/):  The primary repository for protein structures.
    *   [UniProt](https://www.uniprot.org/):  A comprehensive resource for protein sequences and functional information.
    *   [AlphaFold DB](https://alphafold.ebi.ac.uk/): Database of predicted protein structures.
    * [CATH](https://www.cathdb.info/) / [TED](https://ted.cathdb.info/): Classification system for protein structural domains.

## Key Tasks and Tools

### 1. Protein Structure Prediction

Predicting the 3D structure of a protein from its amino acid sequence.

*   **AlphaFold2 / ColabFold:**  [Paper](https://www.nature.com/articles/s41586-021-03819-2) [Code](https://github.com/google-deepmind/alphafold) [Colab](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) [Docker](https://github.com/sokrypton/ColabFold/wiki/Running-ColabFold-in-Docker) - Highly accurate protein structure prediction.
*   **ESMFold:** [Paper](https://www.science.org/doi/10.1126/science.ade2574) [Code](https://github.com/facebookresearch/esm) [Server](https://esmatlas.com/resources?action=fold) - Fast, single-sequence structure prediction using a language model.
*   **RoseTTAFold:** [Paper](https://www.science.org/doi/10.1126/science.abj8754) [Code](https://github.com/RosettaCommons/RoseTTAFold) - Another accurate structure prediction method.
*   **RoseTTAFoldAllAtom:** [Paper](https://www.science.org/doi/10.1126/science.adl2528) [Code](https://github.com/baker-laboratory/RoseTTAFold-All-Atom)
*   **UMol:** [Paper](https://www.nature.com/articles/s41467-024-48837-6) [Code](https://github.com/patrickbryant1/Umol)
*   **AlphaFold2-RAVE:** [Paper](https://arxiv.org/abs/2404.07102) [Code](https://github.com/tiwarylab/alphafold2rave)

### 2. Interaction Modeling

Predicting how proteins interact with other molecules (proteins, ligands, etc.).

*   **AlphaFold3:** [Paper](https://doi.org/10.1038/s41586-024-07487-w) [Code](https://github.com/google-deepmind/alphafold3)
*   **Boltz-1:** [Paper](https://doi.org/10.1101/2024.11.19.624167) [Code](https://github.com/jwohlwend/boltz)
*   **Chai-1:** [Report](https://www.chaidiscovery.com/blog/introducing-chai-1) [Code](https://github.com/chaidiscovery/chai-lab)
* **Docking:**
    *   **DiffDock:** [Paper](https://doi.org/10.48550/arXiv.2210.01776) - Diffusion model for protein-ligand docking.
    *   **Smina:** [Paper](https://doi.org/10.1021/ci300604z) - Fork of Autodock Vina for molecular docking.
    *   **Autodock Vina:** [Paper](https://doi.org/10.1021/acs.jcim.1c00203) - Widely used docking program.
    *   **Lightdock:** [Paper](https://doi.org/10.1093/bioinformatics/btx555) - Flexible protein-protein and protein-ligand docking framework.
    *   **GeoDock:** [Paper](https://doi.org/10.1101/2023.06.29.547134) - Geometry-based docking method.

### 3. Inverse Folding (Sequence Design)

Designing protein sequences that fold into a desired 3D structure.

*   **ProteinMPNN:** [Paper](https://www.science.org/doi/10.1126/science.add2187) [Repo](https://github.com/dauparas/ProteinMPNN) -  Effective model for designing sequences for a given backbone structure.
*   **LigandMPNN:** [Paper](https://www.biorxiv.org/content/10.1101/2023.12.22.573103v1) [Repo](https://github.com/dauparas/LigandMPNN) -  Version of ProteinMPNN adapted for ligand binding sites.
*   **ESM-IF1:** [Paper](https://www.biorxiv.org/content/10.1101/2022.04.10.487779v1) [Repo](https://github.com/facebookresearch/esm) [Colab](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb) - Inverse folding using a protein language model.

### 4. Binder Design
*   **Bindcraft:** [Paper](https://www.biorxiv.org/content/10.1101/2024.09.30.615802) [Code](https://github.com/martinpacesa/BindCraft)
*   **EvoBind:** [Paper](https://www.biorxiv.org/content/10.1101/2024.06.20.599739v2) [Code](https://github.com/patrickbryant1/EvoBind)

### 5. Generative Models (Structure and Sequence)

Generating novel protein structures and sequences with desired properties.

*   **RFDiffusion:** [Paper](https://www.nature.com/articles/s41586-023-06415-8) [Code](https://github.com/RosettaCommons/RFdiffusion) [Colab](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.1/rf/examples/diffusion.ipynb) [Docker](https://github.com/RosettaCommons/RFdiffusion/blob/main/docker/Dockerfile) -  Diffusion models for protein design.
*   **RFDiffusionAllAtom:** [Paper](https://www.science.org/doi/10.1126/science.adl2528) [Code](https://github.com/baker-laboratory/rf_diffusion_all_atom)
*   **Protpardelle:** [Paper](https://www.pnas.org/doi/10.1073/pnas.2311500121) [Code](https://github.com/ProteinDesignLab/protpardelle)
*   **Chroma:** [Paper](https://www.nature.com/articles/s41586-023-06728-8) [Code](https://github.com/generatebio/chroma)
*   **ProGen:** [Paper](https://www.nature.com/articles/s41587-022-01618-2) [Code](https://github.com/salesforce/progen) - Language model for protein generation.
*   **Framediff:** [Paper](https://arxiv.org/abs/2302.02277) [Code](https://github.com/jasonkyuyim/se3_diffusion)
*   **Genie:** [Paper](https://arxiv.org/abs/2301.12485) [Code](https://github.com/aqlaboratory/genie)
*   **FoldFlow:** [Paper](https://arxiv.org/abs/2310.02391) [Code](https://github.com/DreamFold/FoldFlow)
*   **FrameFlow:** [Paper](https://arxiv.org/abs/2310.05297) [Code](https://github.com/microsoft/protein-frame-flow)
*   **Proteus:** [Paper](https://www.biorxiv.org/content/10.1101/2024.02.10.579791v1) [Code](https://github.com/Wangchentong/Proteus)
*   **Multiflow:** [Paper](https://arxiv.org/abs/2402.04997) [Code](https://github.com/jasonkyuyim/multiflow?tab=readme-ov-file)
*   **PepFlow:** [Paper](https://www.nature.com/articles/s42256-024-00860-4) [Code](https://github.com/physicshinzui/pepflow)
*   **Language Model Protein Generation:**
    *   **ProtGPT2:** [Paper](https://doi.org/10.1038/s41467-022-32007-7) -  Transformer-based model for protein sequence generation.
    *   **ZymCTRL:** [Paper](https://www.mlsb.io/papers_2022/ZymCTRL_a_conditional_language_model_for_the_controllable_generation_of_artificial_enzymes.pdf) -  Controllable generation of artificial enzymes.
    *   **ProGen2:** [Paper](https://doi.org/10.1016/j.cels.2023.10.002) - Improved protein language model.

### 6. Protein Language Models (Embeddings and Representations)

Using language models to learn representations of protein sequences.

*   **ESM-2:** [Paper](https://www.science.org/doi/10.1126/science.ade2574) [Code](https://github.com/facebookresearch/esm) -  Powerful protein language model for various downstream tasks.
*   **ESM-3:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.01.600583v2) [Code](https://github.com/evolutionaryscale/esm)
*   **SaProt:** [Paper](https://www.biorxiv.org/content/10.1101/2023.10.01.560349v1) [Code](https://github.com/westlake-repl/SaProt)
*   **ProstT5:** [Paper](https://www.biorxiv.org/content/10.1101/2023.07.23.550085v1) [Code](https://github.com/mheinzinger/ProstT5) -  Protein language model combining sequence and structure information.
*   **ProtBERT:** [Paper](https://academic.oup.com/bioinformatics/article/38/8/2102/6502274) [HuggingFace](https://huggingface.co/Rostlab/prot_bert)
*   **ProtTrans:** [Paper](https://pubmed.ncbi.nlm.nih.gov/34232869/) [Code](https://github.com/agemagician/ProtTrans)


### 7. Molecular Dynamics Simulations
* **OpenMM:** [Paper](https://doi.org/10.1371/journal.pcbi.1005659) - High-performance toolkit for molecular simulation.

### 8. Benchmarks
*   **ProteinGym:** [Paper](https://papers.nips.cc/paper_files/paper/2023/file/cac723e5ff29f65e3fcbb0739ae91bee-Paper-Datasets_and_Benchmarks.pdf) [Code](https://github.com/OATML-Markslab/ProteinGym) [Website](https://proteingym.org/)
*   **ProteinWorkshop:** [Paper](https://openreview.net/forum?id=sTYuRVrdK3) [Code](https://github.com/a-r-j/ProteinWorkshop) [Website](https://proteins.sh/)
*   **Pinder:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.17.603980v4) [Code](https://github.com/pinder-org/pinder) [Website](https://www.pinder.sh/#home)
*   **Plinder:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.17.603955v3) [Code](https://console.cloud.google.com/storage/browser/plinder) [Website](https://www.plinder.sh/)


### 9. Other Useful Tools

*   **FoldSeek:** [Paper](https://www.nature.com/articles/s41587-023-01773-0) [Code](https://github.com/steineggerlab/foldseek) [Server](https://search.foldseek.com/search) - Fast and sensitive protein structure search.
*   **MMseqs2:** [Paper](https://www.nature.com/articles/nbt.3988) [Code](https://github.com/soedinglab/MMseqs2) -  Software suite for searching and clustering large sequence sets.
*   **FoldMason:** [Paper](https://www.biorxiv.org/content/10.1101/2024.08.01.606130v3) [Code](https://github.com/steineggerlab/foldmason) [Website](https://foldmason.com/) - Multiple Protein Structure Alignment at Scale with FoldMason

### Other Resources

*   [Tools suggested by Adaptyv Bio](https://design.adaptyvbio.com/tools)
