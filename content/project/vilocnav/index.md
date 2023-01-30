---
title: 'ViLocNav: Visual Learning-based Optimal Control and Navigation'
summary: Course Project for MEL457 Artificial Intelligence for Engineer by Dr. Trushar B Gohil at VNIT
tags:
  - Course Project
show_date: false
weight: 2
# Optional external URL for project (replaces project detail page).
external_link: ''

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: 'https://docs.google.com/presentation/d/e/2PACX-1vS1-Xj0hpVnTqkFEI0lSEc-nSpX8KvdLqWTSJlY_unEcoZ7EPbdGNQy0mwndiH62g/pub?start=false&loop=true&delayms=3000'
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Model-based control methods like MPC and iLQG are a popular paradigm for autonomous robot navigation because they can efficiently plan robust robot motion trajectories by leveraging a known deterministic or stochastic dynamics model. However, using model-based methods in situations where the environment is a priori unknown and can only be observed partially through onboard sensors on the robot is challenging, and requires mapping and localization of the robot w.r.t to the unknown environment.

Mapping can be used to estimate the 3D structure of the environment (using RGB / RGB-D images / LiDAR scans), which is used by a planner to compute paths to a goal. Although such purely geometric intermediate representations do not capture navigational affordances (such as: to go far away, one should step into a hallway, etc.). Furthermore, mapping is challenging with just RGB observations, and often unreliable even with active depth sensors (such as in presence of shiny or thin objects, or presence of strong ambient light). End-to-end learning methods which do not rely on any model-based setting are used to sidestep this explicit map estimation step and have also been studied by some researchers. However, such approaches have proven to extremely sample inefficient and highly specific to the system they were trained on. Plus the control outputs from the pipeline are jittery and often not optimal, which increases the difficulty of deployment in real-world scenarios.

In our project, we will try to improve on this shortcoming by combining deep learning and model-based control. Our pipeline will consist of a learning-based perception module along with optimal control for autonomous driving. A series of waypoints are produced by the learning-based perception module that guides the robot to the goal via avoiding obstacles. This approach is highly based on the paper “Combining Optimal Control and Learning for Visual Navigation in Novel Environments”. A model-based planner uses these waypoints to generate a smooth and dynamically feasible trajectory, which is then executed on the physical system using feedback control