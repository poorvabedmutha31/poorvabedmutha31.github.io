---
layout: page
title: Emotion-Based Music Player
description: Music recommendation system based on emotional state
img: assets/img/7.jpg
importance: 3
category: work
github: https://github.com/poorvabedmutha31/Emotion-Based-Music-Player
---

## Why I built it
Listeners often want playlists that meet them where they are emotionally, especially while studying or winding down. I developed EmotionTune, a desktop music player that pairs real-time affect detection with curated Spotify playlists so users can shift or sustain their moods intentionally.

## System highlights
- Captures webcam frames, runs a lightweight CNN emotion classifier, and smooths predictions with temporal attention to avoid jittery playlist switches.
- Maps affective states onto arousal–valence coordinates and selects playlists using Spotify’s audio features (danceability, energy, speechiness).
- Provides a feedback loop where listeners can “nudge” toward desired emotions, enabling shared control between the model and the user.

## Impact
- Used by 30 volunteers during focus groups; 83% reported the adaptive playlists helped them stay engaged while studying.
- Logged anonymized usage statistics to refine the emotion-to-genre mapping and identify gaps (e.g., low-energy happy tracks).
- Served as the foundation for my later wellbeing prototypes that combine audio interventions with biofeedback.

## Tech stack
- JavaFX interface with REST calls to a Python microservice that handles inference and playlist curation.
- Spotify Web API, TensorFlow, and MongoDB for session storage and future personalization analyses.

**[View on GitHub](https://github.com/poorvabedmutha31/Emotion-Based-Music-Player){:target="_blank"}**
