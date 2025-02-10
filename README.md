# Machine Learning for Proteins Starter Kit

<div align="center">
  <img src="./protein.gif" alt="Protein Structure Animation" title="Protein Structure Animation" width="400"/>
  <br>
</div>


## Getting Started

*   **Project template:** [lightning-hydra-template](https://github.com/ashleve/lightning-hydra-template)

*   **Protein Data:**
    *   [Protein Data Bank (PDB)](https://www.rcsb.org/):  The primary repository for protein structures.
    *   [UniProt](https://www.uniprot.org/):  A comprehensive resource for protein sequences and functional information.
    *   [AlphaFold DB](https://alphafold.ebi.ac.uk/): Database of predicted protein structures.
    * [CATH](https://www.cathdb.info/) / [TED](https://ted.cathdb.info/): Classification system for protein structural domains.

## Key Tasks and Tools

### 1. Protein Structure Prediction

Predicting the 3D structure of a protein from its amino acid sequence.

*   **AlphaFold2 / ColabFold:**  [Paper](https://www.nature.com/articles/s41586-021-03819-2) [Code](https://github.com/google-deepmind/alphafold) [Colab](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) - Highly accurate protein structure prediction.
*   **ESMFold:** [Paper](https://www.science.org/doi/10.1126/science.ade2574) [Code](https://github.com/facebookresearch/esm) [Server](https://esmatlas.com/resources?action=fold) - Fast, single-sequence structure prediction using a language model.
*   **RoseTTAFold/RoseTTAFoldAllAtom:** [Paper (RF)](https://www.science.org/doi/10.1126/science.abj8754) [Paper (RF-AA)](https://www.science.org/doi/10.1126/science.adl2528) [Code (RF)](https://github.com/RosettaCommons/RoseTTAFold) [Code (RF-AA)](https://github.com/baker-laboratory/RoseTTAFold-All-Atom) - Accurate structure prediction methods from the Baker lab, with the All-Atom version providing full atomic detail.

### 2. Interaction Modeling

Predicting how proteins interact with other molecules (proteins, ligands, etc.).

*   **AlphaFold3:** [Paper](https://doi.org/10.1038/s41586-024-07487-w) [Code](https://github.com/google-deepmind/alphafold3)
*   **Boltz-1:** [Paper](https://doi.org/10.1101/2024.11.19.624167) [Code](https://github.com/jwohlwend/boltz)
*   **Chai-1:** [Report](https://www.chaidiscovery.com/blog/introducing-chai-1) [Code](https://github.com/chaidiscovery/chai-lab)
* **Docking:**
    *   **DiffDock-L:** [Paper](https://arxiv.org/abs/2402.18396) [Code](https://github.com/gcorso/DiffDock) - Diffusion model for protein-ligand docking.
    *   **FlowDock:** [Paper](https://arxiv.org/abs/2412.10966) [Code](https://github.com/BioinfoMachineLearning/FlowDock) - Flow-based protein-ligand docking.

### 3. Inverse Folding (Sequence Design)

Designing protein sequences that fold into a desired 3D structure.

*   **ProteinMPNN:** [Paper](https://www.science.org/doi/10.1126/science.add2187) [Repo](https://github.com/dauparas/ProteinMPNN) -  Effective model for designing sequences for a given backbone structure.
*   **LigandMPNN:** [Paper](https://www.biorxiv.org/content/10.1101/2023.12.22.573103v1) [Repo](https://github.com/dauparas/LigandMPNN) -  Version of ProteinMPNN adapted for ligand binding sites.
*   **ESM-IF1:** [Paper](https://www.biorxiv.org/content/10.1101/2022.04.10.487779v2) [Repo](https://github.com/facebookresearch/esm) [Colab](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb) - Inverse folding using a protein language model.

### 4. Binder Design

Designing protein sequences that bind to a specific target.

*   **Bindcraft:** [Paper](https://www.biorxiv.org/content/10.1101/2024.09.30.615802) [Code](https://github.com/martinpacesa/BindCraft)
*   **EvoBind:** [Paper](https://www.biorxiv.org/content/10.1101/2024.06.20.599739v2) [Code](https://github.com/patrickbryant1/EvoBind)

### 5. Generative Models (Structure and Sequence)

Generating novel protein structures and sequences with desired properties.

*   **RFDiffusion/RFDiffusionAllAtom:** [Paper (RF)](https://www.nature.com/articles/s41586-023-06415-8) [Paper (RF-AA)](https://www.science.org/doi/10.1126/science.adl2528) [Code (RF)](https://github.com/RosettaCommons/RFdiffusion) [Code (RF-AA)](https://github.com/baker-laboratory/rf_diffusion_all_atom) [Colab](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.1/rf/examples/diffusion.ipynb) - Diffusion models for protein design, with the All-Atom version providing full atomic detail.
*   **Protpardelle:** [Paper](https://www.pnas.org/doi/10.1073/pnas.2311500121) [Code](https://github.com/ProteinDesignLab/protpardelle)
*   **Chroma:** [Paper](https://www.nature.com/articles/s41586-023-06728-8) [Code](https://github.com/generatebio/chroma)
*   **Framediff:** [Paper](https://arxiv.org/abs/2302.02277) [Code](https://github.com/jasonkyuyim/se3_diffusion)
*   **Genie:** [Paper](https://arxiv.org/abs/2301.12485) [Code](https://github.com/aqlaboratory/genie)
*   **FoldFlow:** [Paper](https://arxiv.org/abs/2310.02391) [Code](https://github.com/DreamFold/FoldFlow)
*   **FrameFlow:** [Paper](https://arxiv.org/abs/2310.05297) [Code](https://github.com/microsoft/protein-frame-flow)
*   **Multiflow:** [Paper](https://arxiv.org/abs/2402.04997) [Code](https://github.com/jasonkyuyim/multiflow?tab=readme-ov-file)
*   **Language Model Protein Generation:**
    *   **ProtGPT2:** [Paper](https://doi.org/10.1038/s41467-022-32007-7) -  Transformer-based model for protein sequence generation.
    *   **ZymCTRL:** [Paper](https://www.mlsb.io/papers_2022/ZymCTRL_a_conditional_language_model_for_the_controllable_generation_of_artificial_enzymes.pdf) -  Controllable generation of artificial enzymes.

### 6. Protein Language Models (Embeddings and Representations)

Using language models to learn representations of protein sequences.

*   **ESM-2:** [Paper](https://www.science.org/doi/10.1126/science.ade2574) [Code](https://github.com/facebookresearch/esm)
*   **ESM-3:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.01.600583v2) [Code](https://github.com/evolutionaryscale/esm)
*   **ProtTrans:** [Paper](https://pubmed.ncbi.nlm.nih.gov/34232869/) [Code](https://github.com/agemagician/ProtTrans)
*   **ProstT5:** [Paper](https://www.biorxiv.org/content/10.1101/2023.07.23.550085v2) [Code](https://github.com/mheinzinger/ProstT5)
*   **SaProt:** [Paper](https://www.biorxiv.org/content/10.1101/2023.10.01.560349v5) [Code](https://github.com/westlake-repl/SaProt)
*   **PoET:** [Paper](https://arxiv.org/abs/2306.06156) [Code](https://github.com/OpenProteinAI/PoET)

### 7. Benchmarks

*   **ProteinGym:** [Paper](https://papers.nips.cc/paper_files/paper/2023/file/cac723e5ff29f65e3fcbb0739ae91bee-Paper-Datasets_and_Benchmarks.pdf) [Code](https://github.com/OATML-Markslab/ProteinGym) [Website](https://proteingym.org/)
*   **ProteinWorkshop:** [Paper](https://openreview.net/forum?id=sTYuRVrdK3) [Code](https://github.com/a-r-j/ProteinWorkshop) [Website](https://proteins.sh/)
*   **Pinder:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.17.603980v4) [Code](https://github.com/pinder-org/pinder) [Website](https://www.pinder.sh/#home)
*   **Plinder:** [Paper](https://www.biorxiv.org/content/10.1101/2024.07.17.603955v3) [Code](https://console.cloud.google.com/storage/browser/plinder) [Website](https://www.plinder.sh/)


### 8. Other Useful Tools

*   **FoldSeek:** [Paper](https://www.nature.com/articles/s41587-023-01773-0) [Code](https://github.com/steineggerlab/foldseek) [Server](https://search.foldseek.com/search) - Fast and sensitive protein structure search.
*   **MMseqs2:** [Paper](https://www.nature.com/articles/nbt.3988) [Code](https://github.com/soedinglab/MMseqs2) -  Software suite for searching and clustering large sequence sets.
*   **FoldMason:** [Paper](https://www.biorxiv.org/content/10.1101/2024.08.01.606130v3) [Code](https://github.com/steineggerlab/foldmason) [Website](https://foldmason.com/) - Multiple Protein Structure Alignment at Scale with FoldMason

### Other Resources

*   [biolists](https://github.com/biolists) and [yangkky/Machine-learning-for-proteins](https://github.com/yangkky/Machine-learning-for-proteins)
*   [Tools suggested by Adaptyv Bio](https://design.adaptyvbio.com/tools)
*   [MolecularNodes](https://bradyajohnston.github.io/MolecularNodes/)
*   [Molstar](https://molstar.org/)
