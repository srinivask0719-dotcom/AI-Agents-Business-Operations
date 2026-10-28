# Employee Attrition Root-Cause Intelligence

**Domain:** HR

## Problem Statement

Employee turnover has increased significantly, creating recruitment costs and operational disruption. Develop an AI system that integrates employee performance, workload, compensation, absenteeism, overtime, engagement and training data to identify organizational factors associated with attrition and recommend evidence-based retention interventions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. **Define:** Objective: reduce regretted attrition in critical roles. Ethical limits: anonymized data, HR-only access, and no automated decisions about individuals.
2. **Ingest:** Collect HRIS, payroll, promotion, performance, attendance, overtime, engagement and exit data.
3. **Prepare:** Pseudonymize employee IDs and build point-in-time features: pay vs market, time since promotion, overtime trend, manager changes.
4. **Analyze:** Fit an attrition model (survival analysis or gradient boosting) and identify department and manager hotspots.
5. **Validate:** Test on a later period, check fairness across gender, age and location, and review drivers with explainability tools.
6. **Reason:** Insight Agent (LLM) codes exit interviews and survey comments into themes and links them to the quantitative drivers.
7. **Decide:** Propose team-level actions (pay review, workload, career paths, manager coaching), compare cost with replacement cost; HR head approves.
8. **Act:** Action Agent schedules stay interviews, creates review tasks and assigns follow-ups to HR business partners.
9. **Pilot:** Apply to selected teams and compare with similar teams over 3 to 6 months.
10. **Improve:** Track attrition, engagement and cost, then update the drivers and interventions.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
