# NOVA System Architecture

```text
                         ┌─────────────────────┐
                         │        USER         │
                         └──────────┬──────────┘
                                    │
                   ┌────────────────┼────────────────┐
                   │                │                │
                   ▼                ▼                ▼
              ┌─────────┐      ┌─────────┐      ┌─────────┐
              │  VOICE  │      │ VISION  │      │  TOUCH  │
              │   Mic   │      │ Webcam  │      │ TTP223B │
              └────┬────┘      └────┬────┘      └────┬────┘
                   │                │                │
                   └────────────────┼────────────────┘
                                    ▼
                         ┌─────────────────────┐
                         │    RASPBERRY PI     │
                         │       3B+           │
                         │                     │
                         │ Input Processing    │
                         │ Conversation Logic  │
                         │ Memory              │
                         │ Emotion             │
                         │ Personality         │
                         └──────────┬──────────┘
                                    │
                              Private LAN
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │   WINDOWS LAPTOP    │
                         │                     │
                         │       Ollama        │
                         │          │          │
                         │          ▼          │
                         │      Llama 3.2      │
                         └──────────┬──────────┘
                                    │
                              AI Response
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │    NOVA Behavior    │
                         └──────────┬──────────┘
                                    │
                         ┌──────────┴──────────┐
                         │                     │
                         ▼                     ▼
                  ┌─────────────┐       ┌─────────────┐
                  │ SSD1306 OLED│       │   SPEAKER   │
                  │             │       │             │
                  │ Expressions │       │ Voice Output│
                  │ Animations  │       │             │
                  └─────────────┘       └─────────────┘