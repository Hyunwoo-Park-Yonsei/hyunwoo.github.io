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
### 🧾 Introduction
- B-spline-based trajectory optimization is effective in robotics due to its computational efficiency and convex-hull property, especially for quadrotors.
- However, applying B-splines to autonomous vehicles (AVs) is challenging due to rectangular body shapes and kinodynamic constraints.
- This study proposes a novel approach that overcomes these challenges for AV trajectory optimization.
### ⚙️ Method
- The proposed method integrates three components: Incremental Path Flattening (IPF), a disc-type swept volume (SV) estimation, and kinodynamic feasibility constraints.
- IPF flattens paths by increasing curvature penalties around collision areas, enabling collision-free path shaping.
- A disc-type SV model reduces over-approximation and allows efficient navigation in narrow spaces.
Clamped B-spline curvature constraints are introduced to ensure kinodynamic feasibility, including limits on velocity and acceleration.
### ✅ Result
- In simulation, the proposed method outperformed state-of-the-art baselines in path safety and efficiency.
- Real-world experiments with an AV confirmed that the method’s tracking performance aligned with simulation results.
- The approach proved effective in handling both collision avoidance and dynamic feasibility in constrained driving environments.
