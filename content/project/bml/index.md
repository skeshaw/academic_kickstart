---
title: Stochastic Variational Inference
summary: Poisson Matrix Factorization with stochastic updates.
tags:
- Course
date: "2017-04-20T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: <a href=http://hameddaily.blogspot.com/2016/12/simple-matrix-factorization-with.html>Image source</a>
#  focal_point: Smart

url_code: "https://github.com/ankuPRK/BML_HPF/tree/sandipan2"
url_pdf: "https://github.com/skeshaw/project_reports/blob/master/courses/CS698S_report.pdf"
url_slides: ""
url_video: ""

---

One of the central tasks in Bayesian Machine Learning is to compute the posterior distribution given data and prior. One of the popular techniques is Variational Inference. However, in its batch setting, it is often not scalable to large datasets. Fortunately, it can be done in a stochastic setting as well.  
As a part of the project, we did a literature survey of Stochastic Variational Inference (SVI) methods. We also formulated and implemented an SVI version of Hierarchical Poisson Matrix Factorization [[Gopalan et al., 2015](http://jakehofman.com/inprint/poisson_recs.pdf)], while the paper only had batch VB (Variational Bayes) updates.
