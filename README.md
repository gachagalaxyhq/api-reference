# API Reference

> REST API documentation for Gacha Galaxy oracle data and prediction signals.

This repository describes the public-facing interfaces of the Gacha Galaxy protocol. The live product at [gachagalaxy.io/app](https://www.gachagalaxy.io/app) is built on top of the same data layer this API exposes.

---

## Status

The Gacha Galaxy API is currently in **closed beta**. Access is granted on request to:

- Enterprise data licensing partners
- Grading services and marketplace integrators
- Trading-bot developers and prediction-market builders
- Research desks and analytics platforms

The fully public, self-serve API is being rolled out as part of our Q3 2026 roadmap, alongside the Premium Oracle Tier launch.

**Request access:** matthew@gachagalaxy.io

---

## What the API exposes

### 1. Oracle data

- Live reference prices across 7 marketplaces (eBay, Collector Crypt, Courtyard, Phygitals, Beezie, Renaiss, Dyli)
- 20-minute snapshot history for any tracked card-grade tuple
- Fair Market Value (FMV) for grading-aware identities (PSA, BGS, CGC, SGC, Beckett, raw)
- Historical FMV time series

### 2. Mispricing Scanner

- Cards trading below FMV across all tracked marketplaces
- Ranked by spread percentage
- Filterable by marketplace, grading authority, grade, set, and spread threshold

### 3. Prediction signals

- Active signal list with target prices, expiries, and current resolution probability
- Historical signal outcomes for backtesting
- Programmatic signal creation (gated by $GG staking tier)

### 4. Card metadata

- Normalized card identities across marketplaces
- Grading authority and population data (where available)
- Set, card number, and variant resolution

---

## Endpoint structure (representative)

The API follows standard REST conventions. Example paths:


REST API documentation for Gacha Galaxy oracle data and prediction signals.
