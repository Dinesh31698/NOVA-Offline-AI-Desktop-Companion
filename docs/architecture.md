# NOVA System Architecture

## Overview

NOVA is an AI desktop companion built around a Raspberry Pi and a
local AI architecture.

The system combines conversational AI, memory, personality, emotion,
computer vision, voice interaction, touch interaction, and animated
OLED expressions.

The Raspberry Pi handles the physical interaction and companion
interface, while a Windows laptop runs the local language model through
Ollama.

---

## High-Level Architecture

```text
                         ┌──────────────────┐
                         │       USER       │
                         └────────┬─────────┘
                                  │
              ┌───────────────────┼───────────────────┐
              │                   │                   │
              ▼                   ▼                   ▼
            Voice               Face               Touch
              │                   │                   │
              └───────────────────┼───────────────────┘
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │   Raspberry Pi 3B+  │
                       │                     │
                       │ Input Processing    │
                       │ Conversation        │
                       │ Memory              │
                       │ Emotion             │
                       │ Personality         │
                       │ Hardware Control    │
                       └──────────┬──────────┘
                                  │
                           Private Wi-Fi/LAN
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │    Windows Laptop   │
                       │                     │
                       │      Ollama         │
                       │      Llama 3.2      │
                       │                     │
                       │    Local LLM        │
                       └──────────┬──────────┘
                                  │
                           AI Response
                                  │
                                  ▼
                       ┌─────────────────────┐
                       │   Raspberry Pi 3B+  │
                       │                     │
                       │ Emotion / Mood      │
                       │ Memory              │
                       │ Personality         │
                       │ Actions             │
                       └──────────┬──────────┘
                                  │
                    ┌─────────────┼─────────────┐
                    ▼             ▼             ▼
                 ┌──────┐    ┌────────┐    ┌────────┐
                 │ OLED │    │Speaker │    │Actions │
                 └──────┘    └────────┘    └────────┘