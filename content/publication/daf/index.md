---
title: 'Everything is a Transaction: Unifying Logical Concurrency Control and Physical Data Structure Maintenance in Database Management Systems'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Matthew Butrovich
  - Tianyu Li
  - Yash Nannapanei
  - Andrew Pavlo
  - John Rollinson
  - Huanchen Zhang
  - Ambarish Balakumar
  - Daniel Biales
  - Ziqi Dong
  - Emmanuel Eppinger
  - Jordi Gonzalez
  - Wan Shen Lim
  - Jianqiao Liu
  - Lin Ma
  - Prashanth Menon
  - Soumil Mukherjee
  - Tanuj Nayak
  - Amadou Ngom
  - Jeff Niu
  - Deepayan Patra
  - Poojita Raj
  - Stephanie Wang
  - Wuwen Wang
  - Yao Yu
  - William Zhang

date: '2020-12-16T00:00:00Z'
# doi: '10.1145/3589297'

# # Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *Conference on Innovative Data Systems Research* 2023
publication_short: In *CIDR* 2021

abstract: Almost every database management system (DBMS) supporting transactions created in the last decade implements multi-version concurrency control (MVCC). But these systems rely on physical data structures (e.g., B+trees, hash tables) that do not natively support multi-versioning. As a result, there is a disconnect between the logical semantics of transactions and the DBMS’s underlying implementation. System developers must invest in engineering efforts to coordinate transactional access to these data structures and non-transactional maintenance tasks. This burden leads to challenges when reasoning about the system’s correctness and performance and inhibits its modularity. In this paper, we propose the Deferred Action Framework (DAF), a new system architecture for scheduling maintenance tasks in an MVCC DBMS integrated with the system’s transactional semantics. DAF allows the system to register arbitrary actions and then defer their processing until they are deemed safe by transactional processing. We show that DAF can support garbage collection and index cleaning without compromising performance while facilitating higher-level implementation goals, such as non-blocking schema changes and self-driving optimizations.


tags: [resource management, adaptive query processing, structured text search, database query processing]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

url_pdf: 'publication/daf/deferred-action.pdf'
url_code: 'https://github.com/mush-zhang/terrier/tree/deferred-action-ling'
url_video: 'https://www.youtube.com/watch?v=vZX4f9rT694'

# # Associated Projects (optional).
# #   Associate this publication with one or more of your projects.
# #   Simply enter your project's folder or file name without extension.
# #   E.g. `internal-project` references `content/project/internal-project/index.md`.
# #   Otherwise, set `projects: []`.
# projects:
#   - example

# # Slides (optional).
# #   Associate this publication with Markdown slides.
# #   Simply enter your slide deck's filename without extension.
# #   E.g. `slides: "example"` references `content/slides/example/index.md`.
# #   Otherwise, set `slides: ""`.
# slides: example
---
