---
title: Safe and efficient trajectory optimization for autonomous vehicles using b-spline with incremental path flattening.
summary: published in T-ITS in Dec 2024
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
# Introduction
# Method
# Result

B-spline-based trajectory optimization is widely used for robot navigation due to its computational efficiency and convex-hull property (ensures dynamic feasibility), especially as quadrotors, which have circular body shapes (enable efficient movement) and freedom to move each axis (enables convex-hull property utilization). However, using the B-spline curve for trajectory optimization is challenging for autonomous vehicles (AVs) because of their vehicle kinodynamics (rectangular body shapes and constraints to move each axis). 

In this study, we propose a novel trajectory optimization approach for AVs to circumvent this difficulty using an incremental path flattening (IPF), a disc type swept volume (SV) estimation method, and kinodynamic feasibility constraints. IPF is a new method that can find a collision-free path for AVs by flattening path and reducing SV using iteratively increasing curvature penalty around vehicle collision points. Additionally, we develop a disc type SV estimation method to reduce SV over-approximation and enable AVs to pass through a narrow corridor efficiently. Furthermore, a clamped B-spline curvature constraint, which simplifies a B-spline curvature constraint, is added to dynamical feasibility constraints (e.g., velocity and acceleration) for obtaining the kinodynamic feasibility constraints. 

Our experimental results demonstrate that our method outperforms state-of-the-art baselines in various simulated environments. We also conducted a real-world experiment using an AV, and our results validate the simulated tracking performance of the proposed approach.

