# Material Complexity Visualizer

**Real-time shader complexity analysis for the Unreal Engine Material Editor**

Material Complexity Visualizer (MCV) helps developers identify and understand shader complexity hotspots directly inside the Material Editor — at the wire and node level — without needing RenderDoc, shader compilation logs, or GPU profilers.

![Unreal Engine](https://img.shields.io/badge/Unreal%20Engine-5.0%20–%205.7-blue?logo=unrealengine&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Win64-lightgrey)
![License](https://img.shields.io/badge/License-Marketplace-green)

---

## Overview

MCV colors every wire in your material graph with a heatmap gradient (white → violet → magenta → red) that represents estimated shader cost. Cheap connections stay white; expensive ones turn red. Cost numbers are printed directly on wires, and a floating **Legend** shows the current scale. A **Hotspots** panel lists the most expensive nodes so you can jump straight to what matters.

### Key Features

- **Heatmap Wires** — every connection in the material graph is colored by its estimated cost
- **Cost Labels** — numeric cost values displayed directly on wires
- **6 Analysis Modes** — Total, ALU, Samples, Dependent, Flow, Feature Penalty
- **3 Normalization Modes** — Percentile 95, Global Max, Absolute (fixed budgets)
- **Interactive Tooltip** — hover any wire to see a full cost breakdown with a gradient bar, per-mode metrics, and optimization hints
- **Legend Panel** — floating color scale with dynamic tick labels that update with the current mode and normalization
- **Hotspots Panel** — ranked list of the most expensive nodes with click-to-navigate
- **Material Function Support** — full inline traversal of material functions with correct cost propagation
- **Customizable Gradient** — two built-in presets (Neon, Base) or define your own 5-stop gradient
- **Configurable Weights** — adjust how much each metric contributes to the Total score
- **Non-Destructive** — never modifies your materials; editor-only, zero runtime overhead

---

## Supported Versions

| Unreal Engine | Status |
|:---:|:---:|
| 5.0 | ✅ Supported |
| 5.1 | ✅ Supported |
| 5.2 | ✅ Supported |
| 5.3 | ✅ Supported |
| 5.4 | ✅ Supported |
| 5.5 | ✅ Supported |
| 5.6 | ✅ Supported |
| 5.7 | ✅ Supported |

**Platform:** Windows 64-bit (Win64)

---

## Installation

### From Fab / Epic Marketplace

1. Purchase or add **Material Complexity Visualizer** from the [Fab Marketplace](https://www.fab.com/)
2. In the **Epic Games Launcher**, go to your Library → Vault
3. Click **Install to Engine** and select your UE version
4. Open your project — the plugin is automatically enabled

### Manual Installation

1. Download or clone this repository
2. Copy the `MaterialComplexityVisualizer` folder into your project's `Plugins/` directory:
