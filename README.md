# ACMR (Bert4XMR): Enhancing Cross-Market Recommendations by Addressing Negative Transfer and Leveraging Item Co-occurrences
This is the Torch implementation for our paper:

>Hu Z, Nakagawa S, Cai S M, et al. Enhancing cross-market recommendations by addressing negative transfer and leveraging item co-occurrences[J]. Information Systems, 2024: 102388.

## Introduction
We introduce a novel attention based model that exploits users’ historical behaviors to mine general patterns from item co-occurrences and designs market-specific embeddings to mitigate negative transfer. Specifically, we propose an attention-based user interest mining module to harness the potential of common items as bridges for mining general knowledge from item co-occurrence patterns through rich data derived from global markets. In order to mitigate the adverse effects of negative transfer, we decouple the item representations into market-specific embeddings and market-agnostic embeddings. The market-specific embeddings effectively model the inherent biases associated with different markets, while the market-agnostic embeddings learn generic representations of the items.

## Old version on Arxiv
Old version: [Bert4XMR: Cross-Market Recommendation with Bidirectional Encoder Representations from Transformer](https://arxiv.org/abs/2305.15145).

## Latest Version
For more comprehensive analysis and experiments, please refer to our latest edition published on Information Systems: [Enhancing cross-market recommendations by addressing negative transfer and leveraging item co-occurrences](https://doi.org/10.1016/j.is.2024.102388).

## Environment Requirement
The code has been tested running under Python 3.6.5. The required packages are as follows:
* torch == 1.13.0

## Reproducibility & Example to Run the Codes
To demonstrate the reproducibility of the best performance reported in our paper and faciliate researchers to track whether the model status is consistent with ours, we provide [the log of one random run of our model](https://github.com/laowangzi/ACMR/tree/main/log) (the paper reports the average results of five independent replicates of randomly initializing parameters and splitting the dataset).

The instruction of commands has been clearly stated in the codes (see the config.py). 
* To run the code:
```
python train_model.py
```

## Citation 
If you want to use our codes and datasets in your research, please cite:
```
@article{HU2024102388,
title = {Enhancing cross-market recommendations by addressing negative transfer and leveraging item co-occurrences},
journal = {Information Systems},
volume = {124},
pages = {102388},
year = {2024},
issn = {0306-4379},
doi = {https://doi.org/10.1016/j.is.2024.102388},
author = {Zheng Hu and Satoshi Nakagawa and Shi-Min Cai and Fuji Ren and Jiawen Deng},
keywords = {Recommender systems, Cross-market recommendation, Transfer learning}
}
```
