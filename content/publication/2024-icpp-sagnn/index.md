+++
title = "Sparsity-Aware Communication for Distributed Graph Neural Network Training"
date = 2024-08-12T14:43:34-04:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Graph Neural Networks", "Graph-Representation Learning"]
categories = []

authors = ["Ujjaini Mukhopadhyay", "Alok Tripathy", "Oguz Selvitopi", "Katherine Yelick", "Aydın Buluç"]
publication_types = ["1"]

abstract = "Graph Neural Networks (GNNs) are a computationally efficient method to learn embeddings and classifications on graph data. However, GNN training has low computational intensity, making communication costs the bottleneck for scalability. Sparse-matrix dense-matrix multiplication (SpMM) is the core computational operation in full-graph training of GNNs. Previous work parallelizing this operation focused on sparsity-oblivious algorithms, where matrix elements are communicated regardless of the sparsity pattern. This leads to a predictable communication pattern that can be overlapped with computation and enables the use of collective communication operations at the expense of wasting significant bandwidth by communicating unnecessary data.  We develop sparsity-aware algorithms that tackle the communication bottlenecks in GNN training with three novel approaches. First, we communicate only the necessary matrix elements. Second, we utilize a graph partitioning model to reorder the matrix and drastically reduce the amount of communicated elements. Finally, we address the high load imbalance in communication with a tailored partitioning model, which minimizes both the total communication volume and the maximum sending volume. We further couple these sparsity-exploiting approaches with a communication-avoiding approach (1.5D parallel SpMM) in which submatrices are replicated to reduce communication. We explore the tradeoffs of these combined optimizations and show up to 14 × improvement on 256 GPUs and on some instances reducing communication to almost zero resulting in a communication-free parallel training relative to a popular GNN framework based on communication-oblivious SpMM."

url_pdf = "https://dl.acm.org/doi/abs/10.1145/3673038.3673152"

publication_short = "Proceedings of the 53rd International Conference on Parallel Processing"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++
