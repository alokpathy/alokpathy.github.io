+++
title = "Distributed Matrix-Based Sampling for Graph Neural Network Training"
date = 2023-11-06T14:43:34-04:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Graph Neural Networks", "Graph-Reprsentation Learning"]
categories = []

authors = ["Alok Tripathy", "Katherine Yelick", "Aydın Buluç"]
publication_types = ["3"]

abstract = "Graph Neural Networks (GNNs) offer a compact and computationally efficient way to learn embeddings and classifications on graph data. GNN models are frequently large, making distributed minibatch training necessary. The primary contribution of this paper is new methods for reducing communication in the sampling step for distributed GNN training. Here, we propose a matrix-based bulk sampling approach that expresses sampling as a sparse matrix multiplication (SpGEMM) and samples multiple minibatches at once. When the input graph topology does not fit on a single device, our method distributes the graph and use communication-avoiding SpGEMM algorithms to scale GNN minibatch sampling, enabling GNN training on much larger graphs than those that can fit into a single device memory. When the input graph topology (but not the embeddings) fits in the memory of one GPU, our approach (1) performs sampling without communication, (2) amortizes the overheads of sampling a minibatch, and (3) can represent multiple sampling algorithms by simply using different matrix constructions. In addition to new methods for sampling, we show that judiciously replicating feature data with a simple all-to-all exchange can outperform current methods for the feature extraction step in distributed GNN training. We provide experimental results on the largest Open Graph Benchmark (OGB) datasets on 128 GPUs, and show that our pipeline is 2.5× faster Quiver (a distributed extension to PyTorch-Geometric) on a 3-layer GraphSAGE network. On datasets outside of OGB, we show a 8.46× speedup on 128 GPUs in-per epoch time. Finally, we show scaling when the graph is distributed across GPUs and scaling for both node-wise and layer-wise sampling algorithms"

url_pdf = "https://arxiv.org/pdf/2311.02909.pdf"

publication_short = "arXiv:2311.02909"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++
