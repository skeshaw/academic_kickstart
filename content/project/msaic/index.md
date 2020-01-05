---
title: Microsoft AI Challenge
summary: Answer selection given a search query.
tags:
- Personal
date: "2018-12-28T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Image by intheskies from Adobe Stock
#  focal_point: Smart

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---

[Competition homepage](https://www.facebook.com/msaichallenge/)

Ranking passages in response to search queries on the web is a crucial task. To promote work in this area, Microsoft India organized the Microsoft AI Challenge in 2018. The task consisted of appropriately ranking ten answers for each given query and maximizing the mean reciprocal rank (MRR) over a given test set.  
We began by working with popular models like bi-LSTM and Doc2Vec. After getting a good understanding of the data and exploring the relevant literature, we turned to using more advanced models like [HYPERQA](https://arxiv.org/pdf/1707.07847.pdf) and bilateral multi-perspective matching for natural language sentences ([BiMPM](https://arxiv.org/pdf/1702.03814.pdf)).  
Through our extensive experimentation, we were able to achieve results that led us to an expected final rank under 40 (out of 280 teams in the second stage and 1800 overall).
