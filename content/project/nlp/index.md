---
title: Query-based Summarized Email Extraction
summary: Extractive summaries over Enron email dataset.
tags:
- Course
date: "2016-11-20T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Image by Bualong from Adobe Stock
#  focal_point: Smart

url_code: ""
url_pdf: "https://github.com/skeshaw/project_reports/blob/master/courses/CS671A_report.pdf"
url_slides: ""
url_video: ""

---

As the amount of available data around us explodes, it becomes important to be able to present the same in a concise manner. One possible use case could be searching through one's emails for getting a brief summary of threads related to some search terms.  
Through this project, we build a model which returns extractive summaries of emails given a search query. We start by identifying threads which have terms matching with those in the query. This step is followed by clustering the relevant emails, and finally generating brief outputs containing the most significant information for each cluster.
