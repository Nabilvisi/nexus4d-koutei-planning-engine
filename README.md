# NEXUS-4D™ KOUTEI (工程) | Enterprise Project Controls & Linear Scheduling Engine (v5.2 • PE26/QC26 ENGINE)

**Shimizu Corporation (清水建設) Monozukuri Edition — Jakarta MRT Underground Package CP-202 (Station Box & TBM Drive Section)**

`NEXUS-4D™ KOUTEI` is an enterprise-grade, zero-latency (`<16ms` reactive recalculation) Project Controls, Automated MS Project Ingestion Middleware, & Interactive Linear Scheduling Platform built for heavy underground civil infrastructure, deep diaphragm-wall excavations, and Twin EPB TBM bored tunneling.

---

## Core Engineering Capabilities

0. **MS Project Unified Ingestion & 3-Tier Approval Pipeline (`v5.2 データ連携・三段階承認ゲート`)**
   - Keeps **Microsoft Project (`.mpp` / `.xml` / `.xlsx` / `.csv`)** as the single source of scheduling truth in the field while acting as an **Automated Ingestion Middleware**, **Fail-Closed QA/QC Gate**, and **3-Tier Digital Approval Engine** (*Genba Site Engineer → PE26/QC26 Audit → Department Head Release*).
   - Zero double-entry: automatically pushes validated progress deltas (`Δ%`) into the Master WBS Control Grid, recalculates Executive KPI cards (`PHYSICAL %`, `WEEKLY CUT-OFF`, `SPI`), updates the `S-Curve / Banana Curve`, and syncs to Shimizu Cloud Data Lake & Power BI with an immutable `SHA-256` audit lineage.

1. **Master Planning Grid / Excel-Mode (`1. 工程表`)**
   - Live inline-editable WBS spreadsheet (`Tab` / `Enter` / `Arrow` navigation) eliminating Excel–Primavera P6 friction.
   - Instant recalculation of durations, weighted progress (*Bobot %*), weekly cut-off telemetry ($\Delta_{\text{week}}$), and EVM metrics in `<16ms`.
   - **Anzen Dai-Ichi (安全第一) & QA/QC Hold Points:** Hard progress locks when `RFI HOLD` or `GEO HOLD` gates are active, plus 1-to-1 **Genba-Shugi (現場主義)** daily inspector log drill-downs.

2. **Banana Curve Envelope & EVM Suite (`2. バナナ曲線・出来高管理`)**
   - Dual-baseline S-Curve Envelope plotting Early Start ($S_{Early}$) vs. Late Start ($S_{Late}$) based on CPM Total Float, tracking cumulative Earned Value ($S_{Act}$) and Kaizen recovery projections.
   - Full Earned Value Management telemetry: $BAC$, $PV$, $EV$, $AC$, $SV$, $CV$, $SPI$, $CPI$, $TCPI$, and $EAC$.

3. **Linear Scheduling Method (LSM) / Time-Chainage March Chart (`3. 時間・距離工程表`)**
   - Spatial-temporal tunneling & excavation chart across $\text{STA } 14+000$ to $\text{STA } 15+500$, visualizing D-Wall trenching, Top-Down Station Box excavation, and TBM #1 / TBM #2 advance vectors ($v_{tbm} = 12.5\text{ m/day}$, $\eta_{down} = 18\%$) against subsurface boulder anomaly zones.

4. **4-Week Rolling Lookahead (4WLH) & Make-Ready Constraints (`4. 4WLH & QC`)**
   - Tracks Shop Drawings, Permits to Work / KYT (*Kiken Yochi*), PE26/QC26 RFI sign-offs, and rebar/segment readiness across `W42–W45`.

5. **Manpower & Heavy Equipment Histogram (`5. 資源・重機稼働`)**
   - Direct labor histogram (Budgeted vs. Mobilized across 6 specialist trades) and live plant telemetry (*Hydrofraise Bauer BC 40*, *Kobelco CKE2500G-2 250t Crane*, *Komatsu PC300*, *Bentonite Slurry Desanding Plant*).

6. **Interactive CPM Gantt (`6. CPM Gantt`)**
   - Dynamic horizontal Gantt bars with Early Start/Finish, Total Float tails, Critical Path highlighting, and progress fill.

7. **Geotechnical Subsurface Risk Gates (`7. 地盤管理`)**
   - Borehole (`BH-01` to `BH-14`) N-SPT profiles, ERT resistivity anomalies, inclinometer lateral deflection (`INC-04`), settlement markers (`SM-08`), piezometers (`PZ-02`), and 3-tier excavation permit sign-off.

8. **Hou-Ren-So (報・連・相) Escalation & Ringisho (稟議書) Consensus (`8. 報連相・稟議書`)**
   - Structured Japanese governance for variance reporting (*Hōkoku*), lateral trade coordination (*Renraku*), director consultation (*Sōdan*), and interactive *Hanko* (印鑑) consensus approval stamps.

9. **Kaizen Recovery / What-If Simulator (`9. 改善シミュレーション`)**
   - Interactive simulation sliders comparing Schedule Crashing (24/7 night-shift muck haulage), Fast-Tracking (off-site strut prefabrication), and 2nd Rig Mobilization against Liquidated Damages (LD) exposure.

10. **One-Click A4 Landscape Print / PDF Executive 1-Pager**
    - Built-in `@media print` stylesheet formatting the entire cockpit into a clean 1-page steering committee summary.

---

## Repository Structure

- [`index.html`](./index.html) — Standalone production application (served at root `/` on Vercel & GitHub Pages).
- [`nexus4d-planning-engine/index.html`](./nexus4d-planning-engine/index.html) — Mirrored standalone build per PRD Section 4 specification.
- [`planning_engineer_platform_prd_uird.md`](./planning_engineer_platform_prd_uird.md) — Complete Product Requirements Document (PRD) & UI Requirements Document (UIRD).
- [`vercel.json`](./vercel.json) — Zero-config Vercel static deployment routing.
