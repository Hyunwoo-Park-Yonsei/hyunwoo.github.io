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

Traditional trajectory planning methods for autonomous vehicles have several limitations. For example, heuristic and explicit simple rules limit generalizability and hinder complex motions. These limitations can be addressed using reinforcement learning-based trajectory planning. However, reinforcement learning suffers from unstable learning and existing reinforcement learning-based trajectory planning methods do not consider the uncertainties. Thus, this paper, proposes a reinforcement learning-based trajectory planning method for autonomous vehicles. The proposed method includes an iterative reward prediction method that stabilizes the learning process, and an uncertainty propagation method that makes the reinforcement learning agent aware of uncertainties. The proposed method was evaluated using the CARLA simulator. Compared to the baseline methods, the proposed method reduced the collision rate by 60.17%, and increased the average reward by 30.82 times. 
