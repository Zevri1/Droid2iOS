# Frequently asked questions

## Is Droid2iOS an iOS port?
No. This repository is an independent research notebook about Darwin, XNU, ARM64 hardware, firmware interfaces, and the engineering work a hypothetical port would require.

## Can I install iOS on an Android phone with this project?
No installer or usable iOS build is provided. The project does not claim that full iOS can currently run on Android devices.

## If XNU boots, does that mean the project works?
No. A kernel boot is only one milestone. A usable system would also need platform drivers, graphics, storage, networking, security integration, system services, and compatible userspace components.

## Why are drivers such a major obstacle?
Android devices use SoC- and vendor-specific hardware blocks. Their firmware, kernel interfaces, and drivers are not automatically compatible with Darwin or Apple's driver frameworks.

## Which devices are supported?
No device is currently declared supported. See [the compatibility matrix](COMPATIBILITY.md); entries should be added only when backed by reproducible evidence.

## How can I contribute?
Start with [CONTRIBUTING.md](../CONTRIBUTING.md). Useful contributions include primary-source references, careful architecture notes, reproducible observations, and corrections.

## Can I upload Apple firmware or system files?
No. Do not upload proprietary Apple firmware, copyrighted system images, signing material, or private device-owner data. See [the research scope](RESEARCH.md) and [security policy](../SECURITY.md).

## How should I report a result?
Include the exact device and SoC, firmware/build, tool versions, steps, expected and observed results, and relevant logs. Label conclusions as documented, observed, inferred, or unknown.
