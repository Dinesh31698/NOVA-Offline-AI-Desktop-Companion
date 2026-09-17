# NOVA Voice System

## Overview

NOVA supports voice-based interaction through a microphone for input
and a speaker for spoken responses.

The voice system connects speech interaction with NOVA's local AI,
memory, personality, and companion behavior.

---

## Voice Architecture

```text
                     User
                      │
                      ▼
                 Microphone
                      │
                      ▼
              Speech Processing
                      │
                      ▼
              NOVA Conversation
                      │
                      ▼
               Ollama + Llama 3.2
                      │
                      ▼
                AI Response
                      │
                      ▼
             Text-to-Speech
                      │
                      ▼
                  Speaker