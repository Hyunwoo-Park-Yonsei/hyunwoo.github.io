---
title: Safe and efficient trajectory optimization for autonomous vehicles using b-spline with incremental path flattening.
summary: published in arXiv (submitted in T-ITS) in Nov 2023
tags:
  - Autonomous Driving
date: '2023-11-29T00:00:00Z'

# Optional external URL for project (replaces project detail page).
# external_link: ''

image:
  caption: Trajectory Optimization
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
#url_code: ''
links:
- name: arXiv
  url: https://arxiv.org/abs/2311.02957
url_pdf: 'https://arxiv.org/pdf/2311.02957.pdf'
#url_slides: ''
url_video: 'https://youtu.be/7bhxfuhAqos'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

Traditional trajectory planning methods for au- tonomous vehicles have several limitations. Heuristic and ex- plicit simple rules make trajectory lack generality and complex motion. One of the approaches to resolve the above limita- tions of traditional trajectory planning methods is trajectory planning using reinforcement learning. However, reinforcement learning suffers from instability of learning and prior works of trajectory planning using reinforcement learning didn’t consider the uncertainties. In this paper, we propose a trajectory planning method for autonomous vehicles using reinforce- ment learning. The proposed method includes iterative reward prediction method that stabilizes the learning process, and uncertainty propagation method that makes the reinforcement learning agent to be aware of the uncertainties. The proposed method is experimented in the CARLA simulator. Compared to the baseline method, we have reduced the collision rate by 60.17%, and increased the average reward to 30.82 times.

