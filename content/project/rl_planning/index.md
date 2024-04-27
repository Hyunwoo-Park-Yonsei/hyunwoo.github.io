---
title: Trajectory Planning for Autonomous Vehicle Using Iterative Reward Prediction in Reinforcement Learning
summary: published in arXiv in April 2024
tags:
  - Autonomous Driving
date: '2024-04-22T00:00:00Z'

# Optional external URL for project (replaces project detail page).
# external_link: ''

image:
  caption: Trajectory Planning Using Reinforcement Learning
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
#url_code: ''
links:
- name: arXiv
  url: https://arxiv.org/abs/2404.12079
url_pdf: 'https://arxiv.org/pdf/2404.12079.pdf'
#url_slides: ''
url_video: 'https://www.youtube.com/watch?v=PfDbaeLfcN4'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

Traditional trajectory planning methods for autonomous vehicles have several limitations. Heuristic and explicit simple rules make trajectory lack generality and complex motion. One of the approaches to resolve the above limitations of traditional trajectory planning methods is trajectory planning using reinforcement learning. However, reinforcement learning suffers from instability of learning and prior works of trajectory planning using reinforcement learning didn’t consider the uncertainties. In this paper, we propose a trajectory planning method for autonomous vehicles using reinforcement learning. The proposed method includes iterative reward prediction method that stabilizes the learning process, and uncertainty propagation method that makes the reinforcement learning agent to be aware of the uncertainties. The proposed method is experimented in the CARLA simulator. Compared to the baseline method, we have reduced the collision rate by 60.17%, and increased the average reward to 30.82 times.
