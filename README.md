# Metirionic Channel Sounding Evaluation Application

[![latest release](https://img.shields.io/github/v/release/Metirionic/mars-ranging-demo?label=latest%20release)](https://github.com/Metirionic/mars-ranging-demo/releases/latest)

Real-time distance monitoring using Bluetooth® Channel Sounding alongside
Metirionic's Advanced Ranging Stack (MARS).

The Channel Sounding Evaluation Application is a Windows desktop GUI for
visualizing continuous distance measurements between an initiator and a
reflector development kit, with insight into the signal path and how the
environment affects it.

> ℹ️ This repository hosts the **application** (the GUI). The matching
> **firmware images** for the boards are released separately in
> [`Metirionic/mars-cs-nrf54l`](https://github.com/Metirionic/mars-cs-nrf54l).

## Requirements

- **Windows 10 / 11 (x86_64)** — the app is a standalone binary, no installation required.
- A **pair of nRF54L15-based boards** — one flashed as **initiator**, one as
  **reflector**. Firmware is provided by the
  [`mars-cs-nrf54l`](https://github.com/Metirionic/mars-cs-nrf54l) repository
  (see [Firmware & supported hardware](#firmware--supported-hardware) below).

## Download

Grab the latest `mars-ranging-demo.exe` from the
[latest release](https://github.com/Metirionic/mars-ranging-demo/releases/latest).
It is a standalone Windows (x86_64) binary — download and run, no installer.

### Activation key

On first launch the GUI prompts for an **activation key**. Activation keys are
included with evaluation-kit purchases; additional keys are available through
Metirionic Support (`contact@metirionic.com`).

## Getting started

1. **Download** `mars-ranging-demo.exe` from the
   [latest release](https://github.com/Metirionic/mars-ranging-demo/releases/latest).
2. **Flash the boards** — flash one board with the **initiator** firmware and a
   second board with the **reflector** firmware. Prebuilt images and the
   flashing quickstart are in
   [`mars-cs-nrf54l` flash quickstart](https://github.com/Metirionic/mars-cs-nrf54l/blob/main/docs/flash-quickstart.md).
3. **Launch the app** — run `mars-ranging-demo.exe` and enter your activation key
   on first launch.
4. **Connect** the initiator board (it streams ranging data over UART).
5. **Observe live distance** measurements in real time.
6. **Export** measurement data to CSV or binary for further analysis.

## Firmware & supported hardware

The application is identical across all boards; only the firmware differs.
Firmware runs on nRF54L15-based boards and is released in
[`Metirionic/mars-cs-nrf54l`](https://github.com/Metirionic/mars-cs-nrf54l):

- **Latest firmware release:** [releases/latest](https://github.com/Metirionic/mars-cs-nrf54l/releases/latest)
  — includes `cs-ranging-firmware.zip` (one image for the initiator role, one
  for the reflector role, flashed individually).
- **Supported boards & antenna/path presets:** see the
  [hardware reference](https://github.com/Metirionic/mars-cs-nrf54l/blob/main/docs/hardware.md)
  for the live list of supported boards, board overlays, and the
  antenna/path ↔ preset mapping. New hardware support is added there over time.

## Features

- **Real-time monitoring** — observe live distance measurements with high precision.
- **User-friendly interface** — intuitive controls and visualizations.
- **Data export** — save measurement data in CSV or binary formats for further analysis.

## Support & contact

- **Support / licensing:** `contact@metirionic.com`
- **Contact page:** [metirionic.com/contact](https://metirionic.com/contact-2/)

---

© 2026 Metirionic GmbH — proprietary, all rights reserved.
Strehlener Straße 12–14, 01069 Dresden, Germany.

Bluetooth® is a registered trademark of Bluetooth SIG, Inc. MARS and the
Channel Sounding Evaluation Application are trademarks of Metirionic GmbH.