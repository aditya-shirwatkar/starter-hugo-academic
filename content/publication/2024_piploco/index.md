---
title: 'PIP-Loco: A Proprioceptive Infinite Horizon Planning Framework for Quadrupedal Robot Locomotion'

weight: 10

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Naman Saxena
  - Kishore Chandra
  - Shishir Kolathaya 


# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

show_date: false

# date: '2023-07-01T00:00:00Z'
doi: '10.48550/arXiv.2409.09441'

# Schedule page publish date (NOT publication's date).
publishDate: ''

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

# Publication name and optional abbreviated publication name.
publication: ArXiv Preprint
publication_short: ArXiv Preprint

abstract: 'A core strength of Model Predictive Control (MPC) for quadrupedal locomotion has been its ability to enforce constraints and provide interpretability of the sequence of commands over the horizon. However, despite being able to plan, MPC struggles to scale with task complexity, often failing to achieve robust behavior on rapidly changing surfaces. On the other hand, model-free Reinforcement Learning (RL) methods have outperformed MPC on multiple terrains, showing emergent motions but inherently lack any ability to handle constraints or perform planning. To address these limitations, we propose a framework that integrates proprioceptive planning with RL, allowing for agile and safe locomotion behaviors through the horizon. Inspired by MPC, we incorporate an internal model that includes a velocity estimator and a Dreamer module. During training, the framework learns an expert policy and an internal model that are co-dependent, facilitating exploration for improved locomotion behaviors. During deployment, the Dreamer module solves an infinite-horizon MPC problem, adapting actions and velocity commands to respect the constraints. We validate the robustness of our training framework through ablation studies on internal model components and demonstrate improved robustness to training noise. Finally, we evaluate our approach across multi-terrain scenarios in both simulation and hardware.'

# Summary. An optional shortened abstract.
summary: 'arXiv:2409.09441'

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2409.09441'
url_code: 'https://github.com/StochLab/PIP-Loco'
url_dataset: ''
url_poster: ''
url_project: 'https://stochlab.com/PIP-Loco'
url_slides: ''
url_source: ''
url_video: 'https://youtu.be/_mPUU_fAuQY'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ''
---

<!-- empty -->