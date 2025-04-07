---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Graduate Research Assistant
    company: University of Washington
    company_url: 'https://www.allofus.nih.gov/funding-and-program-partners/center-for-linkage-and-aquisition-of-data'
    company_logo:
    location: Seattle, WA, USA
    date_start: '2023-09-16'
    date_end: ''
    description: |2-
      * Designed and implemented a scalable pipeline in Palantir Foundry, enabling efficient processing of 600,000+ US residential addresses for health data standardization from the *All of Us* dataset
      * Adhered to OMOP Common Data Model to ensure cross-study consistency and data compatibility, contributing to dataset interoperability
      * Generated a benchmark dataset from Homeland Infrastructure Foundation-Level Data, facilitating comparative analysis
      * Conducted comprehensive literature reviews on geocoding techniques and standards, providing actionable insights for improved algorithm selection and data linkage

  - title: National Library of Medicine Biomedical Informatics & Data Science Pre-Doctoral Fellow
    company: University of Washington
    company_url: 'http://bime.uw.edu/'
    company_logo:
    location: Seattle, WA, USA
    date_start: '2020-09-16'
    date_end: '2023-09-15'
    description: |2-
      * Developed multimodal models leveraging structured clinical data (EHR/EMR), unstructured documentation, and imaging analysis to predict vertebral compression fractures
      * Collaboratively developed an automated opportunistic screening pipeline to detect vertebral compression fractures on lateral radiographs of the spine
      * Collaboratively developed ensemble method of segmentation models for above pipeline using both CNN- and ResNet-based architectures
      * Fine-tuned Segment Anything 2 for above pipeline achieving a 20% increase in PPV for fracture detection
      * Assisted in migration of legacy PACS data and retiring a data lake at UW Medicine

  - title: Neuroscience Research Assistant
    company: NYU Neuroscience Institute
    company_url: 'https://med.nyu.edu/departments-institutes/neuroscience/'
    company_logo:
    location: New York, NY, USA
    date_start: '2011-08-03'
    date_end: '2014-06-05'
    description: |2-
      * Lead engineer in building custom optrodes used to study behavioral aggression in transgenic mice via electrophysiology and optogenetics
      * Conducted stereotaxic surgeries ensuring precise viral delivery of channelrhodopsin, which enabled targeted study of neural circuits in aggression pathways
      * Executed in vivo optrode and electrophysiology recordings, achieving high-resolution neural signal capture critical for identifying aggression-related neural patterns
      * Conducted comprehensive histochemical analysis with perfusion and cryosection, ensuring precise localization of neural markers across 10+ experimental subjects
design:
  columns: '1'
---
