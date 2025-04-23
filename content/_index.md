---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: Lecturer
          company: Universitat Oberta de Catalunya
          company_url: 'www.uoc.edu'
          location: Barcelona
          date_start: '2021-03-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Teaching: Psychometrics, Introduction to Research in Psychology, Multivariate Data Analysis
              * Research
        - title: Adjunct lecturer
          company: Universitat Autònoma de Barcelona
          company_url: ''
          location: Barcelona
          date_start: '2017-09-01'
          date_end: ''
          description: Teaching methods in Psychology.
        - title: Freelance
          company: 
          company_url: ''
          location: Barcelona
          date_start: '2018-09-01'
          date_end: '2021-03-01'
          description: Psychometrics and statistics.
    design:
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project

      default_button_index: 0

      buttons:
        - name: MISS
          tag: miss
        - name: DigitAsia
          tag: digitasia
        - name: Screens
          tag: Screens
        - name: LaCaixa Foundation
          tag: LaCaixa
        - name: REVISEapp
          tag: REVISEapp
        - name: Personal projects
          tag: Personal projects
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: collection
    id: publi
    content:
      title: Recent Publications and Conferences
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-

      # 
      email: ariadna.angulo.brunet@gmail.com

      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/AnguloBrunet'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---


[congres]: ./congres/