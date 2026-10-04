# Technical Whitepaper — TELEPOT

**Model:** PAX L5 Narrow L2 General 27B
**Company:** Anticloud FZ LLE
**Upstream:** https://github.com/nickoala/telepot
**Category:** AUTOMOTIVE

## Abstract

This whitepaper describes the Anticloud integration of `TELEPOT` ((swap) Use: github.com/OBD-Monitor/obd-monitor — OBD2 car diagnostics)
with PAX L5 Narrow L2 General 27B, the offline-first AI model developed by Anticloud FZ LLE.
The integration produces a zero-cloud, single-binary deployment that exceeds upstream
capabilities while eliminating all third-party API dependencies.

## Technical Improvements

1. PAX L5 Narrow L2 General 27B local ADAS inference — in-vehicle, air-gapped
2. AIOSS tamper-evident vehicle event data recorder (EDR) chain
3. AES-256 encryption for all OBD/CAN bus data and trip logs
4. Single-binary ECU software package for production flash
5. Zero-cloud: all AI features operate without cellular connectivity
6. GPU/CPU equalizer: perception on embedded GPU, path planning on CPU
7. Open OBD-II interface: replaces proprietary diagnostic middleware
8. AUTOSAR-compatible module wrappers for OEM integration

## Architecture

See TECHNICAL/01_Architecture.md for the full architectural description.

## Benchmarks

See OFFICIAL_BENCHMARKS/04_PAX_Results.md for performance targets and measured results.