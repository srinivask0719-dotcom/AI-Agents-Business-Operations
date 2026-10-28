# Inventory Optimization

**Domain:** Operations

## Problem Statement

A retailer simultaneously experiences stockouts for high-demand products and excess inventory for slow-moving products. Develop an AI inventory intelligence system that analyzes historical demand, seasonality, sales, inventory and supplier lead times to recommend inventory decisions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: meet the target service level with minimum inventory. KPIs: fill rate, inventory turns, stockout days.
2. **Ingest:** Pull POS sales, inventory, replenishment lead times, promotions, prices and supplier terms.
3. **Prepare:** Correct demand that was hidden by stockouts, classify SKUs (ABC-XYZ) and build calendar features.
4. **Analyze:** Forecast demand per SKU and location with probabilistic (quantile) forecasts.
5. **Validate:** Backtest with rolling windows and compare with a simple baseline using WAPE and bias.
6. **Reason:** Planner Agent explains exceptions: stockout risk, overstock and slow movers.
7. **Decide:** Compute safety stock and reorder points from the forecast distribution and lead-time variability, within order constraints (MOQ, shelf life, budget).
8. **Act:** Action Agent creates draft purchase orders and transfer proposals; buyers approve above value limits.
9. **Pilot:** Test on selected categories or stores.
10. **Improve:** Monitor service level and inventory days and recalibrate parameters.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
