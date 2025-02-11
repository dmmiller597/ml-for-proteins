# Machine Learning for Proteins Starter Kit

<div align="center">
  <img src="./p3.png" alt="Protein Structure Animation"/>
  
  A curated collection of machine learning tools for proteins

</div>

## Contents

- [Getting Started](#getting-started)
- [Data Sources](#data-sources)
- [Key Tools](#key-tools)
  - [Structure Prediction](#1-structure-prediction)
  - [Interaction Modeling](#2-interaction-modeling)
  - [Sequence Design](#3-sequence-design)
  - [Binder Design](#4-binder-design)
  - [Generative Models](#5-generative-models)
  - [Language Models](#6-language-models)
  - [Benchmarks](#7-benchmarks)
  - [Utility Tools](#8-utility-tools)

## Getting Started

 [PyTorch Lightning + Hydra.](https://github.com/ashleve/lightning-hydra-template) A very user-friendly template for ML experimentation 

## Data Sources

| Resource | Description |
|----------|-------------|
| [Protein Data Bank (PDB)](https://www.rcsb.org/) | Primary repository for protein structures |
| [UniProt](https://www.uniprot.org/) | Comprehensive protein sequence database |
| [AlphaFold DB](https://alphafold.ebi.ac.uk/) | Predicted protein structures |
| [CATH](https://www.cathdb.info/) / [TED](https://ted.cathdb.info/) | Protein domain classification |

## Key Tools

### 1. Structure Prediction

<details open>
<summary>Tools for predicting 3D protein structures from sequences</summary>

- **AlphaFold2 / ColabFold** - State-of-the-art structure prediction
  - [[Paper]](https://www.nature.com/articles/s41586-021-03819-2) [[Code]](https://github.com/google-deepmind/alphafold) [[Colab]](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb)
- **ESMFold** - Fast, single-sequence prediction
  - [[Paper]](https://www.science.org/doi/10.1126/science.ade2574) [[Code]](https://github.com/facebookresearch/esm) [[Server]](https://esmatlas.com/resources?action=fold)
- **RoseTTAFold/RoseTTAFoldAllAtom** - Accurate structure prediction methods
  - [[Paper (RF)]](https://www.science.org/doi/10.1126/science.abj8754) [[Paper (RF-AA)]](https://www.science.org/doi/10.1126/science.adl2528)
  - [[Code (RF)]](https://github.com/RosettaCommons/RoseTTAFold) [[Code (RF-AA)]](https://github.com/baker-laboratory/RoseTTAFold-All-Atom)
</details>

### 2. Interaction Modeling

<details open>
<summary>Tools for protein-molecule interaction prediction</summary>

- **AlphaFold3** - [[Paper]](https://doi.org/10.1038/s41586-024-07487-w) [[Code]](https://github.com/google-deepmind/alphafold3)
- **Boltz-1** - [[Paper]](https://doi.org/10.1101/2024.11.19.624167) [[Code]](https://github.com/jwohlwend/boltz)
- **Chai-1** - [[Report]](https://www.chaidiscovery.com/blog/introducing-chai-1) [[Code]](https://github.com/chaidiscovery/chai-lab)

**Docking Tools:**
- **DiffDock-L** - Diffusion model for protein-ligand docking
  - [[Paper]](https://arxiv.org/abs/2402.18396) [[Code]](https://github.com/gcorso/DiffDock)
- **FlowDock** - Flow-based protein-ligand docking
  - [[Paper]](https://arxiv.org/abs/2412.10966) [[Code]](https://github.com/BioinfoMachineLearning/FlowDock)
</details>

### 3. Sequence Design

<details open>
<summary>Tools for inverse folding and sequence generation</summary>

- **ProteinMPNN** - Backbone sequence design
  - [[Paper]](https://www.science.org/doi/10.1126/science.add2187) [[Code]](https://github.com/dauparas/ProteinMPNN)
- **LigandMPNN** - Ligand-aware sequence design
  - [[Paper]](https://www.biorxiv.org/content/10.1101/2023.12.22.573103v1) [[Code]](https://github.com/dauparas/LigandMPNN)
- **ESM-IF1** - Language model-based inverse folding
  - [[Paper]](https://www.biorxiv.org/content/10.1101/2022.04.10.487779v2) [[Code]](https://github.com/facebookresearch/esm) [[Colab]](https://colab.research.google.com/github/facebookresearch/esm/blob/main/examples/inverse_folding/notebook.ipynb)
</details>

### 4. Binder Design

<details open>
<summary>Tools for designing protein-target binding</summary>

- **Bindcraft** - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.09.30.615802) [[Code]](https://github.com/martinpacesa/BindCraft)
- **EvoBind** - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.06.20.599739v2) [[Code]](https://github.com/patrickbryant1/EvoBind)
</details>

### 5. Generative Models

<details open>
<summary>Tools for generating novel proteins</summary>

- **RFDiffusion/RFDiffusionAllAtom** - Diffusion models for protein design
  - [[Paper]](https://www.nature.com/articles/s41586-023-06415-8) [[Code]](https://github.com/RosettaCommons/RFdiffusion)
- **Protpardelle** - [[Paper]](https://www.pnas.org/doi/10.1073/pnas.2311500121) [[Code]](https://github.com/ProteinDesignLab/protpardelle)
- **Chroma** - [[Paper]](https://www.nature.com/articles/s41586-023-06728-8) [[Code]](https://github.com/generatebio/chroma)

**Additional Models:**
- **Framediff** - [[Paper]](https://arxiv.org/abs/2302.02277) [[Code]](https://github.com/jasonkyuyim/se3_diffusion)
- **Genie** - [[Paper]](https://arxiv.org/abs/2301.12485) [[Code]](https://github.com/aqlaboratory/genie)
- **FoldFlow** - [[Paper]](https://arxiv.org/abs/2310.02391) [[Code]](https://github.com/DreamFold/FoldFlow)
- **FrameFlow** - [[Paper]](https://arxiv.org/abs/2310.05297) [[Code]](https://github.com/microsoft/protein-frame-flow)
- **Multiflow** - [[Paper]](https://arxiv.org/abs/2402.04997) [[Code]](https://github.com/jasonkyuyim/multiflow)

**Language Model Generation:**
- **ProtGPT2** - Transformer-based sequence generation
  - [[Paper]](https://doi.org/10.1038/s41467-022-32007-7)
- **ZymCTRL** - Controllable enzyme generation
  - [[Paper]](https://www.mlsb.io/papers_2022/ZymCTRL_a_conditional_language_model_for_the_controllable_generation_of_artificial_enzymes.pdf)
</details>

### 6. Language Models

<details open>
<summary>Protein language models and embeddings</summary>

- **ESM-2** - [[Paper]](https://www.science.org/doi/10.1126/science.ade2574) [[Code]](https://github.com/facebookresearch/esm)
- **ESM-3** - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.07.01.600583v2) [[Code]](https://github.com/evolutionaryscale/esm)
- **ProtTrans** - [[Paper]](https://pubmed.ncbi.nlm.nih.gov/34232869/) [[Code]](https://github.com/agemagician/ProtTrans)
- **ProstT5** - [[Paper]](https://www.biorxiv.org/content/10.1101/2023.07.23.550085v2) [[Code]](https://github.com/mheinzinger/ProstT5)
- **SaProt** - [[Paper]](https://www.biorxiv.org/content/10.1101/2023.10.01.560349v5) [[Code]](https://github.com/westlake-repl/SaProt)
- **PoET** - [[Paper]](https://arxiv.org/abs/2306.06156) [[Code]](https://github.com/OpenProteinAI/PoET)
</details>

### 7. Benchmarks

<details open>
<summary>Evaluation frameworks and benchmarks</summary>

- **ProteinGym** - Comprehensive evaluation suite
  - [[Paper]](https://papers.nips.cc/paper_files/paper/2023/file/cac723e5ff29f65e3fcbb0739ae91bee-Paper-Datasets_and_Benchmarks.pdf) [[Code]](https://github.com/OATML-Markslab/ProteinGym) [[Website]](https://proteingym.org/)
- **ProteinWorkshop** - Standardized benchmarking platform
  - [[Paper]](https://openreview.net/forum?id=sTYuRVrdK3) [[Code]](https://github.com/a-r-j/ProteinWorkshop) [[Website]](https://proteins.sh/)
- **Pinder** - Protein-protein interaction benchmark
  - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.07.17.603980v4) [[Code]](https://github.com/pinder-org/pinder) [[Website]](https://www.pinder.sh/)
- **Plinder** - Protein-ligand interaction benchmark
  - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.07.17.603955v3) [[Code]](https://console.cloud.google.com/storage/browser/plinder) [[Website]](https://www.plinder.sh/)
</details>

### 8. Utility Tools

<details open>
<summary>Supporting tools and utilities</summary>

- **FoldSeek** - Fast structure search
  - [[Paper]](https://www.nature.com/articles/s41587-023-01773-0) [[Code]](https://github.com/steineggerlab/foldseek) [[Server]](https://search.foldseek.com/search)
- **MMseqs2** - Sequence search and clustering
  - [[Paper]](https://www.nature.com/articles/nbt.3988) [[Code]](https://github.com/soedinglab/MMseqs2)
- **FoldMason** - Structure alignment at scale
  - [[Paper]](https://www.biorxiv.org/content/10.1101/2024.08.01.606130v3) [[Code]](https://github.com/steineggerlab/foldmason) [[Website]](https://foldmason.com/)
</details>

## Additional Resources

<details open>
<summary>Useful Links & Tools</summary>

- [biolists](https://github.com/biolists) - Curated biological resource lists
- [Machine-learning-for-proteins](https://github.com/yangkky/Machine-learning-for-proteins)
- [Adaptyv Bio Tools List](https://design.adaptyvbio.com/tools)
- [MolecularNodes](https://bradyajohnston.github.io/MolecularNodes/)
- [Molstar](https://molstar.org/) - Molecular visualization
</details>

---
