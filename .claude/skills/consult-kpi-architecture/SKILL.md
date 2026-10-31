---
name: consult-kpi-architecture
description: Use to design a KPI system — value-driver trees linking operational metrics to financial outcomes, KPI definitions, targets, owners, data sources, cadence and dashboard/review design.
---

# KPI Architecture

Owner: Operations & Transformation Partner, with the Corporate Finance Partner checking the links to the financial outcomes. Follow consult-operating-system.

## Method
1. **Start from the outcome.** Pick a top metric, such as ROIC, EBITDA, free cash flow or the strategic goal.
2. **Build a value-driver tree** that is MECE and arithmetic: each branch must multiply or add up to its parent. For example: EBITDA = volume × (price − variable cost) − fixed cost. Volume then splits into customers × share of wallet, and so on. Go down to the operational levers people control, such as yield, uptime, OTIF, DSO, win rate and loading per kWh.
3. **Select the KPIs.** Choose 10–15 per level of management, and mix leading and lagging indicators. Every KPI must be controllable by its owner, measurable from existing data, and tied to a decision.
4. **Write a definition card for each KPI:**
   - name;
   - formula;
   - unit;
   - data source and system;
   - frequency;
   - owner;
   - baseline;
   - target and its glide path;
   - thresholds (green, amber, red);
   - the action to take when red.
5. **Cascade the KPIs** across group, region, function and team so they stay consistent and do not double-count.
6. **Review cadence:**
   - weekly operational;
   - monthly performance;
   - quarterly strategic.
   For each, set the dashboard layout, which shows exceptions first, and the meeting agenda.

## Output
- A driver tree (mermaid or indented).
- A KPI dictionary.
- A targets table.
- A dashboard wireframe.
- The review-cadence calendar.

OCSiAl: reconcile with the FP&A Board & Management Reporting persona and 07 Plant KPIs, and with SAP data availability.
