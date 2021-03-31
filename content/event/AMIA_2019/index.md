---
title: RelEx - A system for clinical relation extraction via Convolutional Neural Network

event: AMIA 2019 Annual Symposium (NLP working group)
event_url: https://www.amia.org/amia2019?gclid=CjwKCAjw6fCCBhBNEiwAem5SO_B1qfERGP_Ql3P2LkoqpSDIvji54SxIOnYf6vn75of3sdAWTcUOtRoC3mQQAvD_BwE

location: Washington, D.C
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: Exploring different approaches for ADE Extraction
abstract: "Relation extraction is a task of natural language processing (NLP) to detect and classify the relation between two entities in a text. 
It plays an important role in various NLP related applications such as clinical trial screening, clinical decision making. 
Due to the exponential growth of text in recent years, automatic  extraction  of  semantic relations from text has received growing attention. 
Relation extraction in the clinical domain is more challenging as clinical records can contain multiple pairs of medical entities in the same sentence. 
Convolutional neural networks (CNNs) have been trending due to its strong learning ability features. The max-pooling method of the CNN models help in extracting the most significant features output from the convolution filter.In previous work, CNN models performed well on clinical relation extraction benchmarks, therefore we decided to evaluate its performance against ADE relation extraction benchmarks. Here we describe our relation extraction system for identifying and classifying relations  from  clinical  text using CNNs.   Our  system  consists  of  two  components - sentence-CNN and segment-CNN. We utilize two different data sets: i2b2/VA 2010 , N2C2 2018. The i2b2 corpus includes problem related attributes andrelations from patient discharge summaries. Analysis of our results show segment-CNN outperforms sentence-CNN and this system can be used to extract and clas-sify ADE relation extraction benchmarks. We plan to investigate further into the multi-class labeling of the sentence-CNN and further improve segment-CNN for relation extraction."


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2019-11-16T10:00:00Z"
date_end: "2019-11-20T11:30:00Z"
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: true

image:
  caption: 'AMIA-2019'
  focal_point: Right

links:
- icon: graduation-cap  # Alternatively, use `google-scholar` icon from `ai` icon pack
  icon_pack: fas
  link: https://scholar.google.com/citations?user=3hGpPSYAAAAJ&hl=en
url_code: ""
url_pdf: "media/AMIA_2019.pdf"
url_slides: ""
url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects:
# - BERT-based approach for Relation Extraction
---

<!-- {{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Wowchemy's [*Slides*](https://wowchemy.com/docs/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://wowchemy.com/docs/writing-markdown-latex/).

Further event details, including [page elements](https://wowchemy.com/docs/writing-markdown-latex/) such as image galleries, can be added to the body of this page. -->
