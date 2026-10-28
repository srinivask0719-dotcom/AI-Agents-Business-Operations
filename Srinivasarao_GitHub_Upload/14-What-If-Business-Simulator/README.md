# What-If Business Simulator

**Domain:** Business Analytics

## Problem Statement

Management wants to increase sales by 20% but does not know whether existing employees, inventory, production capacity and logistics can support the additional demand. Build an AI scenario-analysis system that simulates business consequences of different strategic decisions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: assess whether +20% sales is feasible and profitable. Set scenario assumptions: timeline, product mix and price.
2. **Ingest:** Collect sales, capacity, staffing, inventory, lead-time, logistics and cost data.
3. **Prepare:** Build a driver-based operating model linking units sold to labor, materials, machine time and deliveries; calibrate it with history.
4. **Analyze:** Forecast baseline demand and run +10%, +20% and +30% scenarios.
5. **Validate:** Back-test the model on past growth periods and run a Monte Carlo simulation for demand and lead-time uncertainty.
6. **Reason:** Scenario Agent (LLM) converts a manager's question into model inputs and explains the results.
7. **Decide:** Identify bottlenecks and compare mitigation plans (hire, extra shift, outsource, buffer stock) on profit, risk and speed.
8. **Act:** Action Agent exports the chosen plan and creates tasks for owners.
9. **Pilot:** Phase the growth plan with checkpoints.
10. **Improve:** Compare actual with simulated results and recalibrate the model.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
