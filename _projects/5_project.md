---
layout: page
title: Exoplanet Detection
description: Astronomical data analysis for exoplanet discovery
img: assets/img/1.jpg
importance: 3
category: work
github: https://github.com/poorvabedmutha31/Exoplanet-Detection
---

## Overview
During my undergraduate research I explored how transit photometry data could be processed with machine learning to flag exoplanet candidates more efficiently. The goal was to build an interpretable baseline that could triage thousands of light curves before expensive astronomer review.

## Pipeline
- Retrieved Kepler and TESS light curves, detrended them with Savitzky–Golay filters, and normalized flux to remove instrument artefacts.
- Extracted features including transit depth, duration, folding periodicity, and out-of-transit variability; supplemented with Wavelet decomposition coefficients for subtle periodic cues.
- Trained gradient boosting and 1D CNN models while constraining for class imbalance and high false-positive penalties.

## Key results
- Reached 96% balanced accuracy and 0.94 AUC on NASA’s vetted training split.
- Reduced manual inspection workload by half within our 5-person research group, allowing us to focus on ambiguous cases and follow-up observations.
- Published dashboards that visualize each candidate’s phased light curve, residuals, and SHAP attributions for astronomy collaborators.

## Tooling
- Python, LightGBM, TensorFlow, AstroPy, Plotly Dash for visualization, Docker for reproducible processing pipelines.
- Continuous integration with GitHub Actions to rerun feature extraction when new mission data releases drop.

**[View on GitHub](https://github.com/poorvabedmutha31/Exoplanet-Detection){:target="_blank"}**
