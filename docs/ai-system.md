# NOVA AI System

## Overview

NOVA combines local conversational AI with memory, personality, mood,
emotion, and interactive behavior.

The AI system connects the user's interaction with NOVA's conversational
response and companion behavior.

---

## AI Architecture

```text
                         USER
                           │
             ┌─────────────┼─────────────┐
             │             │             │
             ▼             ▼             ▼
           Voice         Vision         Touch
             │             │             │
             └─────────────┼─────────────┘
                           ▼
                  ┌─────────────────┐
                  │  NOVA Input     │
                  │   Processing    │
                  └────────┬────────┘
                           │
                           ▼
                  ┌─────────────────┐
                  │ Conversation    │
                  │     Logic       │
                  └────────┬────────┘
                           │
                    Private Wi-Fi/LAN
                           │
                           ▼
                  ┌─────────────────┐
                  │     Ollama      │
                  │                 │
                  │    Llama 3.2    │
                  └────────┬────────┘
                           │
                       AI Response
                           │
                           ▼
                  ┌─────────────────┐
                  │  NOVA Behavior  │
                  └────────┬────────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
          Emotion        Memory       Personality
             │             │             │
             └─────────────┼─────────────┘
                           ▼
                    Response / Action
                           │
                ┌──────────┴──────────┐
                ▼                     ▼
              OLED                  Speaker