# NOVA Setup

## Overview

This document describes the basic environment required to run the
NOVA project on its Raspberry Pi and local AI system.

---

# System Architecture

NOVA uses a distributed setup:

```text
┌──────────────────────┐
│   Raspberry Pi 3B+   │
│                      │
│  Hardware Interface  │
│  OLED                │
│  Touch               │
│  Webcam              │
│  Microphone          │
│  Speaker             │
└──────────┬───────────┘
           │
       Private LAN
           │
           ▼
┌──────────────────────┐
│    Windows Laptop    │
│                      │
│       Ollama         │
│          │           │
│          ▼           │
│      Llama 3.2       │
└──────────────────────┘