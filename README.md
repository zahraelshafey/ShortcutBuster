# ShortcutBuster

**Detecting and fixing "shortcut learning" in image classification models.**

> A Graduation Project at the **Digital Egypt Pioneers Initiative (DEPI)** · Track: `Microsoft Machine Learning Engineer`

---

## Overview

Many AI models reach high accuracy for the wrong reasons. Instead of learning the real concept, they pick up an easy *shortcut* (for example, the image background). Such models look reliable on paper but fail when the shortcut disappears.

**ShortcutBuster** is a tool that detects this behavior, identifies what the model relies on, measures the damage, and retrains the model to learn the right thing.

## The Problem

A classifier trained to separate **waterbirds** from **landbirds** may simply look at the background: water means waterbird, land means landbird. When a waterbird appears on land, the model gets it wrong.

## How ShortcutBuster Works

| Step | What it does |
|------|--------------|
| 1. Detect | Finds out that the model is relying on a shortcut |
| 2. Identify | Shows what the model depends on (e.g. the background) |
| 3. Measure | Measures how much accuracy drops when the shortcut fails |
| 4. Fix | Retrains the model so it learns the correct feature |

## Practical Plan

- Use the **Waterbirds** dataset (birds placed on water / land backgrounds)
- Train a simple image classification model
- Visualize where the model looks in each image
- Change the background and measure the accuracy
- Retrain and compare results **before vs. after**

## Project Status

| Phase | Status |
|-------|--------|
| Planning & Management | In progress |
| Literature Review | In progress |
| Requirements Gathering | In progress |
| System Analysis & Design | Planned |
| Implementation | Planned |
| Testing & QA | Planned |
| Final Presentation & Reports | Planned |

## Repository Structure

```
ShortcutBuster/
├── README.md
├── docs/        # Project documentation (PDFs, Gantt chart)
├── src/         # Source code
├── tests/       # Test cases and scripts
└── assets/      # Images and diagrams
```

## Documentation

Project documents are available in the [`docs/`](docs/) folder.

## Team

| Name | Role |
|------|------|
| `Zahra Ahmed Hamada Ahmed` | Team Leader |
| `Rana Haithem` | `Member` |
| `Menna Gharib` | `Member`|
| `Sondos Abdo` | `Member` |

**Technical Instructor:** `Mostafa Mohamed`

## References

- Geirhos et al., *Shortcut Learning in Deep Neural Networks*
- Sagawa et al., *Distributionally Robust Neural Networks* (Waterbirds / Group DRO)
- Selvaraju et al., *Grad-CAM: Visual Explanations from Deep Networks*
