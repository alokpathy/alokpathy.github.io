+++
title = "Reducing Communication in Graph Neural Network Training"
date = 2020-05-09T14:43:34-04:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = ["Graph Neural Networks", "Graph-Representation Learning"]
categories = []

authors = ["Alok Tripathy", "Katherine Yelick", "Aydın Buluç"]
publication_types = ["1"]

abstract = "Graph Neural Networks (GNNs) are powerful and flexible neural networks that use the naturally sparse connectivity information of the data. GNNs represent this connectivity as sparse matrices, which have lower arithmetic intensity and thus higher communication costs compared to dense matrices, making GNNs harder to scale to high concurrencies than convolutional or fully-connected neural networks. We present a family of parallel algorithms for training GNNs. These algorithms are based on their counterparts in dense and sparse linear algebra, but they had not been previously applied to GNN training. We show that they can asymptotically reduce communication compared to existing parallel GNN training methods. We implement a promising and practical version that is based on 2D sparse-dense matrix multiplication using torch.distributed. Our implementation parallelizes over GPU-equipped clusters. We train GNNs on up to a hundred GPUs on datasets that include a protein network with over a billion edges."

url_pdf = "https://arxiv.org/pdf/2005.03300.pdf"

publication_short = "ACM/IEEE International Conference for High Performance Computing, Networking, Storage and Analysis, arXiv:2005.03300"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++
