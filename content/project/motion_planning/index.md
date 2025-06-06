---
title: Motion Planner for Public Roads and Airport Apron
summary: Avoiding static obstacles, Overtaking Parked Cars, and Emergent Collision Avoidance
tags:
  - Autonomous Driving
date: "2019-11-11T00:00:00Z"

# Optional external URL for project (replaces project detail page).
# external_link: https://example.org

image:
  caption: Path Planning
  focal_point: Smart

url_video: 'https://www.youtube.com/watch?v=F0yPtwk7-Ww'

---
# Avoiding static obstacles
![alt](shift.gif)
### 🧾 Introduction
- In autonomous driving systems, it is essential to implement avoidance behavior for static obstacles.
- Static obstacles refer to non-moving objects such as parked vehicles, median strips, and traffic cones.
- To ensure safety under perception and localization uncertainties, the system was designed to avoid unnecessary reactions while maintaining stable and safe behavior, thereby reducing potential discomfort or risk for passengers.
### ⚙️ Method
- To generate avoidance paths, we used a quintic polynomial to create a jerk-minimized trajectory.
- To compensate for uncertainties in localization and object detection, we adopted a strategy that alternates between conservative and sensitive decision modes depending on the situation.
### ✅ Result
- As a result, the system successfully generated stable avoidance trajectories in the presence of various static obstacles.
- Even under sensor uncertainty, the vehicle demonstrated robust and safe behavior during navigation.
- This decision strategy balances caution and responsiveness, allowing the system to remain safely proactive without frequent shifts in behavior, which in turn helps maintain ride comfort and operational stability.
# Overtaking Parked Cars
![alt](detour.gif)
### 🧾 Introduction
- This task addresses the need for overtaking parked vehicles or static objects that are illegally stopped or obstructing the lane.
- Unlike static obstacle avoidance, this task requires crossing lane boundaries, which introduces additional risk from vehicles approaching from the adjacent lane.
- The goal is to enable safe and smooth overtaking behavior in environments with irregularly parked vehicles or objects.
### ⚙️ Method
- A classification algorithm was developed to accurately distinguish between regular moving or temporarily stopped vehicles and those that require overtaking.
- Using this algorithm, the system determines whether ovetaking is necessary for obstacle avoidance.
- The jerk-minimized trajectory, generated using a quintic polynomial, was evaluated to determine whether the planned lane departure and reentry would be safe.
- The system continuously monitors the adjacent lane for approaching vehicles in order to plan a safe overtaking decision.
### ✅ Result
- The system was able to successfully identify and overtake parked vehicles and roadside obstacles.
- It demonstrated the ability to safely merge into and return from adjacent lanes while avoiding conflicts with moving traffic.
- This resulted in robust and stable overtaking behavior, even in complex urban driving scenarios.
# Emergent Collision Avoidance
### 🧾 Introduction

- The Emergent Collision Avoidance (ECA) module is an independent safety mechanism designed to operate when primary autonomous driving modules malfunction or behave abnormally.
- To ensure reliability in emergency scenarios, the ECA minimizes interactions with other modules, operating with autonomous logic when safety thresholds are breached.

### ⚙️ Method
- The ECA is based on Mobileye's Responsibility-Sensitive Safety (RSS) framework, which defines provable longitudinal and lateral safety distances.
- It activates only when critical violations of these safety distances occur, prioritizing emergency responsiveness over system coordination.
- Upon detecting a violation, the ECA computes control commands that satisfy the RSS constraints and applies them to override the nominal system.


### ✅ Result

- The ECA successfully overrode unsafe commands and performed emergency maneuvers such as overtaking when required.
- Its independence allowed it to maintain safety even in cases of system malfunction or planning failure.