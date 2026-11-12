# NEXUS-4D™ KOUTEI (工程) v7.0 | Ultimate Forensic, Quantitative Schedule Risk (QSRA) & 4D BIM Simulation Engine

**Shimizu Corporation (清水建設) Monozukuri Edition — Jakarta MRT Underground Package CP-202 (Station Box & Twin EPB TBM Drive Section)**  
**Standard Compliance:** AACE RP 29R-03 • DCMA 14-Point • PMI Practice Standard for Scheduling • FIDIC Red Book 1999 & 2017 • ISO 21502  
**Live Platform:** [https://nexus4d-koutei-planning-engine.vercel.app/](https://nexus4d-koutei-planning-engine.vercel.app/)

---

## Executive Engineering Overview

`NEXUS-4D™ KOUTEI` is an enterprise-grade, single-file (`index.html`), zero-latency (`<16ms` reactive in-memory recalculation) Project Controls & 4D Digital Twin Platform engineered specifically for complex mega-infrastructure projects: deep diaphragm-wall station box excavations, multi-tier top-down strutted slabs, and twin Earth Pressure Balance (EPB) Tunnel Boring Machine (TBM) drives.

Version **7.0** introduces five (5) high-level advanced civil engineering systems providing quantitative forensic risk verification, multi-method claim substantiation, equipment capacity leveling, tropical monsoon-haulage constraints, and full chronological 4D BIM construction sequence playback.

---

## The 5 Pillars of NEXUS-4D™ KOUTEI v7.0

### 🏛️ Pillar 1: Interactive 4D Time-Scrub Sequence Playback Controller (Three.js BIM)
- **Chronological Playback Dock (Tab 10 & 3D Viewport):**
  - **Time Scrubber Slider:** Ranges continuously from Project Commencement (`2026-01-05`, Day 0) through Data Date (`2026-11-03`, Day 303 / W43) to Baseline Completion (`2027-05-12`, Day 492 / W72).
  - **Transport Controls:** `⏮ Start`, `◀ Step Back (-7d)`, `▶ Play / ⏸ Pause`, `Step Forward (+7d) ▶`, `⏭ Finish`, `↺ Cut-Off W43`.
  - **Speed Multiplier:** Selectable `1x (1 day/sec)`, `2x`, `5x`, `10x`.
  - **Time Telemetry Display:** Active Simulation Date, Elapsed Calendar Days, Simulation Week (`W01` to `W72`), and Interpolated Cumulative Progress ($S_{\text{Act}}\%$ vs. $S_{\text{Plan}}\%$, $\Delta S\%$).
- **Dynamic 4D Construction Sequence Interpolation:**
  - **Sequential D-Wall Panels (DW-01 to DW-36 + Bulkheads):** Each panel transitions from unstarted translucent wireframe (`#1e293b`) $\to$ actively trenched glowing amber (`#f59e0b`) $\to$ cured concrete solid emerald (`#10b981`). Borehole BH-09 boulder zone panels freeze in crimson (`#ef4444`) during simulated ground holds.
  - **Top-Down Soil Excavation Block:** Semi-transparent earthen volume descends dynamically through 5 vertical tiers from surface ($0.0\text{m}$) down to base slab formation ($-24.5\text{m}$).
  - **Hydraulic Preloaded Struts & Slabs:** Strut Tier 1 ($-3.0\text{m}$), B1 Concourse Slab ($-8.0\text{m}$), Strut Tier 2 ($-10.0\text{m}$), B2 Intermediate Slab ($-16.0\text{m}$), Struts Tiers 3 & 4 ($-17.5\text{m}$ / $-22.0\text{m}$), and B3 Base Slab ($-24.5\text{m}$) automatically materialize as excavation elevations are cleared.
  - **Twin EPB TBM Advance Vectors:** TBM #1 *Sakura-1* (Northbound) and TBM #2 *Garuda-2* (Southbound) advance along the alignment at daily advance rates ($v_{\text{tbm}} \approx 10.8\text{ m/day}$), dynamically extruding precast segmental concrete lining rings ($\varnothing 6.65\text{m}$) and rotating cutterheads. Cross-Passage CP-01 mining triggers upon shield clearance.

---

### 🎲 Pillar 2: In-Browser Monte Carlo Quantitative Schedule Risk Analysis (QSRA)
- **Probabilistic PERT / Beta Duration Engine:**
  - Non-blocking in-browser Monte Carlo simulation executing **1,000 to 2,000 iterations** via asynchronous micro-batch scheduling.
  - Three-point duration modeling: Optimistic ($a = 0.85 \times D$), Most Likely ($m = D$), Pessimistic ($b = 1.40 \times D$, plus up to $+25$ days for high-risk geotechnical items).
  - Duration distribution: Standard Beta-PERT formulation ($\mu = \frac{a + 4m + b}{6}, \sigma = \frac{b - a}{6}$).
- **Output Analytics & Visualizations:**
  - **Cumulative Probability S-Band (P-Curves):** Real-time Chart.js canvas plotting deterministic finish alongside **P10**, **P50 (Median)**, **P80 (Target Commercial Commitment)**, and **P90 (Worst-Case)** completion dates.
  - **Contingency Buffer Calculation:** Explicitly isolates required schedule contingency (e.g. $+24$ Calendar Days between Deterministic Finish and P80).
  - **Tornado Sensitivity Chart:** Ranks top schedule drivers by **Criticality Index** (% of iterations on critical path) and **Cruciality Index** (Spearman rank correlation coefficient $r$ between activity duration and total project duration).

---

### ⚖️ Pillar 3: AACE RP 29R-03 Multi-Method Forensic Delay Analysis & FIDIC Claim Drafter
- **Multi-Method Forensic Delay Selector (Tab 8):**
  - **Method 1: Time Impact Analysis (TIA — Forward-Looking / AACE MIP 3.7):** Fragnet insertion immediately prior to delay events (e.g. BH-09 boulder lens $+24$ days critical path shift).
  - **Method 2: Contemporaneous Window Analysis (AACE MIP 3.3):** Month-by-month snapshots (`W40`, `W41`, `W42`, `W43`) isolating contractor pacing vs. owner critical delay variances.
  - **Method 3: Collapsed As-Built / But-For Analysis (AACE MIP 3.8):** Excises Employer Risk Events from the as-built network to prove completion date *but for* Employer actions.
- **Automated FIDIC Red Book Claim Notice Generator (Clause 20.1 / 8.4):**
  - Modal action generating formatted legal-grade contractual letters referencing FIDIC 1999/2017 Sub-Clause 20.1 (Contractor's Claims), Sub-Clause 8.4 (Extension of Time for Completion), and Sub-Clause 4.12 (Unforeseeable Physical Conditions).
  - Dynamic parameter binding: Certified delay days, affected WBS, Borehole BH-09 root cause, incurred standby costs, and 28-day notice rule verification.
  - Features 1-click **"Copy to Clipboard"** and **"Print Formal Notice (PDF)"**.

---

### 🚜 Pillar 4: Resource-Constrained Critical Path Method (RC-CPM) & Rig Conflict Detector
- **Heavy Equipment & Specialist Plant Resource Pool:**
  - Models site physical capacity: *Hydraulic Trench Cutter (Bauer BC 40)* [1 Rig], *Crawler Crane (Kobelco CKE2500G-2 250t)* [1 Unit], *Long-Reach Excavators (Komatsu PC300)* [2 Units], *Bentonite Slurry Desanding Plant* [1 Plant, $250\text{ m}^3/\text{hr}$].
- **Heuristic Leveling & Clash Detection Engine:**
  - Scans concurrent WBS activities; flags over-allocation clashes when concurrent demand exceeds fleet capacity.
  - Re-sequences activities using minimum-slack priority rules to compute the **Resource-Constrained Critical Path (RC-CPM)**, revealing artificial float created by classical CPM.

---

### 🌧️ Pillar 5: Jakarta Tropical Monsoon & Hydrological Curfew Modeling
- **Meteorological Rain Risk Matrix:**
  - 12-month historical rainfall profile for Jakarta (High Risk: Nov–Mar; Low Risk: May–Sep).
  - Calculates rain stoppage allowances and dynamically adjusts weather float buffers.
- **Dishub Muck Haulage Curfew Constraints:**
  - Models Central Jakarta municipal restrictions limiting heavy 10-wheel dump trucks along Jalan Gajah Mada / Hayam Wuruk to night-time hours (22:00–05:00).
  - Enforces hard disposal ceiling: **45 trips/night ($675\text{ m}^3/\text{night}$)**. Flags **"Muck Haulage Chokepoint"** and triggers optional temporary muck buffer pit mitigating off-site delays.
- **Piezometer Drawdown & Hydraulic Base Heave Interlock:**
  - Connects piezometer `PZ-02` pore water pressure to excavation depth.
  - Triggers **"Hydraulic Base Heave Warning"** and locks excavation gates when critical gradient exceeds safety limits ($i_{\text{crit}} > 0.85$ or drawdown $< -18.5\text{m}$).

---

## Complete Tab Directory

| Tab | Japanese Title | English Designation | Key Features |
|---|---|---|---|
| **Tab 1** | `1. 工程表` | Master Planning Grid | Excel-mode inline WBS grid, `<16ms` recalculation, QA/QC hold gates, Genba logs |
| **Tab 2** | `2. バナナ・出来高・QSRA` | Banana Envelope & QSRA | Dual S-Curve, EVM + Earned Schedule $SPI_{(t)}$, Monte Carlo QSRA (P10/P50/P80/P90), Tornado |
| **Tab 3** | `3. 時間・距離工程表` | Linear Scheduling (LSM) | Time-Chainage March Chart, TBM advance vectors ($10.8\text{ m/day}$), geotech anomaly overlay |
| **Tab 4** | `4. 4WLH & QC` | 4-Week Lookahead & LPS | 4WLH constraint make-ready, Last Planner PPC progression (`W40–W43`), RFV Pareto |
| **Tab 5** | `5. 資源・RC-CPM` | Plant, Labor & RC-CPM | Specialist equipment pool, direct labor histogram, heuristic RC-CPM clash leveling |
| **Tab 6** | `6. CPM Gantt & DCMA` | CPM Gantt & DCMA Audit | Dynamic Gantt bars, critical path logic, automated DCMA 14-Point schedule audit |
| **Tab 7** | `7. 地盤管理・環境制約` | Geotech & Environmental | Borehole N-SPT profiles, ERT anomalies, Jakarta monsoon matrix, Dishub curfew, PZ-02 heave lock |
| **Tab 8** | `8. 報連相・法務クレーム` | Hou-Ren-So & FIDIC Claims | Japanese governance, Hanko stamps, AACE RP 29R-03 3-method delay analysis, FIDIC claim notice drafter |
| **Tab 9** | `9. 改善シミュレーション` | Kaizen What-If Simulator | Schedule crashing, fast-tracking, 2nd rig mobilization, LD financial exposure comparison |
| **Tab 10** | `10. 4D Twin` | 4D BIM Simulation Engine | Three.js WebGL digital twin, 492-day time scrubber, transport buttons, excavation descent & TBM drives |

---

## Technical Stack & Standards

- **Architecture:** Zero-build standalone single-file cockpit (`index.html`) + mirrored `nexus4d-planning-engine/index.html`.
- **3D Engine:** Three.js r128 with WebGL renderer, OrbitControls, dynamic mesh scaling, and directional fill lighting.
- **Charts:** Chart.js 3.9 (Banana S-Curves, QSRA P-Curves, EVM histograms, March charts).
- **Styling:** Tailwind CSS CDN with Shimizu Obsidian Dark aesthetic (`#070b14`), Shimizu Blue (`#005bac`), Emerald (`#10b981`), Amber (`#f59e0b`), Crimson (`#ef4444`).
- **Standard Reference:**
  - AACE International Recommended Practice 29R-03 (Forensic Schedule Analysis)
  - Defense Contract Management Agency (DCMA) 14-Point Schedule Quality Assessment
  - Project Management Institute (PMI) Practice Standard for Scheduling
  - FIDIC Conditions of Contract for Construction (Red Book 1999 & 2017)
  - ISO 21502:2020 (Project, programme and portfolio management)

---

## Repository Structure

- [`index.html`](./index.html) — Production application (served at root `/` on Vercel & GitHub Pages).
- [`nexus4d-planning-engine/index.html`](./nexus4d-planning-engine/index.html) — Mirrored standalone build for Vercel production deployment.
- [`planning_engineer_platform_prd_uird.md`](./planning_engineer_platform_prd_uird.md) — Master PRD & UI Requirements Document.
- [`vercel.json`](./vercel.json) — Static deployment configuration.

---

*© 2026 Shimizu Corporation (清水建設株式会社) • Jakarta MRT Underground Package CP-202 Project Controls & 4D BIM Engineering Division.*
