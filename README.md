# 🔋 Otto HP — ESP32-S3 Battery Robot PCB

> EasyEDA · ESP32-S3 SuperMini · Li-ion charging and protection · 5 V boost

![Status](https://img.shields.io/badge/status-design-yellow)

<!-- TODO: 3D render -> media/render.png, assembled board photo -> media/board.jpg -->

## Overview

A compact controller board for a small Otto-style robot. It charges and protects a single Li-ion cell, boosts it to 5 V and runs everything from an ESP32-S3 SuperMini.

## Power path

```
Li-ion cell → TP4056 charger → DW01A + FS8205 protection → boost to 5 V → ESP32-S3 SuperMini + servos
```

| Block | Part |
|---|---|
| MCU | ESP32-S3 SuperMini |
| Charging | TP4056 |
| Protection | DW01A + FS8205 dual MOSFET |
| Regulation | Boost converter to 5 V |
| Connectors | JST battery connector, 2-pin power jumper (J1) |

<!-- TODO: schematic PDF -> hardware/schematic.pdf -->

## Author

**Jasin Jesin** · [LinkedIn](https://www.linkedin.com/in/jasinjesin/)
