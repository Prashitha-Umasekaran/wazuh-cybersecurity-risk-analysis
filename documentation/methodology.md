# Project Methodology

## 1. Environment Setup

A simulated Security Operations Centre (SOC) environment was configured using Wazuh and Kali Linux.

Wazuh was used for security monitoring, while Kali Linux acted as the testing environment for generating security-related activities.

## 2. Agent Monitoring

The Kali Linux agent was connected to the Wazuh monitoring environment.

Agent connectivity and monitoring status were reviewed through the Wazuh interface.

## 3. Security Event Observation

Security events were examined through Wazuh, including:

- Authentication activity
- Password-guessing detections
- Privileged user activity
- Port-status changes
- System-related events

## 4. Threat and Risk Interpretation

Observed security events were reviewed to understand their potential significance.

MITRE ATT&CK-related detection information was used to provide context for selected security activities.

## 5. Data Visualisation

Security information was presented through a Power BI dashboard to make event patterns and risk indicators easier to understand.

The dashboard approach focused on:

- Event trends
- Alert severity
- Authentication activity
- Critical alerts
- Agent-based event distribution

## 6. Business-Oriented Interpretation

The final stage focused on communicating technical security information in a business-friendly way.

The objective was to help stakeholders understand security activity, identify areas requiring attention, and support risk-based prioritisation.

## Methodology Note

This document describes the workflow represented by the original project and its available screenshots. It is not a claim that the original virtual machines or raw event database are currently available.
