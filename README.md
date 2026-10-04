<p align="center">
  <img src="docs/banner.svg" width="980" alt="TAKSI — worldwide mobility platform, powered by OMNICOR">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Go-1.24-00ADD8?logo=go&logoColor=white" alt="Go 1.24">
  <img src="https://img.shields.io/badge/Flutter-stable-02569B?logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/license-proprietary-C42B2B" alt="License: proprietary">
  <img src="https://img.shields.io/badge/status-pre--launch-orange" alt="Status: pre-launch">
</p>

> **Public product showcase.** TAKSI is a proprietary platform — this repository presents the product, its architecture and economics. The source code lives in a private monorepo.

A worldwide ride-hailing, freight, and loaders platform — passenger app, driver app, dispatch backend, and admin console in one codebase.

**Core economics:** drivers keep 100% of the fare with instant payout on ride completion. The platform monetizes through a flat shift subscription instead of per-ride commission. Passenger fares are set by a proprietary dynamic pricing engine tuned per city and vehicle class.

---

## Architecture

<p align="center">
  <img src="docs/architecture.svg" width="980" alt="TAKSI platform architecture">
</p>

## How the money flows

<p align="center">
  <img src="docs/economics.svg" width="980" alt="Money flow — passenger pays, driver receives 100%, platform earns on shift subscription">
</p>

## Screenshots

<p align="center">
  <img src="docs/demo.gif" width="236" alt="App preview — live flow">
  <img src="docs/screenshots/01_welcome.png" width="236" alt="Welcome">
  <img src="docs/screenshots/02_order.png" width="236" alt="Ride order">
</p>
<p align="center">
  <img src="docs/screenshots/04_ride.png" width="236" alt="Ride in progress">
  <img src="docs/screenshots/05_driver.png" width="236" alt="Driver navigation">
  <img src="docs/screenshots/06_cabinet.png" width="236" alt="Driver account — earnings & stats">
</p>

## What's inside

<p align="center">
  <img src="docs/features.svg" width="980" alt="Platform capabilities — ride engine, driver model, pricing, payments, geo, compliance, AI support, admin, i18n, cargo">
</p>

## OMNICOR ecosystem integration

<p align="center">
  <img src="docs/omnicor.svg" width="980" alt="OMNICOR L2 OMNI tokenomics — buyback-burn cycle and staged emission">
</p>

<p>
  <img src="docs/brand/omni-token-dark.svg" width="48" align="right" alt="OMNI token">
  TAKSI is wired into the <a href="https://github.com/AI-Omnicor">OMNICOR</a>
  network — an independent L2 blockchain with the OMNI utility token.
  The integration is dormant by default and activates purely by
  configuration; the platform ships and operates fully on fiat rails.
</p>

Every completed ride books a rouble-denominated buyback obligation —
a public debt ledger with no OMNI price locked in. A Safe periodically
burns the matching OMNI on L1: **100% of the taxi buyback is destroyed**
(public `totalBurned` counter). Protocol fees flow through an immutable
FeeSplitter — **70% burned, 30% to the Treasury** on every `sweep()`.
Emission is staged — 10% circulating, 20% founder allocation, 70%
ecosystem reserve released in ~40 quarterly tranches over 10 years;
unclaimed tranches burn automatically. Supply only ever shrinks.
Custody is split between hot executor wallets and cold corporate
addresses whose keys never touch the server.

## Engineering

<p align="center">
  <img src="docs/engineering.svg" width="980" alt="Repository layout, security model, build & test">
</p>

## License

Proprietary — All Rights Reserved.

---
