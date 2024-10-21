---
title: "Subject-level spinal osteoporotic fracture prediction combining deep learning vertebral outputs and limited demographic data"
date: 2024-09-10
authors:
- Nathan M. Cross
- Jessica Perry
- Qifei Dong
- Gang Luo
- admin
- Nancy E. Lane
- Lynn Marshall
- Sandra K. Johnston
- David R. Haynor
- Jeffrey G. Jarvik
- Patrick J. Heagerty


# author_notes:
# - ""

publication_types: ["2"]
abstract: "**Purpose:** Osteoporotic vertebral fractures are common and morbid. Automated opportunistic screening for incidental vertebral fractures from radiographs, the highest volume imaging modality, could improve osteoporosis detection and management. We consider how to form patient-level fracture predictions and summarization to guide management, using our previously developed vertebral fracture classifier on segmented radiographs from a prospective cohort study of US men (MrOS). We compare the performance of logistic regression (LR) and generalized additive models (GAM) with combinations of individual vertebral scores and basic demographic covariates.

<br><br>**Methods:** Subject-level LR and GAM models were created retrospectively using all fracture predictions or summary variables such as order statistics, adjacent vertebral interactions, and demographic covariates (age, race/ethnicity). The classifier outputs for 8663 vertebrae from 1176 thoracic and lumbar radiographs in 669 subjects were divided by subject to perform stratified fivefold cross-validation. Models were assessed using multiple metrics, including receiver operating characteristic (ROC) and precision-recall (PR) curves.

<br><br>**Results:** The best model (AUC-ROC = 0.968) was a GAM using the top three maximum vertebral fracture scores and age. Using top-ranked scores only, rather than all vertebral scores, improved performance for both model classes. Adding age, but not ethnicity, to the GAMs improved performance slightly.

<br><br>**Conclusion:** Maximal vertebral fracture scores resulted in the highest-performing models. While combining multiple vertebral body predictions risks decreasing specificity, our results demonstrate that subject-level models maintain good predictive performance. Thresholding strategies can be used to control sensitivity and specificity as clinically appropriate.

"
featured: false
publication: "*Archives of Osteoporosis*"
doi: "10.1007/s11657-024-01433-z"
tags: ["osteoporosis" ,"compression fracture", "logistic regression", "generalized additive model", "Bayesian", "imputation", "radiograph"]
---