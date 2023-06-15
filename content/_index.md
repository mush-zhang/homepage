---
# Leave the homepage title empty to use the site title
title: Ling Zhang
type: landing
sections:
  # - block: hero
  #   content:
  #     text: |-
  #      <br/><br/><br/><br/>
  #   design:
  #     columns: '1'
  #     background:
  #       image:
  #         # Name of image in `assets/media/`.
  #         filename: header.jpg
  #         filters:
  #           brightness: 1
  #         #  Image fit. Options are `cover` (default), `contain`, or `actual` size.
  #         size: actual
  #         position: center
  #         parallax: true
  #         text_color_light: true
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
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

<!-- header:
  image: "/headers/bubbles-wide.jpg"
  caption: "Yay! It works!" -->