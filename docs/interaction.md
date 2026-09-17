# NOVA Interaction System

## Overview

NOVA is designed as a multimodal desktop companion. It combines voice,
vision, touch, conversational AI, memory, emotion, and an expressive
OLED interface.

The interaction system connects these different input and output
channels into a single companion experience.

---

## Interaction Architecture

```text
                         USER
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
        Voice            Vision           Touch
          │                │                │
     Microphone          Webcam          TTP223B
          │                │                │
          └────────────────┼────────────────┘
                           ▼
                    NOVA Input Layer
                           │
                           ▼
                   Conversation Logic
                           │
                           ▼
                   Ollama + Llama 3.2
                           │
                           ▼
                    AI Response
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
           Memory       Emotion     Personality
              │            │            │
              └────────────┼────────────┘
                           ▼
                     NOVA Behavior
                           │
                ┌──────────┴──────────┐
                ▼                     ▼
              OLED                  Speaker
          Expressions            Voice Output