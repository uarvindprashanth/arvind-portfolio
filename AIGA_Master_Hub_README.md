# AIGA Portal (Autonomous Identity & Governance Agent)

## Overview
The AIGA Portal serves as the unified Command Center for Enterprise IT Operations. It seamlessly integrates four critical layers of IT service management: Governance, Predictive Analytics, Tactical Remediation, and Executive Reporting. 

By utilizing a Single Page Application (SPA) architecture, the portal provides a "Single Pane of Glass" experience. It shares a centralized AI intelligence layer powered by Gemini 2.5 Flash, allowing operations teams to shift from reactive monitoring to proactive, business-aligned IT management.

## System Architecture
* **Frontend Design:** Custom HTML/CSS/JavaScript interface with a high-contrast theme optimized for 24x7 NOC environments.
* **Modular Integration:** Uses iframe-based isolation to load specific modules while maintaining a persistent navigation layer.
* **Centralized Authentication:** Employs browser `localStorage` to securely share the `GEMINI_API_KEY` across all operational tabs, ensuring a frictionless user experience.
* **AI Engine:** Google Gemini 2.5 Flash API for low-latency, high-context analysis and code generation.

## Module Ecosystem
1. **Governance Hub:** Strategic oversight of ITIL maturity and ISO/SOC2 compliance.
2. **SLA Predictor:** Data-driven risk analysis and infrastructure health monitoring.
3. **Ops Runbook:** Tactical incident resolution and automated script generation.
4. **Executive View:** Business-value translation and financial risk assessment.

## Usage Instructions
Launch `aiga_master_hub.html` in any modern web browser. Upon first load, the system will prompt for a Gemini API key. Once provided, the AI Agent Status will show as "Connected," unlocking deep analytical capabilities across all modules.
