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

SC-NC Hardware is being built as the hardware layer split out of SC-NeuroCore: the runtime bindings that connect a compiled network to a device, the trim tables that calibrate it, and the acquisition frames read back from it, through drivers, edge, analogue, memristive and spintronic paths. It imports SC-NC Core, SC-NC Data and SC-NC Compiler. Its current executable surface is repository validation tooling. It has no installed hardware runtime, device driver, acquisition reader or qualified record schema.

Read [Architecture](ARCHITECTURE.md), [validation tooling](validation-tooling.md), [data boundaries](THREAT_MODEL.md) and the [repository boundary decision](adr/0001-repository-boundary.md).
