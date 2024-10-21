---
title: "Using an Ensemble of Segmentation Methods to Detect Vertebral Bodies on Radiographs"
date: 2024-08-29
authors:
- admin
- Jonathan Renslo
- Qifei Dong
- Sandra K. Johnston
- Jessic Perry
- David R. Haynor
- Gang Luo
- Nancy Lane
- Jeffrey G. Jarvik
- Nathan M. Cross

# author_notes:
# - ""

publication_types: ["2"]
abstract: "**Background and Purpose:** We have developed an ensemble of vertebral body (VB) segmentation models for lateral radiographs as a critical component of an automated, opportunistic screening tool. Our goal is to detect the approximate location of thoracic and lumbar VBs, including fractured vertebra, on lateral radiographs.

<br><br>**Materials and Methods:** The Osteoporotic Fractures in Men Study (MrOS) data set includes spine radiographs of 5994 men aged ≥65 years from 6 clinical centers. Two segmentation models, U-Net and Mask-RCNN (Region-based Convolutional Neural Network), were independently trained on the MrOS data set retrospectively, and an ensemble was created by combining them. Primary performance metrics for VB detection success included precision, recall, and F1 score for object detection on a held-out test set. Intersection over union (IoU) and Dice coefficient were also calculated as secondary metrics of performance for the test set. A separate external data set from a quaternary health care enterprise was acquired to test generalizability, comprising diagnostic clinical radiographs from men and women aged ≥65 years.

<br><br>**Results:** The trained models achieved F1 score of U-Net = 83.42%, Mask-RCNN = 86.30%, and ensemble = 88.34% in detecting all VBs, and F1 score of U-Net = 87.88%, Mask-RCNN = 92.31%, and ensemble = 97.14% in detecting severely fractured vertebrae. The trained models achieved an average IoU per VB of 0.759 for U-Net and 0.709 for Mask-RCNN. The trained models achieved F1 score of U-Net = 81.11%, Mask-RCNN = 79.24%, and ensemble = 87.72% in detecting all VBs in the external data set.

<br><br>**Conclusion:** An ensemble model combining predictions from U-Net and Mask-RCNN resulted in the best performance in detecting VBs on lateral radiographs and generalized well to an external data set. This model could be a key component of a pipeline to detect fractures on all vertebrae in a radiograph in an automated, opportunistic screening tool under development.

"
featured: true
publication: "*American Journal of Neuroradiology (AJNR)*"
doi: "10.3174/ajnr.A8343"
tags: ["machine learning", "artificial intelligence", "segmentation" ,"object detection", "radiograph", "vertebral body", "ensemble model", "Mask-RCNN", "U-Net", "radiograph"]
---