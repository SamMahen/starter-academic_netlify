---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Extracting Adverse Drug Events from Clinical Notes'
subtitle: ''
summary: ''
authors:
- Darshini Mahendran
- Bridget McInnes T
tags: []
categories: []
date: '2021-03-25'
lastmod: 2021-03-22T00:38:59-04:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2018-03-22T04:38:59.693380Z'
publication_types:
- '2'
abstract: Adverse drug events (ADEs) are unexpected incidents caused by the administration of a drug or medication. To identify and extract these events, we require information about not just the drug itself but attributes describing the drug (e.g., strength, dosage), the reason why the drug was initially prescribed, and any adverse reaction to the drug. This paper explores the relationship between a drug and its associated attributes using relation extraction techniques. We explore three approaches- a rule-based approach, a deep learning-based approach, and a contextualized language model-based approach. We evaluate our system on the n2c2-2018 ADE extraction dataset. Our experimental results demonstrate that the contextualized language model-based approach outperformed other models overall and obtain the state-of-the-art performance in ADE extraction with a Precision of 0.93, Recall of 0.96, and an F-1 score of 0.94; however, for certain relation types, the rule-based approach obtained a higher Precision and Recall than either learning approach.
publication: 'American Medical Informatics Association (AMIA) Summits on Translational Science'
---
