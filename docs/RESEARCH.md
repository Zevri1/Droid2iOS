# Research scope

## Questions

1. Which assumptions does XNU make about the platform during early boot?
2. Which ARM64 interfaces are generic, and which are Apple- or SoC-vendor-specific?
3. What firmware handoff and device-description data would a port need?
4. Which drivers are essential before a system can be considered minimally usable?
5. What can be demonstrated safely in emulation before touching physical devices?

## Evidence standard

Every claim should be classified as one of:

- **Documented** — supported by an authoritative source or source code.
- **Observed** — directly observed in a named experiment, with logs or artifacts.
- **Inferred** — a reasoned interpretation that still needs validation.
- **Unknown** — not yet established.

Record the device model, SoC revision, firmware/build, tool versions, exact steps, expected result, observed result, and relevant logs. Never turn an inference into a compatibility claim.

## Milestones

- Literature review and source mapping.
- Platform and boot-interface study.
- Emulation-first experiments.
- Hardware-specific feasibility assessment.
- Driver, userspace, security, and stability gap analysis.

## Scope boundary

This is not an iOS redistribution project. Do not upload proprietary Apple firmware, copyrighted system images, signing material, or device-owner data. A successful kernel boot alone is not evidence of a complete operating system.
