---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: rounded # Options: circle (default), square, rounded
      spacing:
        padding: [2rem, 0, 0, 0]
  - block: collection
    id: papers
    content:
      title: Research
      filters:
        folders:
          - publications
        featured_only: false
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Media
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
