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
  url: https://arxiv.org/abs/2404.12079v4
url_pdf: 'https://arxiv.org/pdf/2404.12079v4.pdf'
#url_slides: ''
url_video: 'https://www.youtube.com/watch?v=PfDbaeLfcN4'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
### 🧾 Introduction
- Traditional trajectory planning for autonomous vehicles often relies on heuristics or simple rules, which limit generalization and complex behavior handling.
- Reinforcement learning (RL) has the potential to overcome these limitations, but suffers from instability and often ignores uncertainty during planning.
- This work addresses both issues by proposing an uncertainty-aware RL-based trajectory planner.
### ⚙️ Method
- The proposed method uses an iterative reward prediction framework, which forecasts expected future states and incorporates them into the learning process to improve training stability.
- Additionally, it applies uncertainty propagation techniques to make the agent aware of environmental and model uncertainties during trajectory planning.
- This dual approach improves both the robustness and adaptability of the RL agent.
### ✅ Result
- The method was evaluated in the CARLA simulator and compared with baseline RL planners.
- It reduced the collision rate by 60.17% and increased the average reward by 30.82×, demonstrating significant improvements in both safety and performance.

