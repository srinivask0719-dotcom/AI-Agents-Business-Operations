# Customer Churn & Retention Intelligence

**Domain:** Marketing

## Problem Statement

A subscription business is experiencing increasing customer churn despite continued marketing expenditure. Develop an AI system that identifies behavioral patterns associated with churn, segments at-risk customers, determines potential causes, and generates personalized retention strategies.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: lower voluntary churn within a retention budget. Define churn (no renewal 30 days after expiry) and the maximum cost per saved customer.
2. **Ingest:** Pull subscription, product usage events, billing, support tickets and survey scores.
3. **Prepare:** Build a point-in-time feature table (only data from before each prediction date, to prevent leakage): usage trend, recency, failed payments, tickets, tenure.
4. **Analyze:** Train a gradient-boosting churn model and a survival model to estimate when churn is likely; use a time-based test split.
5. **Validate:** Check recall in the top risk decile, probability calibration and lift, and compare results across plans and segments.
6. **Reason:** Planner Agent (LLM) summarizes the top drivers (SHAP) and ticket themes per segment and retrieves the retention playbook (RAG).
7. **Decide:** Use uplift logic: rank customers by expected saved value minus offer cost so only persuadable customers are targeted.
8. **Act:** Action Agent sends personalized offers or outreach through the CRM; large offers need manager approval.
9. **Pilot:** Hold out a random 10% of selected customers as a control group to measure true uplift.
10. **Improve:** Track net retention gain, retrain monthly and stop actions that do not beat the control.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
