<p align="center">
  <img src="https://raw.githubusercontent.com/arxynehq/.github/main/profile/assets/logo.png" alt="Arxyne" width="280"/>
</p>

<h3 align="center">The AI Harness for Cyber-Physical Products</h3>

<p align="center">
  <em>From design intent to digital twin — one continuous engineering loop.</em>
</p>

---

## What is Arxyne?

Arxyne makes AI safe and useful for engineering. We embed AI into real engineering workflows — with governance, provenance, and physics validation built in — on a composable system built on **OpenUSD**.

We don't build vehicles, robots, or aircraft. We give engineering teams **AI they can actually trust** — from first sketch to every mile driven or hour flown.

## The Problem

Engineering complex physical products is broken:

- **Siloed tools** — CAD, simulation, test, manufacturing, and operations all speak different languages
- **PLM knows parts, CAE knows physics, and no one speaks both** — part identity lives in Teamcenter / Windchill / 3DEXPERIENCE; simulation results live on file shares; they never meet. When a part changes, an engineer manually figures out which sims to re-run.
- **No single source of truth** — design intent lives in slides, simulation results live in folders, real-world data lives in the cloud
- **Manual loops** — an engineer changes a parameter, waits hours for simulation, reads results, repeats
- **No AI adoption path** — engineers can't use AI because there's no governance, no provenance, no way to trust the output

The result: 3–5 year development cycles, billions in validation costs, armies of CAE ops staff stitching the gaps by hand, and products that never learn from the real world.

## The Platform

Arxyne closes the loop across the entire product lifecycle:

```
Design Intent → Simulation → Validation → Manufacturing → Digital Twin → Optimisation
      ↑                                                                        ↓
      └────────────────────── Closed Loop ─────────────────────────────────────┘
```

**OpenUSD Digital Twins** — Every product is a composable, versionable, diffable digital twin with 6 composition layers spanning design through real-world operation.

**AI-Assisted Engineering** — AI agents handle orchestration, validation, and traceability — running solvers, assessing results, benchmarking competitors — so engineers can focus on decisions, not plumbing. Governed and auditable.

**Multi-Domain** — Ground vehicles, aircraft, any cyber-physical product. Same pipeline, same gates, different physics. Proven on DrivAer sedan (Cd=0.275 vs published 0.258) and ONERA M6 swept wing (Cd=0.017, 127s solve).

**Containerised Solvers** — CFD, structural, dynamics — any solver runs in Docker, returns structured data. The platform orchestrates; solvers are pluggable.

**Deploy Anywhere** — Runs on any infrastructure: workstation, data centre, or NVIDIA DGX. Deploy on-premise to keep IP secure, or scale to cloud when needed.

**Unified Part & Change Management (UPCM)** — Every part is a first-class citizen with stable identity, revision lineage, content hash, and an automatic dependency graph into simulation results. When a part changes, Arxyne knows *exactly* which sims are invalidated and why. PLM knows parts. CAE knows physics. Arxyne is the only place they meet.

## Why OpenUSD?

USD isn't just for movies anymore. It's the composition layer for the physical world:

- **Hierarchical** — vehicles, aircraft, robots all decompose into assemblies and parts
- **Non-destructive layers** — design, simulation, manufacturing, and operations overlay without conflicts
- **Native part identity** — parts are USD prims; revisions are sublayers; supersedence is composition strength. No separate part database to keep in sync.
- **Industry momentum** — NVIDIA Omniverse, Apple Vision Pro, Pixar, and now industrial digital twins
- **Diffable** — compare your product against any competitor using auto-discovered shared attributes

## Architecture

<p align="center">
  <img src="https://raw.githubusercontent.com/arxynehq/.github/main/profile/assets/architecture.svg" alt="Arxyne Architecture" width="680"/>
</p>

## Status

- ✅ OpenUSD digital twin schema (51+ typed attributes, 6 composition layers)
- ✅ Agentic CFD pipeline (OpenFOAM in Docker, autonomous agent loop)
- ✅ Multi-domain: DrivAer sedan (Cd=0.275, 6.6% vs published) + ONERA M6 wing (Cd=0.017)
- ✅ Product-type-aware sanity gates + auto-baseline management
- ✅ Automated target assessment with product-agnostic competitor diffing
- ✅ Convergence-based early stopping + stall detection
- ✅ Provenance, validation, and engineering gate system
- ✅ Solver registry (6 physics domains — aero active, 5 planned)
- ✅ "Ask Programme X" — conversational AI queries across the digital twin
- ✅ NVIDIA Omniverse integration (USD scene graph + auto-launch)
- ✅ 867 tests (unit + integration, CI on every push)
- ✅ 3 products: DrivAer Baseline, ARX Type-X (ONERA M6 wing), Ahmed Body
- ✅ AI surrogates (NVIDIA DoMINO NIM — 30s inference vs 6hr CFD, validated ≤1.5%)
- 🔜 Multi-physics (vehicle dynamics, structural)
- 🔜 Manufacturing compilation layer

## The Vision

Today: an engineer tells an agent "assess this wing at Cd ≤ 0.02" and the platform runs the loop — simulation, assessment, reporting — autonomously.

Tomorrow: every complex machine has a living digital twin that learns from the real world and feeds improvements back into the next design. From prototype to production to operation to next generation — one continuous thread of data.

**We're making AI safe and useful for physical engineering.**

---

<p align="center">
  <strong>Arxyne</strong><br/>
  <em>arx</em> (Latin: citadel) · <em>-yne</em> (modern, technical)<br/><br/>
  <a href="https://arxyne.com">arxyne.com</a> · <a href="mailto:chris@arxyne.com">chris@arxyne.com</a>
</p>
