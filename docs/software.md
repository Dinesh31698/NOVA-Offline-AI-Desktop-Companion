# NOVA Software Stack

## Overview

NOVA is primarily developed using Python and combines local AI,
computer vision, voice interaction, OLED graphics, hardware control,
and networking.

---

## Programming Language

### Python

Python is the primary programming language used for NOVA.

It connects the AI, hardware, computer vision, voice, memory, emotion,
and interaction components.

---

## Local AI

### Ollama

Ollama provides the local language-model runtime for NOVA.

It runs on the Windows laptop and provides the interface for local LLM
inference.

### Llama 3.2

Llama 3.2 is the documented language model used by NOVA's local AI
architecture.

```text
Raspberry Pi
     │
     │ Private Wi-Fi / LAN
     ▼
Windows Laptop
     │
     ▼
Ollama
     │
     ▼
Llama 3.2