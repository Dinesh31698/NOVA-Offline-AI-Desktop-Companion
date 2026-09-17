# NOVA Hardware Wiring

## Overview

NOVA uses the Raspberry Pi as the main hardware controller. The
SSD1306 OLED provides the visual face, the TTP223B provides touch
input, and the webcam, microphone, and speaker provide vision and
voice interaction.

---

## Hardware Connections

### SSD1306 OLED

| OLED Pin | Raspberry Pi |
|---|---|
| VCC | 3.3V — Physical Pin 1 |
| GND | GND — Physical Pin 6 |
| SDA | GPIO2 — Physical Pin 3 |
| SCL | GPIO3 — Physical Pin 5 |

The OLED communicates with the Raspberry Pi using the I²C interface.

The documented OLED address is:

```text
0x3C