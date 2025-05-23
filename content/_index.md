---
# Leave the homepage title empty to use the site title
title: "Ole Kristian Dyskeland"
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: 
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: nhh_varde-solutions7231.jpg
          filters:
            brightness: 0.2
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I do research on competition between digital platforms, and focus primarily on media markets. I study how the platforms' competition for consumers influence their relationship with content providers. 

    design:
      columns: '1'
  - block: collection
    id: workingpapers
    content:
      title: Working Papers
      text: ""
      filters:
        folders:
          - wp
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: workinprogress
    content:
      title: Work in Progress
      text: ""
      filters:
        folders:
          - wip
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: publications
    content:
      title: Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Presentations
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News and Media
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: article-grid
      columns: 1
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

---
