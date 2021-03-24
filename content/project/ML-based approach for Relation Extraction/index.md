---
title: Rule based approach for relation extraction using NLP - RelEx (Rule-based)
summary: Determines the relation between two entities utilizing the co-location information between them.
tags:
- NLP
date: "2018-02-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Graph-based traversal algorithm
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

Our machine learning-based  approach presents a feature-vector based, supervised machine learning approach to extract explicit semantic relations and classify them. Our approach takes sentences as the input, defines a set of features, and combines them into a feature vector to train a machine learning model. This is the most crucial part of our approach. The idea is to decrease the size of the effective vocabulary, which would increase the classification accuracy by eliminating the noise in the feature representation. Relations between entities are extracted and classified through this learned system. The figure shows the pipeline of our approach. In the final step of our approach, a feature vector is generated for each sentence by incorporating the extracted features in the previous step. The generated feature vector is then used to train a classifier that classifies the relation between the entities. The following classifiers, which represent three main classification algorithms, are available to train and evaluate the data set in our approach:\footnote{Natural Language Toolkit's (NLTK) sci-kit learn library classifiers are used.} Decision Trees, Naive Bayes (NB), and SVMs. The resulting model is then used to classify the relations.