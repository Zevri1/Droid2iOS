# Contributing to Droid2iOS

Thanks for helping improve the research. Contributions should prioritize accuracy, reproducibility, and clear separation between evidence and speculation.

## Good contributions

- Primary-source references about Darwin, XNU, ARM64, firmware, and hardware interfaces.
- Corrections to technical explanations.
- Reproducible experiments with logs and exact version details.
- Improvements to documentation, accessibility, and the project website.

## Before opening a pull request

1. Search existing issues and discussions to avoid duplicate work.
2. Keep changes focused and explain the engineering reason.
3. Do not include proprietary Apple firmware, operating-system images, signing keys, or private device data.
4. Do not claim device compatibility without reproducible evidence.
5. Update the relevant documentation when behavior or conclusions change.

## Experiment report format

- Device and exact model:
- SoC / revision:
- Firmware and software versions:
- Tools and versions:
- Steps performed:
- Expected result:
- Observed result:
- Logs / evidence:
- Known limitations:

## Evidence labels

Use **Documented**, **Observed**, **Inferred**, or **Unknown** as defined in [the research guide](docs/RESEARCH.md). A kernel boot or early-boot display is not equivalent to a usable operating system.
