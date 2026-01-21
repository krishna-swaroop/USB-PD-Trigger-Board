# Board Design Document - USB-PD-Trigger-Board

## Overview

The **USB-PD-Trigger-Board** is a USB Power Delivery (PD) sink board based on the **Cypress CYPD3177 (EZ-PD™ BCR)** controller. It is designed to "trigger" or negotiate specific voltage and current profiles from a USB-PD power source (like a wall adapter or power bank) and provide that power to a DC barrel jack or header.

## Key Specifications

- **Controller:** Cypress CYPD3177 (EZ-PD™ BCR)
- **Input:** USB Type-C (PD 2.0/3.0 compliant)
- **Output Voltage:** Configurable via resistors (5V, 9V, 12V, 15V, 20V)
- **Output Current:** Up to 5A (depending on source)
- **Status Indication:** LED for PD negotiation status
- **Protection:** Integrated VBUS-to-CC short protection

## Architecture

The board follows the reference design for CYPD3177, providing a plug-and-play solution for converting USB-C PD power to standard DC rails.

---
_Last Updated: 22-01-2026_
