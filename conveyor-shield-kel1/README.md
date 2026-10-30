# Conveyor Sorter Shield (Group 1)

> Group project – KCCI Firmware & PCB modules, Kelompok 1.

A 2-layer shield for the **STM32 Nucleo-F411RE** that powers and connects all peripherals of the conveyor-belt sorting
system built in the firmware module.

## Connections

| Ref | Connects to |
|---|---|
| J9 | 12 V input – main supply |
| Buck1 | LM2596 step-down module – 12 V → 5 V for the Nucleo and peripherals |
| J8 | BTS7960 DC conveyor-motor driver |
| J3 | Sorting-gate servo |
| J4 | Time-of-flight distance sensor |
| J1 | OLED display |
| J2 | Rotary encoder |
| J5 | Relay module |
| J6 / J7 | Start / Emergency buttons |
| SW1 | Nucleo reset button |

## Files

| Path | Contents |
|---|---|
| [`kicad/`](kicad/) | KiCad 10 project and the `Komponen_Kustom` symbol library |

The Nucleo and LM2596 footprints are embedded in the board file. The LM2596 3D model path points to a teammate's local
library, so it will show as missing in the 3D viewer; the PCB itself is unaffected.
