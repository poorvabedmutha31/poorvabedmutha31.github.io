---
layout: page
title: "SciPred — Predatory Journal Detection"
description: NLP pipeline to detect predatory journals using SciBERT embeddings
img: assets/img/3.jpg
importance: 2
category: work
github: https://github.com/poorvabedmutha31/SciPred
---

## Overview
SciPred is an end-to-end text classification pipeline I developed to detect predatory journals by analyzing article and journal text features using SciBERT embeddings and a lightweight MLP classifier.

## Approach
- Collected and cleaned a dataset of journal and article metadata and descriptions; used web-scraping with BeautifulSoup to assemble training data.
- Embedded textual content with SciBERT and trained an MLP classifier to distinguish predatory outlets from legitimate journals.
- Applied careful preprocessing and class-balancing to improve model stability.

## Results
- Achieved an F1 score of 0.92 on held-out data, outperforming baseline text-only models by ~8%.

## Stack
- Python, HuggingFace Transformers (SciBERT), PyTorch, scikit-learn, BeautifulSoup.

**[View on GitHub](https://github.com/poorvabedmutha31/SciPred){:target="_blank"}**
