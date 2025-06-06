---
title: Occlusion-aware Risk Assessment and Driving Strategy for Autonomous Vehicles Using Simplified Reachability Quantification
summary: Published in RA-L in Nov 2023. Trajectory planning method for autonomous vehicle under occluded area. 
tags:
  - Autonomous Driving
date: '2023-11-02T00:00:00Z'

# Optional external URL for project (replaces project detail page).
# external_link: ''

image:
  caption: Occlusion-aware Risk Assessment
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
#url_code: ''
links:
- name: RA-L
  url: https://ieeexplore.ieee.org/abstract/document/10305287
url_pdf: 'https://arxiv.org/pdf/2306.07004.pdf'
#url_slides: ''
url_video: 'https://youtu.be/TJo2pfhkxw4'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
### 🧾 Introduction
- One of the key challenges in autonomous driving is safely navigating areas with occluded pedestrians and vehicles.
- Prior methods used phantom vehicle generation to estimate risk but were often overly conservative or ineffective in real time under heavy occlusion.
- To address this, we propose an efficient occlusion-aware risk assessment framework and a risk-adaptive speed control strategy.
### ⚙️ Method
- The proposed method models phantom agents in occluded regions using a simplified probabilistic reachability distribution.
- Based on the quantified risk of phantom agents, the system dynamically sets speed limits to enable safe yet efficient navigation.
- The approach maintains constant-time complexity and is computationally efficient, requiring less than 5 ms per decision.
### ✅ Result
- Simulation results show the proposed method increased intersection traversal time by 1.48×,
but reduced average collision rate and discomfort score by 6.14× and 5.03×, respectively.
- The method achieves state-of-the-art time efficiency while significantly improving safety and ride comfort in occluded scenarios.
