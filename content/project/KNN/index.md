---
title: K-Nearest Neighbors algorithm (KNN) on Cuda
summary: Developing KNN algorithm on the GPU (Graphics Processing Unit) using CUDA.
tags:
- Other
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
url_pdf: "media/KNN.pdf"
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
