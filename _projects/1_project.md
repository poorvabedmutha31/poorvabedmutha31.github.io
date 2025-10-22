---
layout: page
title: SpO2 and Heart Rate Measurement using Smartphone Camera
description: Real-time physiological measurements from smartphone video
img: assets/img/12.jpg
importance: 1
category: work
github: https://github.com/poorvabedmutha31/SpO2-and-Heart-Rate-measurement-using-smartphone-camera
related_publications: true
---

## Motivation
Pulse oximeters are ubiquitous, yet they still require dedicated hardware that can be hard to distribute in low-resource settings. I set out to capture the same vital signs with only a smartphone camera and lightweight signal processing so that remote clinics and telehealth programs could gather longitudinal measurements without additional sensors.

## What I built
- A photoplethysmography pipeline that isolates fingertip ROIs, performs temporal filtering, and stabilizes illumination variations to estimate SpO₂ and heart rate in real time.
- Calibration routines that adapt to skin tone and ambient lighting by modulating exposure time and using per-channel gain compensation.
- A responsive interface that streams live vitals, highlights signal quality warnings, and logs anonymized sessions for clinician review.

## Results
- Matched reference pulse oximeter readings within 0.95% RMSE for SpO₂ and below 2 BPM error for heart rate across 25 participants.
- Reduced sampling requirements by 40% compared with traditional pipelines, enabling smooth performance on mid-range Android devices.
- Integrated a privacy-preserving export that shares only summary vitals, not raw video, aligning with telehealth compliance requirements.

## Stack
- Python, OpenCV, NumPy, SciPy for signal processing and prototyping.
- TensorFlow Lite for optional motion artefact rejection on-device.
- Flask API that streams processed vitals to a clinician dashboard.

**[View on GitHub](https://github.com/poorvabedmutha31/SpO2-and-Heart-Rate-measurement-using-smartphone-camera){:target="_blank"}**
