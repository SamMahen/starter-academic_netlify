---
title: BERT-based approach for relation extraction using NLP - RelEx-BERT
summary:  Explores using BERT contextualized embeddings into a simple feed-forward neural network.
tags:
- NLP
date: "2020-07-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: BERT-based approach
  focal_point: Smart

links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: "https://github.com/SamMahen/RelEx-BERT"
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

Our BERT-based approach explores using BERT contextualized embeddings into a simple feed-forward neural network. We first extract the sentence containing the relation and pass it through a pre-trained BERT model. The output is then fed into a dropout layer and then into a fully-connected dense layer for classification. As with our deep learning-based approaches, we treat the RE as a binary classification task building a separate model for each drug-entity type. Figure shows the architecture of our BERT-based approach. Our approach contains the following BERT-based language models:

* *BERT (-cased and -uncased)* - Original BERT models trained on a large corpus of English data: BookCorpus (800M words) and Wikipedia (2,500M words) in a self-supervised manner (without human annotation). 
* *BioBERT* - Model is initialized with the general BERT and further trained over a corpus of biomedical research articles from PubMed[^1] abstracts and PubMed Central[^2] article full texts.
* *Clinical BERT* - Model is initialized with BioBERT and further fine-tuned over the Medical Information Mart for Intensive Care-III (MIMIC-III) clinical note corpus.

[^1]: https://www.ncbi.nlm.nih.gov/pubmed/
[^2]: https://www.ncbi.nlm.nih.gov/pmc/
