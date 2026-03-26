# RBX1 Binder Dashboard (GEM x Adaptyv Competition)

Interactive dashboard for exploring ranked **de novo RBX1 binder designs** generated with **BoltzGen** and validated with **AlphaFold3 (AF3)** and **Boltz-2**.

The dashboard is designed for rapid inspection of candidate quality across multiple structural confidence metrics, consensus validation tiers, and sequence-level details.

## Live dashboard

https://carlos-laborda.github.io/rbx1-binder-dashboard/

## Overview

This project presents an interactive visualization layer for an RBX1 miniprotein binder campaign. The dashboard focuses on binders designed against **full-length RBX1 with 3 Zn²⁺ ions** and organizes candidates using cross-model validation signals from AF3 and Boltz-2.

The interface includes:

- tier-based filtering
- scatter plots comparing AF3 and Boltz-2 confidence metrics
- sortable ranking table
- per-candidate detail panel with sequence and interface metrics

## Validation tiers

Candidates are grouped into five confidence tiers:

- **Platinum** — strict high-confidence consensus between AF3 and Boltz-2
- **Gold** — strong consensus
- **Silver** — moderate consensus
- **Bronze** — single-model rescue
- **Fail** — poor confidence in both models

## Metrics shown

The dashboard highlights the main ranking signals used in the campaign:

- **AF3 iPSAE**
- **Boltz-2 iPSAE**
- **AF3 iPTM**
- **Boltz-2 iPTM**
- **BoltzGen RMSD**
- **H-bonds**
- **ΔSASA**
- designed amino acid sequence

## Usage

Open the live dashboard and:

1. filter by validation tier
2. sort candidates by AF3 or Boltz-2 metrics
3. click any design in the table or scatter plots
4. inspect sequence and interface-related details in the side panel

## Notes

This repository is intended as a lightweight presentation layer for ranked RBX1 binder candidates. It is optimized for interactive review of top designs rather than raw pipeline execution.
