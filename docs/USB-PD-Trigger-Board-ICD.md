# Interface Control Document - USB-PD-Trigger-Board

## 1. External Interfaces

### 1.1 USB Type-C Input (J1)

- **Connector Type:** USB Type-C Receptacle
- **Function:** Power input and PD negotiation
- **Signals:** VBUS, GND, CC1, CC2

### 1.2 DC Power Output (J2)

- **Connector Type:** DC Barrel Jack / Terminal Block
- **Function:** Negotiated power output
- **Voltage:** 5V - 20V (Configurable)
- **Current:** Max 5A

## 2. Internal Configuration

### 2.1 Voltage Selection (VSEL)

Resistor divider on the VSEL pin of CYPD3177 determines the target voltage:

| Resistor Value | Target Voltage |
|----------------|----------------|
| Open           | 5V             |
| ...            | ...            |

### 2.2 Current Selection (ILIM)

Resistor on ILIM pin sets the maximum current limit requested from the source.

---
_Last Updated: 22-01-2026_
