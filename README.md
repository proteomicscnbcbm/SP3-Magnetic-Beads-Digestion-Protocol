# Automated Magnetic Bead-Based Digestion Protocols for Opentrons OT-2

![OT-2](docs/images/ot2_robot.png)

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Reproducibility](https://img.shields.io/badge/automation-OT2-blue.svg)]()
[![Proteomics](https://img.shields.io/badge/workflow-proteomics-purple.svg)]()
[![Bead-based digestion](https://img.shields.io/badge/method-magnetic_beads-orange.svg)]()

---

## 📌 Overview

This repository provides a fully automated and reproducible implementation of **magnetic bead-based proteomic digestion** using **hydroxyl-functionalized beads** on the **Opentrons OT-2** platform.

The workflow is based on and extends:

> **Ciordia S. et al. (2024)**  
> *Refinement of paramagnetic bead-based digestion protocol for automatic sample preparation using an artificial neural network*  
> *Talanta* — PMID: 38569368

---

## 🎯 Goals

- Offer an **open-source, reproducible** digestion workflow
- Minimize manual handling time through **full automation**
- Reduce tip and reagent usage via **alternate-column design**
- Provide a modular breakdown of the digestion protocol optimized for robotic execution

---

## 🧬 Protocol Structure

The workflow is split into **three operational modules** due to pipette tip constraints and to support up to **6 alternate columns (even-numbered positions)**:

1. **Protein Binding to Hydroxyl Magnetic Beads**
2. **Washing & Interferent Removal**
3. **Enzymatic Digestion & Peptide Elution**

This modular approach enables:

- Tip saving strategy  
- Deck space optimization  
- Full digestion reproducibility across batches  

---

## 📁 Repository Structure

├── protocols/
│ ├── part1_binding.py
│ ├── part2_washing.py
│ └── part3_digestion.py
├── deck_layouts/
│ └── deck_map_2_4_6_columns.pdf
├── consumables/
│ └── consumables_list.md
├── docs/
│ ├── optimization_notes.md
│ ├── ANN_parameters.md
│ └── troubleshooting.md
├── notes/
├── LICENSE
└── README.md
