# NEXUS-4D™ KOUTEI (工程) v8.0 | 5D Commercial BIM, Multi-Baseline Drift, Multi-Calendar & Subsurface Lithology Mega-Cockpit

**Shimizu Corporation (清水建設) Monozukuri Edition — Jakarta MRT Underground Package CP-202 (Station Box & Twin EPB TBM Drive Section)**  
**Standard Compliance:** FIDIC Red Book 1999/2017 Sub-Clauses 14.3, 8.4, 4.12 • AACE RP 29R-03 • DCMA 14-Point • buildingSMART BCF 2.1 • ISO 19650 • ISO 21502  
**Live Production Platform:** [https://nexus4d-koutei-planning-engine.vercel.app/](https://nexus4d-koutei-planning-engine.vercel.app/)  
**Repository:** [https://github.com/Nabilvisi/nexus4d-koutei-planning-engine](https://github.com/Nabilvisi/nexus4d-koutei-planning-engine)

---

## Executive Engineering Overview

`NEXUS-4D™ KOUTEI v8.0` is an enterprise-grade, single-file (`index.html`), zero-latency (`<16ms` reactive in-memory recalculation) Project Controls, Forensic & 5D BIM Simulation Engine. Engineered specifically for complex mega-infrastructure projects, it unites **Time (4D)**, **Money (5D)**, **Contractual Governance**, and **Subsurface Geological Physics** for the Jakarta MRT Underground Package CP-202 (Harmoni – Sawah Besar – Mangga Besar) and Phase 2A Corridor.

---

## The 5 Master Engineering Systems of NEXUS-4D™ KOUTEI v8.0

### 💰 System 1: 5D Cost-Loaded Schedule & FIDIC Sub-Clause 14.3 IPC Certification Engine
- **Contract Bill of Quantities (BoQ) Data Binding:**
  - Full relational binding of all WBS activities to contractual BoQ items totaling exactly **BAC = IDR 420.00 Billion**:
    - `BoQ-01`: Diaphragm Wall (D-Wall) Concrete Grade B45 (14,200 m³ @ IDR 2.85 M/m³ = IDR 40.470 B)
    - `BoQ-02`: High-Tensile Deformed Rebars Grade SD490 (4,650 Tons @ IDR 16.50 M/Ton = IDR 76.725 B)
    - `BoQ-03`: Deep Excavation & Mucking (182,000 m³ @ IDR 385,000/m³ = IDR 70.070 B)
    - `BoQ-04`: Precast Segmental Tunnel Rings (2,450 Rings @ IDR 85.0 M/Ring = IDR 208.250 B)
    - `BoQ-05`: Guide Wall, Traffic Decking & Deep Dewatering Curtains (Lump Sum = IDR 12.485 B)
    - `BoQ-06`: Cross-Passage Excavation, Ground Freezing & MEP First-Fix (Lump Sum = IDR 12.000 B)
- **FIDIC Red Book Sub-Clause 14.3 Interim Payment Certificate (IPC #11) Engine:**
  - Automated certified monthly billing ledgers:
    - **Gross Certified Value of Works:** $\sum (\text{Actual Qty}_i \times \text{Unit Rate}_i) = \text{IDR } 188.37\text{ B}$ (44.85% EV).
    - **Advance Payment Amortization:** 10% gross value deduction until initial 10% mobilization advance (IDR 42.00 B) is recovered (-IDR 18.84 B recovered to date).
    - **Retention Money Withholding:** 5% retention capped at 5% of Contract Sum (-IDR 9.42 B withheld to date, capped at IDR 21.00 B).
    - **Net Certified Payable:** Current net payable **IDR 12.86 Billion** printable with traditional Japanese Hanko Inkan seals (所長, 監理検認, MRTJ承認).
- **Working Capital & Overdraft S-Curve:**
  - Interactive Chart.js canvas tracking **Cash In** (Certified IPC receipts assuming a 30-day Employer payment cycle) vs **Cash Out** (Cumulative Actual Field Costs AC).
  - Highlights **Maximum Working Capital Deficit / Overdraft Exposure** (Peak: **-IDR 28.40 B** at Month 8) and **Financial Break-Even Date** (**Month 13 / January 2027**).
- **3D Capital Intensity Heatmap (5D BIM):**
  - Toggle in Tab 10 (4D Digital Twin):
    - **Dark Blue ($< \text{IDR } 10\text{ B}$):** Decking, Struts, Instrumentation Sensors.
    - **Violet ($\text{IDR } 10\text{–}30\text{ B}$):** Intermediate Slabs S2, Bulkheads, Station Box Roof S1.
    - **Gold ($> \text{IDR } 50\text{ B}$):** Heavy Base Slab B3 and Twin TBM Segmental Tunnel Rings.

---

### 📊 System 2: Multi-Baseline Schedule Diff & Revision Audit Ledger
- **Multi-Baseline Snapshot Repository:**
  - **Baseline Rev 0 (Target):** Original Contract Award Baseline (Data Date 2025-11-15, Contract Completion 2027-05-11).
  - **Baseline Rev 1 (EOT-1):** Approved Extension of Time after BH-09 Boulder Encounter (2026-08-20, +42 Days EOT, Completion 2027-06-22).
  - **Baseline Rev 2 (Target Recovery):** Active Working Schedule (Data Date 2026-11-03, Target Completion 2027-05-25 with Kaizen mitigation).
- **Schedule Drift & Logic Manipulation Auditor:**
  - Automated variance comparison:
    - Identifies logic softening (e.g., FS-0d $\to$ SS+15d on WBS-2.3 to WBS-3.1).
    - **Float Erosion Radar:** Detects activities where Total Float eroded by $> 10$ days without physical progress (WBS-3.2 eroded 18d $\to$ 0d; WBS-4.2 eroded 28d $\to$ 14d).
- **Visual Split-Gantt Bar Diff:**
  - Dual stacked bars in Tab 6 (CPM Gantt): Upper Bar (Baseline Rev 0 Target in grey translucent), Lower Bar (Active Forecast color-coded by Critical Path & Float with actual progress fill and slip delta badges).

---

### 📅 System 3: Multi-Calendar & Cultural Workforce Shift Engine
- **Three Dedicated Project Calendars:**
  - **Calendar A: 24/7/365 Continuous Underground:** Applied to TBM Shield Driving (WBS-4.1, 4.2), Ring Erection, and Bentonite Slurry Desanding.
  - **Calendar B: 6-Day Surface (Mon–Sat):** Applied to Station Box Diaphragm Wall (WBS-2.1, 2.3), King Post Driving (WBS-3.1), and Surface Grouting (Sundays strictly non-working per AMDAL environmental noise permits).
  - **Calendar C: 5-Day Technical / Engineering:** Applied to QA/QC Submittals, RFI Reviews, and Shop Drawing approvals.
- **"Lebaran Mudik" (帰省) Workforce Drop Simulator:**
  - Models nationwide Eid al-Fitr holiday in Indonesia (March 24 to April 7, 2027 / 14-day window):
    - Simulates a **75% reduction in available direct labor** (Workforce drops from 420 to 105 personnel).
    - Mucking productivity drops by 75% (820 m³/d $\to$ 205 m³/d) and TBM advance drops to 3.2 m/d.
    - Automated early warning alert when critical path pouring (WBS-5.1 Base Slab) overlaps with the holiday window.
    - **Kaizen Mudik Mitigation Plan:** 1-click activation of pre-cast buffer rings and double overtime incentive.

---

### 🗺️ System 4: Linear Scheduling 2.0 (LSM) with Subsurface Lithology & Slurry Heatmap
- **Subsurface Lithological Stratigraphy Cross-Section:**
  - High-density 2D geological backdrop along alignment chainage (STA 14+000 to STA 15+500 and elevation 0.0m to -30.0m):
    - **Stratum 1 (Topsoil & Alluvial Fill):** Brown (0.0 to -4.5m, N=8–14)
    - **Stratum 2 (Marine Silty Clay):** Dark Slate Blue (-4.5 to -14.0m, N=12–18, high plasticity)
    - **Stratum 3 (Dense Volcanic Aquifer Sand):** Amber/Gold (-14.0 to -22.0m, N=32–48, water ingress risk)
    - **Stratum 4 (Basalt Boulder / Cobble Lens):** Crimson Hatch Pattern (STA 14+780 to 14+860 at BH-09, N > 60)
  - Station Box excavation outline at STA 14+000 to 14+350 down to -24.5m with twin TBM tubes at -16.5m depth.
- **TBM Slurry Support Pressure ($P_{face}$) Safety Envelope:**
  - Real-time curve tracking required EPB chamber face pressure ($2.4 \text{ to } 2.8\text{ bar}$) vs overburden depth ratio ($C/D = 2.48$).
  - Dynamic safety boundaries: $P_{collapse} = 1.95\text{ bar}$ (Active collapse / settlement limit) and $P_{heave} = 3.15\text{ bar}$ (Passive blowout limit) along Jalan Gajah Mada.

---

### 📑 System 5: buildingSMART BCF 2.1 Exporter & Schedule Fragility Radar
- **buildingSMART BCF (BIM Collaboration Format) 2.1 Exporter:**
  - 1-click **"Export BCF Issue Ticket"** on any WBS row or 3D element.
  - Generates standard BCF 2.1 XML payload: Camera XYZ viewpoint, GUID, WBS Code, Assigned Subcontractor, Priority, and RFI / Hold status.
  - Direct import compatibility into Autodesk Navisworks, Revit, Solibri, and BIM Track.
- **Schedule Fragility Radar (Predictive Early Warning Index):**
  - Composite formula:
    $$SFI = 0.35 \times (\text{Float Burn Rate}) + 0.35 \times (\text{Open RFI Lag Days}) + 0.30 \times (\text{Heavy Rig Over-Allocation})$$
  - Risk Thresholds:
    - $SFI < 40$: Robust (Green)
    - $40 \le SFI \le 70$: Vulnerable (Amber)
    - $SFI > 70$: High Fragility / Imminent LD Threat (Crimson Pulsing)
  - **Fragility Radar Widget in Top Command Header** alerting management **14 days prior** to critical milestone breach with full diagnostic modal.

---

## Technology Stack & Architecture

- **Core Runtime:** Pure Standalone Vanilla HTML5 / ES2022 / WebGL. Zero npm build step or server dependency.
- **Styles:** Tailwind CSS (Dark Mode Obsidian Palette) with custom Japanese Monozukuri engineering accents.
- **3D Digital Twin:** Three.js r128 with OrbitControls, custom procedural geometries, multi-tier shader interpolation, and 5D cost intensity mapping.
- **Charts & Physics:** Chart.js 4.4.1 (Banana S-Curves, EVM histograms, Overdraft curves, Monte Carlo probability distribution).
- **Standards:** buildingSMART BCF 2.1, ISO 19650, FIDIC Red Book Sub-Clauses 14.3, 8.4, 4.12, DCMA 14-Point, AACE RP 29R-03.
