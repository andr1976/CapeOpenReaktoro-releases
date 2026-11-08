# Reaktoro e-NRTL CESAR-1 CAPE-OPEN property package: portable distribution

Public download location for the portable, no-installer build of the CESAR-1 (aqueous AMP/piperazine)
electrolyte NRTL property package for CAPE-OPEN 1.1 simulators (Windows x64), built on
[Reaktoro](https://reaktoro.org). The release artifacts are produced by the build workflow of the source
repository.

Landing page: <https://andr1976.github.io/CapeOpenReaktoro-releases/>

## Download

Get the latest `ReaktoroCO-CESAR1-Portable-<version>.zip` from the **[Releases](../../releases)** page.
Each release also carries the source of the modified Reaktoro library it is built with.

## What it is

- One CAPE-OPEN 1.1 property package, **Reaktoro eNRTL (AMP-PZ-CO2-H2O)**, with the fixed compound slate
  H2O, CO2, AMP, PZ, N2, O2 (N2 and O2 as Henry-law inerts).
- Electrolyte NRTL model of the CESAR-1 solvent with published parameters; vapour-liquid equilibrium,
  enthalpy, density, viscosity and surface tension for process simulation of CO2 capture.
- Example COFE flowsheets (absorber, absorber with desorber, lean vapour compression, pilot-plant cases)
  in [`Flowsheets/`](Flowsheets).

## Install (per user, no administrator rights)

1. Extract the ZIP to a permanent folder, e.g. `C:\ReaktoroCO-CESAR1`.
2. Close the simulator and run **`Install.bat`** (run it again if you move the folder).
3. Optional: `Test-Package.ps1` checks the installation without a simulator.
4. Select **Reaktoro eNRTL (AMP-PZ-CO2-H2O)** in the simulator.

To uninstall, run **`Uninstall.bat`** and delete the folder.

## Prerequisites

- Windows 10/11 x64 with .NET Framework 4.8
- Microsoft Visual C++ 2015-2022 x64 runtime
- A 64-bit CAPE-OPEN 1.1 simulator, e.g. [COCO/COFE](https://www.cocosimulator.org) with ChemSep

## Citation

Any publication, presentation, report or other dissemination of results obtained with the package shall
cite the paper given in [`citation.json`](citation.json) and in [`LICENSE.txt`](LICENSE.txt) (clause 4).
Please also cite Reaktoro: A. M. M. Leal, Reaktoro: An open-source unified framework for modeling
chemically reactive systems, https://reaktoro.org (2015).

## Licence

Freeware under the conditions in [`LICENSE.txt`](LICENSE.txt), provided as is without warranty. The
third-party libraries in the bundle keep their own licences (LGPL v2.1 for Reaktoro and its companions,
MIT, MPL 2.0); see `THIRD-PARTY-NOTICES.txt` and `SOURCES.txt` in the ZIP.

## Support

Questions and bug reports: [issue tracker](../../issues).
