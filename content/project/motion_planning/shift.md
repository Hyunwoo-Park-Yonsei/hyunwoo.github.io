---
title: Avoiding static obstacles
summary: 
tags:
  - Autonomous Driving
date: "2020-11-11T00:00:00Z"

# Optional external URL for project (replaces project detail page).
# external_link: https://example.org

# image:
#   caption: Path Planning
#   focal_point: Smart

# url_video: 'https://www.youtube.com/watch?v=F0yPtwk7-Ww'
---
# Avoiding static obstacles
# Overtaking Parked Cars
# Emergent Collision Avoidance
One of the unresolved challenges for autonomous vehicles is safe navigation among occluded pedestrians and vehicles. Previous approaches included generating phantom vehicles and assessing their risk, but they often made the ego vehicle overly conservative or could not conduct a real-time risk assessment in heavily occluded situations. 

We propose an efficient occlusion-aware risk assessment method using simplified reachability quantification that quantifies the reachability of phantom agents with a simple distribution model on phantom agents' state. Furthermore, we propose a driving strategy for safe and efficient navigation in occluded areas that sets the speed limit of an autonomous vehicle using the risk of phantom agents. 

Simulations were conducted to evaluate the performance of the proposed method in various occlusion scenarios involving other vehicles and obstacles. Compared with the baseline case of no occlusion-aware risk assessment, the proposed method increased the traversal time of an intersection by 1.48 times but decreased the average collision rate and discomfort score by up to 6.14 times and 5.03 times, respectively. The proposed method has shown the state-of-the-art level of time efficiency with constant time complexity and computational time of less than 5 ms.