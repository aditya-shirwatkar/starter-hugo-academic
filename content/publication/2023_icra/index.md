---
title: 'Force control for Robust Quadruped Locomotion: A Linear Policy Approach'

weight: 10

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Vamshi Kumar Kurva
  - Devaraju Vinoda
  - Aman Singh
  - Aditya Sagi
  - Himanshu Lodha
  - Bhavya Giri Goswami
  - Shivam Sood
  - Ketan Nehete
  - Shishir Kolathaya


# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

show_date: false

# date: '2023-07-01T00:00:00Z'
doi: 'https://doi.org/10.1109/ICRA48891.2023.10161080'

# Schedule page publish date (NOT publication's date).
publishDate: ''

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: 2023 IEEE International Conference on Robotics and Automation (ICRA)
publication_short: ICRA 2023

abstract: 'This work presents a simple linear policy for direct force control for quadrupedal robot locomotion. The motivation is  that  force  control  is  essential  for  highly  dynamic  and  agile motions. We learn a linear policy to generate end-foot trajectory parameters and a centroidal wrench, which is then distributed among  the  legs  based  on  the  foot  contact  information  using  a quadratic  program  (QP)  to  get  the  desired  ground  reaction forces.  Unlike  the  majority  of  the  existing  works  that  use complex nonlinear function approximators to represent the RL policy  or  model  predictive  control  (MPC)  methods  with  many optimization  variables  in  the  order  of  hundred,  our  controller uses a simple linear function approximator to represent policy along with only a twelve variable QP for the force distribution. A centroidal dynamics-based MPC method is used to generate reference trajectory data, and then the linear policy is trained using  imitation  learning  to  minimize  the  deviations  from  the reference   trajectory.   We   demonstrate   this   compute-efficient controller  on  our  robot  Stoch3  in  simulation  and  real-world experiments on indoor and outdoor terrains with push recovery.'

# Summary. An optional shortened abstract.
summary: '*2023 IEEE International Conference on Robotics and Automation (ICRA), London*'

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://www.stochlab.com/papers/force_lp_ICRA_2023.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://youtu.be/k89QdImcqdo'

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