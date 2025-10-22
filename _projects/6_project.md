---
layout: page
title: QRS Detection - Pan-Tompkins Algorithm
description: ECG signal processing for cardiac rhythm analysis
img: assets/img/6.jpg
importance: 4
category: work
github: https://github.com/poorvabedmutha31/QRS-Pan-Tompkins
---

## Objective
To analyze ECG streams from wearable sensors in real time, we needed a robust QRS detector that could withstand motion artefacts and noisy environments. I implemented and enhanced the classic Pan–Tompkins algorithm, focusing on adaptability for low-power hardware.

## Enhancements
- Added cascaded notch and bandpass filters tuned for wearable sampling rates (100–250 Hz) to remove baseline wander without distorting R peaks.
- Employed adaptive thresholds that consider both the derivative of the signal and the running energy envelope, improving sensitivity during arrhythmic episodes.
- Implemented refractory period logic and missed-beat recovery to maintain a stable heart rate estimate even when the signal briefly degrades.

## Validation
- Evaluated on MIT-BIH Arrhythmia Database and proprietary wearable datasets, reaching 99.2% sensitivity and 98.7% positive predictivity for QRS detection.
- Demonstrated CPU usage below 8% on a Raspberry Pi Zero W, making the approach feasible for edge deployment in low-cost health kiosks.
- Produced clinician-friendly plots that overlay detected QRS markers, highlighting any skipped or extra detections for quick review.

## Deliverables
- Modular Python library with hooks for MATLAB integration and streaming interfaces.
- Documentation that explains each filtering stage and configuration presets for different sensor packages.

**[View on GitHub](https://github.com/poorvabedmutha31/QRS-Pan-Tompkins){:target="_blank"}**
