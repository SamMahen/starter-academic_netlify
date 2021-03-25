---
title: Extracting Adverse Drug Events from Clinical Notes

event: AMIA 2021 Virtual Informatics Summit
event_url: https://www.amia.org/summit2021

location: Virtual
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: Exploring different approaches for ADE Extraction
abstract: "Adverse drug events (ADEs) are unexpected incidents caused by the administration of a drug or medication. To
identify and extract these events, we require information about not just the drug itself but attributes describing the
drug (e.g., strength, dosage), the reason why the drug was initially prescribed, and any adverse reaction to the drug.
This paper explores the relationship between a drug and its associated attributes using relation extraction techniques.
We explore three approaches: a rule-based approach, a deep learning-based approach, and a contextualized language
model-based approach. We evaluate our system on the n2c2-2018 ADE extraction dataset. Our experimental results
demonstrate that the contextualized language model-based approach outperformed other models overall and obtain
the state-of-the-art performance in ADE extraction with a Precision of 0.93, Recall of 0.96, and an F 1 score of
0.94; however, for certain relation types, the rule-based approach obtained a higher Precision and Recall than either
learning approach."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2021-03-25T10:00:00Z"
date_end: "2021-03-25T11:30:00Z"
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  focal_point: Right

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: "media/AMIA_2021.pdf"
url_slides: ""
url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
- example
---

{{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Wowchemy's [*Slides*](https://wowchemy.com/docs/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://wowchemy.com/docs/writing-markdown-latex/).

Further event details, including [page elements](https://wowchemy.com/docs/writing-markdown-latex/) such as image galleries, can be added to the body of this page.
