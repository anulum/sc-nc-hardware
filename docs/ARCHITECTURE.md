<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-HARDWARE — repository foundation
-->

# Repository architecture

## Current executable tooling

**What it contains:** the repository's metadata, source-provenance, workflow, dependency-alignment, documentation, inventory and preflight controls.

**What each control does:** it inspects its fixed, declared local scope.

**What received metadata cannot do:** select another acceptance policy or grant domain authority.

Foundation qualification is in progress.

## Intended domain boundaries

| Record | Responsibility | Required evidence |
| --- | --- | --- |
| Runtime binding | How a compiled network is bound to a device: target, image, ports and limits | Binding checks against the target's profile before any load |
| Trim table | The calibration lookup table of a device, with its measurement source | Table checks against its calibration measurements |
| Acquisition frame | One frame read back from a device, with its timing, channels and integrity fields | Integrity and timing checks; a damaged frame is refused |

## Planned record schemas

- `sc_nc_hardware.runtime_binding.v1`
- `sc_nc_hardware.trim_lut_table.v1`
- `sc_nc_hardware.acquisition_frame.v1`

These are planned identifiers. None of them is registered or qualified here.

Read [validation tooling](validation-tooling.md) for the executable repository interfaces.
