# Atharva Mahajan

MS Mechanical Engineering at the **University of Michigan**, working on generative
models and closed-loop control for high-dimensional physical systems.

Most learned controllers ask one network to figure out both what a good state looks
like and how to reach it. My work separates those questions — let a generative model
say *where* a system should go, and let a small controller or a single forward pass
work out the rest.

## Research

**Policy-DRIFT: Dynamic Reward-Informed Flow Trajectory Steering** — *NeurIPS 2026*
First author. A conditional flow-matching model is trained over a multi-regime flow
manifold and steered by Terminal Reward Guidance to generate flow states that are both
physically realizable and reward-maximizing; a lightweight deep-RL policy then learns
only to track them. Reaches 48.95% drag reduction at Re_τ = 180 — 16.2% above the DRL
benchmark — at 37× lower actuation energy, running from wall-only sensing.
[Paper](https://arxiv.org/abs/2605.14022)

**CFD foundation models for geometry-generalizable flow prediction** — *in progress*
Conventional neural surrogates are retrained per geometry, which makes them useless for
exploring a design space. This work pretrains a surrogate that transfers across shapes,
pairing a joint-embedding predictive architecture (JEPA) with a mesh-density-preserving
geometry encoding. Preliminary results show zero-shot prediction on held-out geometries
with no fine-tuning.

**Upstream history in adverse-pressure-gradient turbulent boundary layers**
DNS/LES campaigns quantifying non-local memory effects via spectral densities,
Reynolds-stress budgets and β-evolution, from work at KTH.
[Int. J. Heat and Fluid Flow, 2025](https://www.sciencedirect.com/science/article/pii/S0142727X25002620)

## Code

[**cfm-airfoil-pressure**](https://github.com/atsmah123/cfm-airfoil-pressure) —
Reconstructs a full airfoil surface pressure field from as few as 5 pressure taps, with
calibrated uncertainty. A DeepSets encoder with learned positional attention handles
sensors in any arrangement; a FiLM-conditioned 1D UNet vector field does the generation.
183 Pa MAE at 10 taps on AirfRANS.

[**FoamSense**](https://github.com/atsmah123/FoamSense) —
Agentic AI for OpenFOAM: launching and managing simulations through natural language.

[**portfolio**](https://github.com/atsmah123/portfolio) —
Source for [atsmah123.github.io/portfolio](https://atsmah123.github.io/portfolio/).

## Background

Before the ML work: a 3D meshfree Euler solver in Fortran/CUDA driven to a 450× GPU
speedup, large-scale DNS on HPC systems, and co-founding Applied Aero Labs, where we
built India's first portable fan-array wind tunnel on a government innovation grant.

---

[Portfolio](https://atsmah123.github.io/portfolio/) ·
[LinkedIn](https://www.linkedin.com/in/atharva-mahajan-/) ·
atharvm@umich.edu
