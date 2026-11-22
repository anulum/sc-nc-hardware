<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-HARDWARE — repository foundation
-->

# Architecture

## Current executable surface

The checkout contains:
- repository validation tooling;
- dedicated tests;
- workflow definitions;
- native documentation.

No domain component of SC-NC Hardware is implemented yet, and no code has moved here from SC-NeuroCore. The metadata keeps domain capabilities, claims and qualified record formats empty.

## Intended records

1. **Runtime binding:** How a compiled network is bound to a device: target, image, ports and limits.
2. **Trim table:** The calibration lookup table of a device, with its measurement source.
3. **Acquisition frame:** One frame read back from a device, with its timing, channels and integrity fields.

## Ownership

**This project owns** the planned SC-NC Hardware records and boundary rules.

**Owned elsewhere:**

| Responsibility | Owner |
|---|---|
| board and technology profiles | Circuit Technology |
| laboratory measurements | Circuit Lab |
| deployment packages | Deploy Pack |
| the public package, documentation and releases of the monolith | SC-NeuroCore |

## Interpretation

- **Devices.** No device behaviour is claimed without a device run that supports it.
- **Moves.** Code arrives only through SC-NeuroCore's split import gate, unit by unit; a planned move is not a moved capability.

Read [the documentation architecture](docs/ARCHITECTURE.md) for the planned records, rules and schema identifiers.
