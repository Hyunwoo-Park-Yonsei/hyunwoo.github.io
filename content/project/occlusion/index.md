---
title: Occlusion-aware Risk Assessment and Driving Strategy for Autonomous Vehicles Using Simplified Reachability Quantification
summary: published in RA-L in Nov 2023
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

One of the unresolved challenges for autonomous vehicles is safe navigation among occluded pedestrians and vehicles. Previous approaches included generating phantom vehicles and assessing their risk, but they often made the ego vehicle overly conservative or could not conduct a real-time risk assessment in heavily occluded situations. 

We propose an efficient occlusion-aware risk assessment method using simplified reachability quantification that quantifies the reachability of phantom agents with a simple distribution model on phantom agents' state. Furthermore, we propose a driving strategy for safe and efficient navigation in occluded areas that sets the speed limit of an autonomous vehicle using the risk of phantom agents. 

Simulations were conducted to evaluate the performance of the proposed method in various occlusion scenarios involving other vehicles and obstacles. Compared with the baseline case of no occlusion-aware risk assessment, the proposed method increased the traversal time of an intersection by 1.48 times but decreased the average collision rate and discomfort score by up to 6.14 times and 5.03 times, respectively. The proposed method has shown the state-of-the-art level of time efficiency with constant time complexity and computational time of less than 5 ms.