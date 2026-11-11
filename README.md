# Droid2iOS

**Experimental research into Darwin and XNU on Android hardware.**

Droid2iOS is an independent systems-research project exploring the technical distance between Android ARM64 devices and Apple's Darwin/XNU ecosystem. It is a research notebook—not an iOS port, installer, or promise of a usable iPhone-like operating system.

## Project goals

- Study Darwin and the XNU kernel architecture.
- Document ARM64 SoC, firmware, boot-chain, and device-tree assumptions.
- Map driver and hardware-support gaps (display, storage, USB, networking, GPU).
- Separate kernel-level proof of concept from userspace and daily-driver requirements.
- Publish evidence, reproducible experiments, and honest compatibility notes.

## Research areas

| Area | Focus |
|---|---|
| Darwin / XNU | Mach and BSD layers, kernel configuration, platform dependencies |
| ARM64 hardware | SoC layout, interrupts, memory map, peripherals |
| Boot chain | Firmware interfaces, boot stages, kernel handoff |
| Drivers / I/O | Display, storage, USB, network and device discovery |
| Graphics | GPU initialization, acceleration and display pipeline |
| Userspace | System services, libraries, UI and application compatibility |

## Reality check

Booting a kernel is not equivalent to running iOS. A useful system would also require compatible platform drivers, graphics, security integration, system services, userspace components, and extensive device-specific work. Apple's platform components and many device drivers are proprietary. This repository does not claim that any Android device can currently run full iOS as a daily driver.

## Repository layout

- `index.html` — static project website.
- `docs/RESEARCH.md` — research scope and evidence standards.
- `docs/COMPATIBILITY.md` — compatibility matrix template.

## Contributing

Research references, corrections, logs, and reproducible findings are welcome. Please include the exact device/SoC, software and firmware versions, steps taken, logs, expected result, and observed result. Do not report a feature as working without evidence.

## License

This project is licensed under the [Apache License 2.0](LICENSE).

## Links

- Source: https://github.com/Zevri1/Droid2iOS
