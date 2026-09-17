# NOVA Vision System

## Overview

NOVA uses a webcam and computer-vision processing to understand visual
interaction with the user.

The vision system provides face-based awareness that can be used by
NOVA's interaction and companion behavior.

---

## Vision Architecture

```text
                         USB Webcam
                              │
                              ▼
                           OpenCV
                              │
                 ┌────────────┼────────────┐
                 │            │            │
                 ▼            ▼            ▼
             Face          Face         Facial
           Detection     Tracking     Expression
                 │            │         Awareness
                 └────────────┼────────────┘
                              ▼
                       NOVA Vision Data
                              │
                 ┌────────────┼────────────┐
                 ▼            ▼            ▼
             Greeting      Emotion      Interaction
                 │            │            │
                 └────────────┼────────────┘
                              ▼
                         NOVA Behavior