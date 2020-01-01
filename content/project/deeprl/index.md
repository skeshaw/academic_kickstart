---
title: Transfer Learning in Deep RL
summary: Evaluate using policies learned from harder tasks.
tags:
- Course
date: "2019-11-21T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

#image:
#  caption: Photo by rawpixel on Unsplash
#  focal_point: Smart

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

---

The general idea of transfer learning is to reuse learnings or experiences from related tasks to obtain a _jumpstart_ on the task of interest. A lot of work in this paradigm in RL is centered around learning from _easier_ but related tasks to generalize to a desired, _harder_ task.  
A recently published work on Challenge Learning [[Jason Ma, 2019](https://drive.google.com/file/d/13lT4li8V0KKS0wqrn3Y047JiMEHCZAjF/view)] explores the other direction of transfer. It proposes learning policies on a harder version of an environment and evaluating the same on an easier one by controlling a single environment variable. The paper, however, only demonstrates experimental results on CartPole using an Advantage Actor Critic (A2C) [[Mnih et al., 2016](https://arxiv.org/pdf/1602.01783.pdf)] architecture.  
We add evaluations of the environment on an actor-critic architecture using Proximal Policy Optimization (PPO) [[Schulman et al., 2017](https://arxiv.org/pdf/1707.06347.pdf)] as the actor, which is shown to be much more robust to changes in the environment. We also control for an extra affecting variable, the magnitude of the horizontal force applied on the cart (a constant).
