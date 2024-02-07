---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: portfolio
    id: research
    content:
      title: Research
      filters:
        folders:
          - publication
        exclude_featured: true
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Publications
          tag: Publications
        - name: Preprint
          tag: Preprint
        - name: PhD thesis
          tag: PhD
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: citation
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: notes
    content:
      title: Notes
      filters:
        folders:
          - post
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: markdown
    id: teaching
    content:
      title: Teaching
      text: |-
            My teaching experience:
            - 2021 **Calculus 1, Math 100**, Instructor, *University of Alberta*
            - 2019-2020 **Differential equations (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2019-2020 **Algebra (level L3)**, Teaching Assistant, *Sorbonne Université*
            - 2019-2020 **Arithmetic and algebra (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2017-2018 **Euclidean and Hermitian vector spaces, affine isometries (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2017-2018 **Isometry groups and symmetrical groups (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2017-2018 **Arithmetic and algebra (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2016-2017 **Linear algebra 2, Euclidean vector spaces, affine isometries (level L2)**, Teaching Assistant, *Sorbonne Université*
            - 2016-2017 **Analysis and algebra for science (level L1)**, Teaching Assistant, *Sorbonne Université*
            - 2018–2020 Courses given to students preparing the french Agrégation Externe de Mathématiques (highest teaching competitive exam).
            - 2015–2016 Interrogations (khôlles) given in preparatory classes MPSI in Lycée Louis-le-Grand (Paris).        
  - block: markdown
    id: music
    content:
      title: Music
      text: Out of mathematics I am a pianist as well as a musical critic in classical music for [Bachtrack](https://bachtrack.com/), specialized in piano and chamber music, but also covering orchestra. I wrote numerous reviews of concerts, as well as some interviews of musicians or program of concerts. Here is [my page](https://bachtrack.com/fr_FR/22/270/list-published/20748) on Bachtrack. I was several times part of the Press Jury for the International Competition for Outstanding Piano Amateurs.
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      # Contact (add or remove contact options as necessary)
      email: sgaulhiac@impan.pl
      # phone: 888 888 88 88
      # appointment_url: ""
      address:
        street: 'ul. Sniadeckich 8'
        city: Warsaw
        #region: CA
        postcode: '00-656'
        country: Poland
        country_code: PL
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
