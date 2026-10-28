# Marketing Budget Optimization

**Domain:** Marketing

## Problem Statement

A company is spending heavily across multiple marketing channels, but management cannot determine which campaigns generate profitable customers. Develop an AI-driven system that analyzes campaign, customer, conversion and revenue data to identify inefficient spending, estimate campaign effectiveness, and recommend how the marketing budget could be reallocated.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: maximize contribution margin (not just revenue) from a fixed budget. Constraints: minimum brand spend and a maximum 25% budget shift per channel per month.
2. **Ingest:** Data Agent connects to ad accounts, web analytics, CRM and billing and loads daily spend, impressions, clicks, leads and orders.
3. **Prepare:** Standardize channel names and currencies, match orders to campaigns using UTM / click IDs, and attach product margin to each order.
4. **Analyze:** Compute CAC, ROAS, payback period and contribution margin per campaign; flag campaigns with payback longer than 12 months.
5. **Validate:** Attribution is imperfect, so estimate incremental impact with a marketing-mix model (weekly sales vs adstocked spend) and confirm key channels with a geo or holdout test.
6. **Reason:** Planner Agent (LLM) combines the results with business context (seasonality, launches) and proposes 2 to 3 allocation scenarios with expected margin and risk.
7. **Decide:** An optimizer selects the best scenario under the constraints; the marketing head approves (shifts under 10% may be auto-approved).
8. **Act:** Action Agent updates channel budgets through platform APIs or the budget sheet and logs each change with its reason.
9. **Pilot:** Run the new plan for 4 weeks in selected regions and keep comparable regions on the old plan.
10. **Improve:** Compare forecast and actual margin, update the model, and repeat the cycle every month.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
