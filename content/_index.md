---
title: ''
summary: Academic website of Yu Zhu
type: landing
aliases:
  - /about/
  - /about.html

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/cv.pdf
      headings:
        about: About
        education: Education
        interests: Research Interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: Research
      subtitle: ''
      text: |-
        My research connects physical modeling with modern machine learning.
        I develop physics-driven methods for reconstructing molecular-orbital
        information from scanning tunneling microscopy images, and I work on
        machine learning force fields and scalable materials-modeling workflows.

        I am also interested in open-set fine-grained recognition, where models
        must recognize known categories while detecting previously unseen ones.
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: citation

  - block: collection
    content:
      title: Recent Publications
      filters:
        folders:
          - publications
        exclude_featured: true
    design:
      view: citation

  - block: collection
    id: projects
    content:
      title: Research Projects
      filters:
        folders:
          - projects
      count: 4
    design:
      view: article-grid
      fill_image: false
      columns: 2
      show_date: false
      show_read_time: false
      show_read_more: true
---
