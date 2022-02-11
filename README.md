# Bilateral Message Passing

We provide the implementaion & detail of the bilateral message passing [bi-MP](https://arxiv.org/abs/2202.04768) in PyTorch, DGL frameworks. 

Analogous to the bilateral image filter, we propose a bi-MP scheme to address over-smoothing in classic MP GNNs. Instead of directly propagating information through local edges, the proposed model defines a pairwise modular gradient between nodes and uses it to apply a gating mechanism to the MP layer’s aggregating function. More specifically, the bilateral-MP takes a soft assignment matrix of as input and extracts the modular gradient by applying metric learning layers to selectively transfer the messages. The key intuition is that the propagation of useful information within the same node class survives while the extraneous noise between different classes is reduced. Thus, the bilateral-MP layer results in better graph representation and improved performance by preventing over-smoothing. Our proposed scheme can be generalized to all ordinary MP GNNs.

![Figure1_upload](https://user-images.githubusercontent.com/84267304/152954507-846c98ec-3858-4143-b448-e10b072e7a9f.jpg)

Various categories contains scripts from [benchmarking-gnns](https://github.com/graphdeeplearning/benchmarking-gnns).

# Reference

  @misc{kwon2022boosting,
      title={Boosting Graph Neural Networks by Injecting Pooling in Message Passing}, <br>
      author={Hyeokjin Kwon and Jong-Min Lee}, <br>
      year={2022}, <br>
      eprint={2202.04768}, <br>
      archivePrefix={arXiv}, <br>
      primaryClass={cs.LG} <br>
  }


