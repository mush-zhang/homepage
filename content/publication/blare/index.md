---
title: 'Exploiting Structure in Regular Expression Queries'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Shaleen Deep
  - Avrilia Floratou
  - Anja Gruenheid
  - Jignesh M. Patel
  - Yiwen Zhu

date: '2023-02-01T00:00:00Z'
doi: '10.1145/3589297'

# # Schedule page publish date (NOT publication's date).
# publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *ACM SIGMOD Conference* 2023
publication_short: In *SIGMOD* 2023

abstract: Regular expression, or regex, is widely used to extract critical information from a large corpus of formatted text by finding patterns of interest. In tasks like log processing, the speed of regex matching is crucial. Data scientists and developers regularly use regex libraries that implement optimized regular expression matching using modern automata theory. However, computing state transitions in the underlying regex evaluation engine can be inefficient when a regex query contains a multitude of string literals. This inefficiency is further exasperated when analyzing large data volumes. This paper presents BLARE, Blazingly Fast Regular Expression, a regular expression matching framework that is inspired by the mechanisms that are used in database engines, which use a declarative framework to explore multiple equivalent execution plans, all of which produce the correct final result. Similarly, BLARE decomposes a regex into multiple regex and string components and then creates evaluation strategies in which the components can be evaluated in an order that is not strictly a left-to-right translation of the input regex query. Rather than using a cost-based optimization approach, BLARE uses an adaptive runtime strategy based on a multi-armed bandit approach to find an efficient execution plan. BLARE is also modular and can be built on top of any existing regex library. We implemented BLARE on four commonly used regex libraries, RE2, PCRE2, Boost Regex, and ICU Regex, and evaluated it using two production workloads and one open-source workload. BLARE was 1.6x to 3.7x faster than RE2 and 3.4x to 7.9x faster than Boost Regex. PCRE2 did not finish on one of the workloads, but on the remaining two workloads, BLARE improved the performance of PCRE2 by 3.1x to over 100x. For the open-source dataset, BLARE provided a speed up of 61.7x for ICU Regex. BLARE code is publicly available at https://github.com/mush-zhang/Blare.

tags: [regular expression, adaptive query processing, structured text search, database query processing]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
# url_project: ''
# url_source: ''
# url_video: ''

url_pdf: 'publication/blare/BLARE.pdf'
url_code: 'https://github.com/mush-zhang/Blare'
url_poster: 'publication/blare/Ling_blare_poster.png'
url_slides: 'publication/blare/blare_new_slides.pdf'

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
