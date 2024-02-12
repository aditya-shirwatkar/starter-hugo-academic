---
title: ODE Analysis of Gradient based Unconstrained Optimization Algorithms
summary: Course Project for DS 211 - Numerical Optimization
tags:
  - Course Project
show_date: false
weight: -2
# Optional external URL for project (replaces project detail page).
external_link: ''

math: true

# image:
#   caption: Photo by rawpixel on Unsplash
#   focal_point: Smart

# links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
url_code: ''
url_pdf: 'project/num_opt/main.pdf'
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

This work focuses on analyzing well-established gradient-based unconstrained optimization algorithms like Gradient Descent (GD), Mirror Descent (MD), Nesterov’s Accelerated Gradient Descent (NAGD) and Newton's Method (NM). To achieve this, we derive the continuous-time ordinary differential equations (ODEs) of these algorithms, by comparing their iterative update rule to a discretized version of the corresponding ODE. We then construct Lyapunov functions to investigate the convergence and stability properties of the equilibrium points of the ODE (which correspond to stationary points or local minima of the objective function). Additionally, we consider some special cases for which the rate of convergence for all of them can be shown as $\mathcal{O}(1/t^p)$, where $p \in \mathbb{R_+}$. Lastly, we propose a new Lyapunov function for the ODE corresponding to Newton's method and provide a new simple proof for its convergence rate.
