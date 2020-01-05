---
title: Fine-grained Vehicle Classification
summary: Real time object classification in video.
tags:
- Course
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart

url_code: ""
url_pdf: "https://github.com/skeshaw/project_reports/blob/master/courses/CS771A_report.pdf"
url_slides: ""
url_video: ""

---

Through this project, we built a model which learned to detect and classify moving objects in videos. A classifier learned to distinguish between pedestrians and vehicles, as well as predicting fine-grained results for vehicles like 2-wheelers, 4-wheelers, etc.  
First, the classifier learned to distinguish between different object classes. We employed Histogram of Gradients (HOG) [[N. Dalal and B. Triggs](https://lear.inrialpes.fr/people/triggs/pubs/Dalal-cvpr05.pdf)] and Scale-Invariant Feature Transform (SIFT) [[David G. Lowe](https://www.cs.ubc.ca/~lowe/papers/ijcv04.pdf)] for building image features. Subsequently, we used the learned classifier with a sliding window approach over video frames to localize and identify objects.  
An issue which we encountered while running our model over video frames was the prediction of many false positives (a window containing no object identified as having one). To address this, we turned to the approach of [hard negative mining](https://www.reddit.com/r/computervision/comments/2ggc5l/what_is_hard_negative_mining_and_how_is_it/). Here, we saved a wrongly classified empty window as background and forced the classifier to learn it as a separate class. This led to a significant reduction in the false positive rate. 
