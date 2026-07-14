---
title: "AIDA: Adaptive Imagination for Domain Adaptation"
summary: Sim-to-real adaptation framework for visual reinforcement learning that uses discriminator-gated imagination and self-consistency to learn from scarce target data.
tags:
  - Other
  - Reinforcement Learning
  - Robotics
date: '2026-06-29T00:00:00Z'

image:
  caption: AIDA overview
  focal_point: Smart

---

### Introduction
- Sim-to-real transfer for visual reinforcement learning is difficult because image observations create state-distribution shift between simulation and target environments.
- Prior domain adaptation methods often require large target datasets or image-based RL training, which is expensive and impractical when real-world data is scarce.
- AIDA targets cross-modality adaptation: a source policy is trained with low-dimensional simulator states, while the target domain provides only image observations and limited pre-collected trajectories.

### Method
- AIDA first trains a state-based policy and dynamics model in the source domain, then freezes them during target-domain adaptation.
- A mapping function projects target image observations into the source state space, with trajectory alignment and reconstruction losses enforcing visual consistency and source-target alignment.
- Adaptive imagination generates policy-conditioned synthetic rollouts from target-inferred states, and a three-way discriminator truncates rollouts when they drift from target-supported regions.
- A self-consistency loss cycles imagined states through state -> image -> state so reliable synthetic transitions provide additional representation-learning signal without extra target interaction.

### Result
- The method was evaluated across five MuJoCo tasks and two Gymnasium-Robotics tasks using only 50 target trajectories per task.
- AIDA achieved the lowest state-mapping RMSE on all seven tasks and the highest return ratio on six of seven tasks among the compared domain-adaptation methods.
- Ablation results showed that adaptive truncation outperformed fixed imagination horizons, confirming that per-state rollout reliability is important under limited target data.
