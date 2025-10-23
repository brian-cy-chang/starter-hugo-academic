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
  - title: Senior Machine Learning Engineer
    company: Accompany Health
    company_url: 'https://accompanyhealth.com/'
    company_logo:
    location: Bethesda, MD, USA
    date_start: '2025-05-12'
    date_end: ''
    description: |2-
      * Designed a framework to summarize clinical evidence for hierarchical condition categories (HCCs) for clinical operations teams to decrease manual documentation review
      * Designed and developed Retrieval-Augmented Generation (RAG) pipelines in Vellum AI, deployed as bots to assist healthcare providers, optimizing clinical workflows and decreasing time spent on manual policy and evidence-based guidelines review by 40%
      * Implemented and deployed internal versions of LLM-as-a-judge custom metrics to evaluate RAG pipelines for performance and trustworthiness

  - title: Graduate Research Assistant
    company: University of Washington
    company_url: 'https://www.allofus.nih.gov/funding-and-program-partners/center-for-linkage-and-aquisition-of-data'
    company_logo:
    location: Seattle, WA, USA
    date_start: '2023-09-16'
    date_end: '2025-03-15'
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

design:
  columns: '1'
---
