# NOVA Features

NOVA combines local conversational AI, memory, emotion, personality,
computer vision, voice interaction, touch input, and expressive OLED
feedback into a single desktop companion.

---

## 1. Local AI Conversation

NOVA provides conversational interaction using a local language-model
architecture.

The AI processing layer uses:

- Ollama
- Llama 3.2
- Local LLM inference

The language model runs on the connected laptop while the Raspberry Pi
handles the companion interface.

---

## 2. Natural Voice Interaction

NOVA supports voice-based interaction through microphone input and
spoken responses through a speaker.

The voice interaction system is designed to support natural
conversations rather than only fixed commands.

---

## 3. Contextual Memory

NOVA uses memory to maintain context across interactions.

Memory-related features include:

- Conversation context
- Long-term memory
- User information
- Preferences
- Reminders
- Daily journal

Memory allows interactions to become more contextual instead of treating
every conversation as completely independent.

---

## 4. Emotion Engine

NOVA includes an emotion system that allows its behavior and visual
expressions to respond to interaction.

The emotion system includes:

- Dynamic emotional states
- Mood transitions
- Emotion-based behavior
- Emotion-based expressions

The documented emotional architecture uses OCC and PAD concepts together
with personality and memory influences.

---

## 5. Adaptive Personality

NOVA is designed with a personality that changes through interaction.

Personality-related features include:

- Adaptive personality
- Interaction-based personality changes
- Friendship progression
- XP
- Levels
- Unlockable behaviors

These features allow NOVA's behavior to develop through continued
interaction.

---

## 6. Self-Talk

NOVA includes self-directed conversational behavior.

Self-talk allows NOVA to generate interactions without requiring every
interaction to begin with a direct user command.

---

## 7. Dream Mode

NOVA includes a dream-mode behavior as part of its companion
personality system.

Dream behavior provides an additional autonomous interaction state.

---

## 8. Attention-Seeking Behavior

NOVA includes attention-seeking behavior as part of its companion
personality.

This allows the system to initiate interaction and behave more like an
interactive digital companion.

---

## 9. Face Detection

NOVA uses a camera-based computer-vision system for detecting faces.

The camera provides visual input that can be used as part of NOVA's
environmental awareness.

---

## 10. Face Recognition

NOVA includes face-recognition functionality for identifying known
users.

This allows NOVA to provide more personalized interaction based on
recognized users.

---

## 11. Face Tracking

NOVA supports face tracking through its camera-based vision system.

Face tracking allows the system to follow detected faces within the
camera view.

---

## 12. Facial Expression Awareness

NOVA includes facial-expression awareness as part of its computer-vision
interaction system.

Visual information can therefore contribute to NOVA's interaction and
behavior.

---

## 13. Time-Aware Greetings

NOVA provides greetings based on the time context.

This allows interactions to be more appropriate to the current part of
the day.

---

## 14. Birthday and Event Remembrance

NOVA can remember birthdays and events and respond with dedicated
interactions.

The project includes a dedicated birthday animation demonstrated on the
OLED display.

---

## 15. Weather Updates

NOVA provides weather-related interactions and updates.

Weather information can be incorporated into the companion's responses.

---

## 16. Reminders

NOVA supports reminders as part of its personal-assistance features.

Reminders can be incorporated into the companion's interaction flow.

---

## 17. Animated OLED Face

The SSD1306 OLED acts as NOVA's visual face.

The display provides animated visual feedback including:

- Eyes
- Facial expressions
- Emotional expressions
- Speaking animations
- Thinking animations
- Singing mode
- Interactive screens

---

## 18. Emotion-Based Expressions

NOVA's OLED expressions can represent different emotional and behavioral
states.

The visual expression system connects NOVA's internal interaction state
with visible animations.

---

## 19. Storytelling Mode

NOVA supports interactive storytelling.

The storytelling system combines conversational AI with expressive OLED
animations and voice interaction.

---

## 20. Study Buddy Mode

NOVA includes a Study Buddy mode for learning assistance.

It provides:

- Explanations
- Quizzes
- Learning assistance

This allows NOVA to act as an interactive study companion.

---

## 21. Mini-Games

NOVA includes interactive mini-games displayed through the OLED
interface.

Games provide an additional way for users to interact with the
companion.

---

## 22. Interactive Entertainment

NOVA supports interactive entertainment through:

- Storytelling
- Mini-games
- Interactive activities
- Singing mode

These features use the OLED and conversational interface to create
different companion experiences.

---

## 23. Capacitive Touch Interaction

The TTP223B capacitive touch sensor provides physical touch input.

Touch can be used as an interaction method alongside voice and vision.

---

## 24. Multi-Modal Interaction

NOVA combines multiple interaction channels:

```text
                 ┌───────────────┐
                 │     NOVA      │
                 └───────┬───────┘
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
        Voice          Vision          Touch
          │              │              │
      Microphone       Webcam         TTP223B
          │              │              │
          └──────────────┼──────────────┘
                         ▼
                  NOVA AI System
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
            OLED                  Speaker
         Expressions           Voice Output