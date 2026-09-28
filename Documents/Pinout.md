# ESP32 Prototyping & Breakout Board — Pinout

This document describes the header arrangement used in the PCB design.

## Important: Pin Numbering

The KiCad schematic labels the ESP32 connections using the **physical ESP32 module pin numbers 1–38**.

These numbers are **not GPIO numbers**.

The board therefore uses the same numbering convention as the schematic so that the physical PCB, schematic, and layout remain consistent.

For the GPIO function associated with a physical ESP32 module pin, refer to the pinout of the specific ESP32 development board/module being used.

## 19-Pin Header Arrangement

Each side of the ESP32 module is represented by a 19-pin header.

### ESP32 Module Pins 1–19

| Header Pin | ESP32 Module Pin |
|---:|---:|
| 1 | 1 |
| 2 | 2 |
| 3 | 3 |
| 4 | 4 |
| 5 | 5 |
| 6 | 6 |
| 7 | 7 |
| 8 | 8 |
| 9 | 9 |
| 10 | 10 |
| 11 | 11 |
| 12 | 12 |
| 13 | 13 |
| 14 | 14 |
| 15 | 15 |
| 16 | 16 |
| 17 | 17 |
| 18 | 18 |
| 19 | 19 |

### ESP32 Module Pins 20–38

The paired 19-pin header exposes the remaining physical module pins.

| Header Pin | ESP32 Module Pin |
|---:|---:|
| 1 | 20 |
| 2 | 21 |
| 3 | 22 |
| 4 | 23 |
| 5 | 24 |
| 6 | 25 |
| 7 | 26 |
| 8 | 27 |
| 9 | 28 |
| 10 | 29 |
| 11 | 30 |
| 12 | 31 |
| 13 | 32 |
| 14 | 33 |
| 15 | 34 |
| 16 | 35 |
| 17 | 36 |
| 18 | 37 |
| 19 | 38 |

## Power and Ground Rails

The board also provides dedicated headers for the board-level power rails:

| Rail | Purpose |
|---|---|
| 5V Rail | Access to the board's 5 V supply |
| 3.3V Rail | Access to the regulated 3.3 V supply |
| GND Rail | Ground connection |

These rails are intended to simplify connections to sensors, modules, and other peripherals during prototyping.

## Test LED

A separate header is provided for the test LED connection.

| Connection | Description |
|---|---|
| Test LED | External access to the test LED connection |

## ESP32 Form Factors

The PCB contains multiple ESP32 header arrangements so that the same prototyping platform can be used with different ESP32 development-board sizes.

The exact mechanical compatibility depends on the physical pin spacing and board dimensions of the ESP32 development board.

## Schematic Reference

For the authoritative electrical connections, refer to:

```text
KiCad/pcb_esp32_v1.kicad_sch
```

For the physical placement and routing, refer to:

```text
KiCad/pcb_esp32_v1.kicad_pcb
```
