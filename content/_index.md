---
# Leave the homepage title empty to use the site title
title: Ling Zhang
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  - block: collection
    id: publication
    content:
      title: Publications
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: citation
---
