# NOVA Hardware

## Hardware Overview

NOVA combines Raspberry Pi hardware with a visual display, camera,
touch input, microphone, and speaker to create an interactive desktop
AI companion.

```text
                         NOVA Hardware
                              │
                    ┌─────────┴─────────┐
                    │   Raspberry Pi    │
                    │    Controller     │
                    └─────────┬─────────┘
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
          ▼                   ▼                   ▼
        OLED              Touch Sensor          Camera
          │                   │                   │
          ▼                   ▼                   ▼
     Expressions         Interaction          Vision
                             
                         ┌────┴────┐
                         ▼         ▼
                    Microphone  Speaker