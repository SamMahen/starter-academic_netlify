---
title: K-Nearest Neighbors algorithm (KNN) on Cuda
summary: Developing KNN algorithm on the GPU (Graphics Processing Unit) using CUDA.
tags:
- NLP
date: "2019-09-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Mappings of the different kernel configurations.
  focal_point: Smart

links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

KNN is a simple classification algorithm. The algorithm
is based on the feature similarity, it classifies a given data
point based on how closely out-of-sample attributes, it re-
sembles the training set. Three different kernel configurations
are implemented: 1D grid and 1D-x block mapping (thread
per instance), 1D grid and 1D-x block mapping with shared
memory (block per instance), 1D grid of 2D blocks mapping
(column per instance).The number of k is taken as a user
parameter. Code is optimized as both the accuracy of the
sequential and MPI and Cuda versions are same. The grid
and block size are determined depending on the number of
threads assigned per block.

*1D grid and 1D-x block mapping* - First approach is a 1D grid with 1D-x block mapping. For
a given dataset, each thread is assigned to perform KNN for a
particular instance. Number of threads are equal to the number
of instances. Depending on the number of threads per block,
the block number is determined. The mapping for Approach
1 is shown in Figure. 

*1D grid and 1D-x block mapping with shared memory* - Second approach, is 1D grid and 1D-x block mapping
with shared memory. For a given dataset, each block is
assigned to perform KNN for a particular instance. Euclidean
distance calculation of one instance with all other instances are
divided between the threads in each block. Since all threads
in the block are performing the euclidean distance calculation
simultaneously, the distance matrix is initialized in the shared
memory where all threads were synchronized before selecting
the k number of nearest of elements. Since multiple threads are
assigned to one instance instead of one thread the processing time is reduced which makes this mapping more efficient than
the Approach 1

*1D grid of 2D blocks mapping* - Third approach is a 1D grid divided into 2D blocks and are
indexed using row and column values. For a given dataset,
each column is assigned to perform KNN for a particular
instance. The euclidean distance calculation performed by
different threads are written to a 2D matrix in the shared
memory and read into a temporary array while selecting the
k number of nearest of elements. Since one block is assigned
to more than one instance to perform KNN, this reduces the
time compared to the approach where a thread is assigned
to an instance but not than the approach where each block is
assigned one instance.