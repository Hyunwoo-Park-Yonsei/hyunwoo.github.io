---
title: An open-space planner.
summary: Reference Planner for unstructured environments.
tags:
  - Autonomous Driving
date: '2022-08-29T00:00:00Z'

# Optional external URL for project (replaces project detail page).
# external_link: ''

image:
  caption: Open-space planner
  focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
#url_code: ''
# url_pdf: 'https://arxiv.org/pdf/2311.02957.pdf'
#url_slides: ''
url_video: 'https://youtu.be/ZvOuJ3Kb-jg' 

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---
![alt](osp.gif)
[Watch Full Video](https://www.youtube.com/watch?v=m6aqP3xJUOE)
### 🧾 Introduction
- The Open Space Planner (OSP) module was developed for autonomous path planning in unstructured environments such as parking lots or areas without lane markings.
- It is based on the method proposed in ["Autonomous Driving Trajectory Optimization With Dual-Loop Iterative Anchoring Path Smoothing and Piecewise-Jerk Speed Optimization"](https://ieeexplore.ieee.org/abstract/document/9300224).
- The OSP was tested in both the CARLA simulator and real-world vehicle experiments.
### ⚙️ Method
- Hybrid A* was used to generate an initial feasible path considering vehicle kinematics.
- The path was then optimized using Sequential Quadratic Programming (SQP) to minimize jerk and acceleration, resulting in a smooth and dynamically feasible path.
- To ensure probabilistic completeness, a kinodynamic informed RRT* was implemented as a backup planner.
### ✅ Result
- The OSP module successfully generated collision-free, smooth, and dynamically feasible path in both simulation and real-world settings.
- The hybrid planning structure allowed robust handling of complex environments, with RRT* ensuring fallback coverage when optimization failed.
- The resulting path demonstrated low jerk and acceleration profiles, enhancing ride comfort and vehicle control performance.