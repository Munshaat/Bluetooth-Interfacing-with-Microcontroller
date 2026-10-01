# Bluetooth Interfacing and Smart Control Using 8051

A microcontroller-based project demonstrating **Bluetooth communication and smart device control using the 8051 microcontroller**. The system uses an **HC-05 Bluetooth module** to establish wireless communication with the 8051 and control LEDs and relays through UART communication.

## Project Overview

The project explores wireless interfacing between an **8051 microcontroller** and an **HC-05 Bluetooth module**.

Bluetooth commands received through the UART interface are processed by the 8051 to control connected output devices. The project also demonstrates a Morse-code-based interaction using LEDs and an LCD.

## Key Features

* Bluetooth communication using **HC-05**
* UART-based serial communication with the 8051
* Wireless control of multiple output devices
* Control of **8 LEDs**
* Relay-based device control
* Morse-code representation using dot and dash
* LCD-based display
* 8051 Assembly Language implementation
* Circuit simulation and verification using Proteus

## Hardware Components

* 8051 Microcontroller
* HC-05 Bluetooth Module
* 8 LEDs
* Relays
* LCD Display
* Resistors
* Power and interfacing components

## Pin Configuration

| Component | 8051 Connection                                |
| --------- | ---------------------------------------------- |
| HC-05 RXD | P3.0 / UART interface                          |
| HC-05 TXD | P3.1 / UART interface                          |
| Relay 1   | P3.2                                           |
| Relay 2   | P3.3                                           |
| LCD       | Connected through the designated LCD interface |
| LEDs      | P1.0 – P1.7                                    |

## Working Principle

The HC-05 Bluetooth module receives commands from a paired Bluetooth device and transfers the received data to the 8051 through UART communication.

The 8051 processes the received command and generates the corresponding output:

```text
Bluetooth Device
       │
       ▼
    HC-05
       │
     UART
       │
       ▼
  8051 MCU
       │
 ┌─────┴───────────┐
 ▼                 ▼
LED Control    Relay Control
       │
       ▼
   LCD / Morse
   Indication
```

## Morse Code Function

The project also demonstrates Morse-code output using the LEDs.

Received or programmed characters can be represented using:

* **Dot (.)**
* **Dash (-)**

The LED outputs are controlled according to the corresponding Morse pattern, while the LCD provides additional visual information.

## Software and Tools

* **Proteus** — Circuit design and simulation
* **8051 Assembly Language** — Microcontroller programming
* **HC-05 Bluetooth** — Wireless communication
* **UART** — Serial communication

## Project Highlights

* Implemented UART communication between an 8051 microcontroller and HC-05 Bluetooth module.
* Developed Assembly Language routines for receiving and processing serial data.
* Controlled LEDs and relays using wireless commands.
* Implemented Morse-code indication using LED outputs.
* Integrated an LCD for displaying information.
* Tested the complete system through Proteus simulation.

## Repository Structure

```text
bluetooth-interfacing-8051/
│
├── README.md
├── Bluetooth Interfacing and Smart Control Using 8051.pdf
│
├── Proteus/
│   └── [Proteus project files]
│
└── Code/
    └── [8051 Assembly source files]
```

## Academic Project

**Department of Electrical and Electronic Engineering**
**Islamic University of Technology (IUT)**

**Project:** Bluetooth Interfacing and Smart Control Using 8051
