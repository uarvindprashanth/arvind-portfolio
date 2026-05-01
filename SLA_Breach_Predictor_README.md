# SLA Breach Predictor

## Overview
The SLA Breach Predictor is a predictive analytics module designed to identify at-risk incidents before they violate Service Level Agreements (SLAs). Moving beyond traditional static ticket queues, this tool correlates historical incident data with real-time infrastructure health to generate dynamic breach probabilities.

## Core Capabilities
* **Data Integration:** Built to natively parse and analyze the UCI ServiceNow Incident dataset (comprising 24,918 real-world IT incidents), with support for custom CSV uploads.
* **Intelligent Risk Scoring:** Calculates risk based on ITIL parameters including priority, incident age vs. target, reassignment counts, and reopen rates.
* **Infrastructure Health Pulse:** Features a live background simulation (`INFRA_HEALTH`) that monitors infrastructure degradation. If system health drops below 70%, the risk score of all active incidents is automatically penalized by 15%, correlating system stability directly with SLA compliance.
* **AI Analyst Chat:** A context-aware Gemini 2.5 Flash agent capable of identifying root causes of breaches, suggesting prioritization strategies, and drafting executive summaries based on the loaded dataset.

## NOC Integration
Operators can use this dashboard to sort the "Top 20 at-risk incidents" and immediately deploy resources to tickets showing a high probability of failure, drastically reducing overall MTTR and penalty exposure.
