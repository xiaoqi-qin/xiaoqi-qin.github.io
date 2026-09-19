---
layout: page
title: Map-Conditioned Multi-View Interactive World Modeling
permalink: /projects/multi-view-interactive-world-model/
description: Action-conditioned multi-view first-person world modeling for highly dynamic interactive environments, in ongoing industry collaboration with YAHAHA.
importance: 1
category: research
---

**Ongoing industry collaboration with [YAHAHA](https://yahaha.com/) · Peking University · Advised by [Prof. Hao Tang](https://ha0tang.github.io/)**

[Project Page & Demos](https://zhengqisun.github.io/multiview-world-model/)

Developing a multi-view interactive world model that generates first-person videos from a shared 3D world state. The framework combines map-derived geometric conditioning and player-state information with a shared video diffusion model.

The CS:GO engine advances the shared world state, which is projected into each observer's view. Geometric and player-state conditions guide an adapted LingBot-World video model; each observer uses the same model weights and its own visual history.

## Demonstrations

The project page presents multi-view generation and autoregressive continuation. These demonstrations accompany our work on spatial grounding, cross-view consistency, and temporal stability.

## My contributions

- Designed a residual **Map Memory conditioning adapter** with LoRA to provide an explicit spatial reference across views.
- Built the end-to-end data and evaluation pipeline from raw gameplay recordings to synchronized multi-view clips and Map Memory conditions.
- Trained and debugged the 14B model on a **16× NVIDIA H200 GPU cluster**, diagnosing failures across the data, training, and systems stack.
- Developed evaluations for spatial grounding, cross-view consistency, world stability, and long-horizon behavior.

**Status.** This work is ongoing. The project page and selected demos are public; the manuscript is in preparation.
