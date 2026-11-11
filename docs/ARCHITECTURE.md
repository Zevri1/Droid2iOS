# Architecture notes

This document describes the research model, not a working port.

## Conceptual layers

1. **Hardware** — ARM64 CPU, memory, interrupt controller, timers, storage, display, GPU, and peripheral buses.
2. **Firmware and boot environment** — secure boot policy, bootloader behavior, platform initialization, and the handoff contract.
3. **Kernel** — XNU's Mach and BSD components plus platform-specific code and drivers.
4. **Kernel extensions / drivers** — device discovery, power management, storage, display, networking, and other I/O paths.
5. **Userspace** — libraries, daemons, launch services, graphics services, UI frameworks, and applications.

## Main compatibility boundaries

- An ARM64 instruction set match does not imply a platform port.
- A bootloader capable of loading a kernel does not provide the device tree, interrupt routing, or drivers the kernel expects.
- Linux drivers are not drop-in XNU drivers.
- Reaching a kernel prompt, serial log, or framebuffer is a limited boot experiment—not evidence of a complete operating system.
- A functional system requires a coherent driver stack, graphics, power management, security integration, userspace, and device-specific validation.

## Research workflow

1. Establish the exact hardware and firmware identity.
2. Locate authoritative documentation and source references.
3. Map required platform interfaces against available hardware descriptions.
4. Prefer emulation and static analysis before device experiments.
5. Record logs and classify each conclusion by evidence level.
6. Reassess feasibility before expanding the scope.

## Non-goals

This project does not claim to build or distribute Apple's iOS, bypass Apple's security mechanisms, or provide a daily-driver installation method.
