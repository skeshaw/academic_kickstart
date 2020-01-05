---
title: Low-resource Neural Machine Translation
summary: NMT with transfer learning and MUSE.
tags:
- Personal
date: "2019-10-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Image by mohamed Hassan from Pixabay
  focal_point: Smart

#links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
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

The developments in Neural Machine Translation community (NMT) have been showing the way for the rest of the researchers in the text generation community since the last 5-6 years, especially after the advent of seq2seq models [[Sutskever et al., 2014](https://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf), [Bahdanau et al., 2014](https://arxiv.org/pdf/1409.0473.pdf)] for translation. While more recent advances made in this field for languages like French (fr) and German (de) have been astonishing, one frequently overlooked fact is the amount of data and resources required for achieving those results.  
Especially when we consider low-resource languages like Basque (eu) and Gujarati (gu), it would be almost impossible to replicate those lofty scores for these languages due to much less amount of freely available data. However, encouraging efforts have been made in this field to make use of transfer learning [[Zoph et al., 2016](https://www.aclweb.org/anthology/D16-1163.pdf)], whereby a parent model (say, de-en) over much larger dataset is used to provide a good initial point for translation in a low-resource setting (gu-en).  
As a part of this project, I implemented an ACL 2019 paper [[Kim et al., 2019](https://www.aclweb.org/anthology/P19-1120.pdf)] on transfer learning in NMT which also uses cross-lingual maps [[Conneau et al., 2018](https://arxiv.org/pdf/1710.04087.pdf)] to learn, without any need for shared vocabularies between source and target languages. Due to limitations on available resources, I was only able to replicate the general trend of results, as reported in the paper, for Basque-English and extend the framework to Gujarati-English.
