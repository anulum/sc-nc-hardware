<!--
SPDX-License-Identifier: AGPL-3.0-or-later
Commercial license available
© Concepts 1996–2026 Miroslav Šotek. All rights reserved.
© Code 2020–2026 Miroslav Šotek. All rights reserved.
ORCID: 0009-0009-3560-0851
Contact: www.anulum.li | protoscience@anulum.li
SC-NC-HARDWARE — repository foundation
-->

# SC-NC Hardware

SC-NC Hardware is being built as the hardware layer split out of SC-NeuroCore: the runtime bindings that connect a compiled network to a device, the trim tables that calibrate it, and the acquisition frames read back from it, through drivers, edge, analogue, memristive and spintronic paths. It imports SC-NC Core, SC-NC Data and SC-NC Compiler. This checkout contains repository validation tooling and documentation only. Full foundation qualification is in progress. There is no installed hardware runtime, device driver, acquisition reader or qualified record schema.

**What does not exist yet:**
- any code moved from SC-NeuroCore;
- a registered runtime record schema;
- an installed hardware runtime, device driver or acquisition reader.

## Boundary

**What this project owns:**

| Record | Scope |
|---|---|
| Runtime binding | How a compiled network is bound to a device: target, image, ports and limits |
| Trim table | The calibration lookup table of a device, with its measurement source |
| Acquisition frame | One frame read back from a device, with its timing, channels and integrity fields |

**Static imports:** only SC-NC Core, SC-NC Data and SC-NC Compiler.

**Records read without importing their code:** SC-NC Bridges, Sim Real Witness, AER Link Witness, Loop Timing Witness, Deploy Pack and Flight Recorder read this repository's records.

**Records it reads without importing their code:** those of SC-NC Data, SC-NC Compiler, Bitstream Evidence CI and Circuit Lab.

**Code planned to move here from SC-NeuroCore,** package by package, when SC-NeuroCore's split import gate allows it: `hardware`, `drivers`, `edge`, `analog_bridge`, `memristor`, `spintronic`, `comm` and `hypervisor`.

**Explicit non-claims and operating boundaries:**
- No board, device, sensor or chip is attached or driven by this foundation.
- A binding or trim table describes a device; it does not prove the device behaves as described.

## Current tooling

Repository controls inspect:
- metadata and source attribution;
- workflows and dependency alignment;
- native documentation and repository inventory;
- preflight orchestration.

Metadata declares architecture-only maturity with empty implemented domain capability and claim inventories.

- Use the exact environment in [Contributing](CONTRIBUTING.md).
- Full CI and preflight belong in CI or in an explicitly admitted pre-push environment.
- See [Validation](VALIDATION.md) for the maintained validation scope.

## Intended evidence

Every future record will carry its source and environment digests, its numeric formats where it has them, and its explicit verification boundary. None of the planned record schemas is registered or qualified by this foundation.

## Documentation and support

Read [Architecture](ARCHITECTURE.md), [support](SUPPORT.md), [security reporting](SECURITY.md) and [citation metadata](CITATION.cff).

**Not claimed:**
- a hosted service, released package or DOI;
- a public CI status;
- a performed simulation, hardware measurement or benchmark result.

## Licence

Source is licensed under [AGPL-3.0-or-later](LICENSE). A commercial licence is available through the contact in [NOTICE](NOTICE.md).

![ANULUM](docs/assets/anulum_logo_company.jpg)

![Fortis Studio](docs/assets/fortis_studio_logo.jpg)

## Text and data mining reservation
The rightsholder, Miroslav Šotek (ANULUM), expressly reserves the use of the
works in this repository for text and data mining, including the collection of
this content for, and its use in, training, fine-tuning or evaluating machine
learning and artificial intelligence models, in accordance with Article 4(3) of
Directive (EU) 2019/790 and the national provisions transposing it.

No permission for such use has been granted beyond what the licence in
`LICENSE` grants. This reservation does not change that licence: uses the
licence permits remain permitted on its terms, including its attribution and
share-alike conditions.

Reservation made on 2026-11-22. Requests for permission: contact the
rightsholder through the contact listed in this repository.
