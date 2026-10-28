# Supply Chain Disruption Prediction

**Domain:** Operations

## Problem Statement

A manufacturing company frequently experiences production delays because disruptions in suppliers, inventory and transportation are identified too late. Develop an AI operations system that analyzes supplier, inventory, production and delivery data to identify emerging risks and recommend mitigation actions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: detect disruption risk 2 to 4 weeks ahead. Define disruption events and their service impact.
2. **Ingest:** Connect ERP, supplier scorecards, logistics tracking, production plans and external news and weather feeds.
3. **Prepare:** Build a supplier-material-week dataset with labeled disruption outcomes; engineer lead-time, stock-cover and backlog features.
4. **Analyze:** Train a risk classifier and an anomaly detector for lead-time shifts.
5. **Validate:** Use time-based splits, precision and recall, and agree alert thresholds with planners to avoid alert fatigue.
6. **Reason:** Monitoring Agent (LLM) reads supplier emails and news to detect events and maps them to affected materials.
7. **Decide:** Rank risks by probability x impact and choose mitigation (alternate source, safety stock, expedite) on cost and service trade-offs.
8. **Act:** Action Agent drafts purchase orders, sends supplier queries and notifies planners; low-cost actions may run automatically within limits.
9. **Pilot:** Start with critical suppliers and measure the stockouts avoided.
10. **Improve:** Log outcomes and retrain the model monthly.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
