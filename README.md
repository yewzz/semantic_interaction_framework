# A PyTorch Implementation of the Semantic Interaction Learning

The code for the ACL 2023 paper “Weakly-Supervised Spoken Video Grounding via Semantic Interaction Learning”.

### Requirements

- Ubuntu 18.04
- CUDA 11.4
- Python 3.7
- Pytorch 1.9


## Data Preparation
The visual features of ActivityNet Caption can be downloaded from [here](https://cs.stanford.edu/people/ranjaykrishna/densevid/).
The speech data can be downloaded from [here](https://drive.google.com/file/d/11f6sC94Swov_opNfpleTlVGyLJDFS5IW/view?usp=sharing).



## Training procedure

To pretrain the model using the LibriSpeech dataset.

Run `python train.py --config-path='config/activitynet/config_pretrain.json' `

To train the model for weakly-supervised spoken video grounding.

Run `python train.py --config-path='config/activitynet/config_weak_graph.json' `
