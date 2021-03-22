---
title: Rule based approach for relation extraction using NLP - RelEx (Rule-based)
summary: Determines the relation between two entities utilizing the co-location information between them.
tags:
- NLP
date: "2018-02-01T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: "https://github.com/NLPatVCU/RelEx"

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

Our rule-based approach determines whether a relation exists between two entities utilizing the co-location information between them. We use a Breadth-First Search algorithm (BFS) to find the selected entity's closest occurrence on either side of other entities. For each entity, we traverse both sides until the selected entity's closest occurrence is found based on the provided span values of the entities. We explore four traversal mechanisms: traverse left side only, traverse right side only, traverse left first then right and vice versa.  
