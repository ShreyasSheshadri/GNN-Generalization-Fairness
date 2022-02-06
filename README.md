# GNN-Generalization-Fairness

This repo provides the official implementations for the experiments described in the following paper:

[**Subgroup Generalization and Fairness of Graph Neural Networks**](https://arxiv.org/abs/2106.15535)

Jiaqi Ma\*, Junwei Deng\*, and Qiaozhu Mei. NeurIPS 2021.

(\*: equal constribution)

## Installation

### Planetoid Dependencies
- ~~torch 1.8.0~~ `pytorch-1.8.1`
- ~~dgl 0.4.3~~ `dgl-0.6.1`
- networkx 2.4  
- ~~numpy 1.17.3~~ `numpy-1.21.2`
  
### OGB Dependencies
- ~~torch 1.8.2~~ `pytorch-1.8.1`
- ~~torch-geometric~~ `pyg-2.0.1`
- networkx 2.4
- ogb 1.3.2
- ~~numpy 1.17.3~~ `numpy-1.21.2`

### Installation

If you choose to install the dependencies individually:
```
conda install pytorch=1.8 -c pytorch
conda install pyg -c pyg -c conda-forge
conda install networkx=2.4
conda install ogb==1.3.2 -c conda-forge
pip install dgl
```

For REPL (`ipython`), we install: `conda install notebook`.

Else, recreate the `ma` conda environment: 
```
conda env create --file conda-envs/ma.yml
```

Activate with `conda activate ma`, and deactivate with `conda deactivate`.

**NOTE**: The specified version set is unsatisfiable: e.g., a) `numpy==1.17.3 -> python[version='>=3.6,<3.7.0a0|>=3.7,<3.8.0a0|>=3.8,<3.9.0a0']`),b) `pytorch-sparse==0.6.12 -> pytorch=1.8`, and, c) `pytorch-sparse==0.6.12 -> python[version='>=3.9,<3.10.0a0'] -> libffi[version='>=3.3,<3.4.0a0']`.

## Run the code

Please refer to the readme in each subfolder.

## Cite
```
@article{DBLP:journals/corr/abs-2106-15535,
  author    = {Jiaqi Ma, Junwei Deng, Qiaozhu Mei},
  title     = {Subgroup Generalization and Fairness of Graph Neural Networks},
  journal   = {CoRR},
  volume    = {abs/2106.15535},
  year      = {2021},
  url       = {https://arxiv.org/abs/2106.15535},
  eprinttype = {arXiv},
  eprint    = {2106.15535},
  timestamp = {Mon, 05 Jul 2021 15:15:50 +0200},
  biburl    = {https://dblp.org/rec/journals/corr/abs-2106-15535.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```
