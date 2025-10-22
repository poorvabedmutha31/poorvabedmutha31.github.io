---
layout: page
title: Classify Facial Expressions with Deep Learning
description: Emotion recognition using convolutional neural networks
img: assets/img/3.jpg
importance: 2
category: work
github: https://github.com/poorvabedmutha31/Classify-Facial-Expressions-with-Deep-Learning
giscus_comments: true
---

## Motivation
Emotion classification is fundamental for empathetic VR interfaces, yet many public models underperform on in-the-wild student data. I fine-tuned deep learning pipelines to capture subtle affect shifts for wellbeing check-ins without demanding additional sensors.

## Model design
- Combined a VGG-style encoder with attention pooling to keep inference light while handling FER2013 facial micro-expressions.
- Augmented grayscale frames with CLAHE and random occlusion to mimic webcam noise and improve robustness to masks.
- Open-sourced training notebooks with explainability reports (Grad-CAM overlays) that instructors can audit before deployment.

## Evaluation
- Achieved 71% macro-F1 on the FER2013 validation split and 68% macro-F1 on a held-out UCSD student dataset collected under IRB oversight.
- Reduced model size to 14 MB and exported to TensorFlow Lite for integration into browser-based prototypes.
- Benchmarked bias metrics across skin tone and gender presentation to monitor and document disparate error rates.

## Integration
- Packaged the classifier behind a REST API that returns emotion logits, confidence intervals, and the raw attention map for downstream UX.
- Authored documentation on ethical deployment and opt-in consent workflows for student wellbeing pilots.

**[View on GitHub](https://github.com/poorvabedmutha31/Classify-Facial-Expressions-with-Deep-Learning){:target="_blank"}**
