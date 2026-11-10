# Cybersecurity Risk Analysis Using Wazuh, Kali Linux & Power BI

A practical cybersecurity monitoring case study showing how security events from a simulated SOC environment can be reviewed and communicated through a business-risk lens.

> **Project evidence:** This repository preserves screenshots from the original hands-on implementation. The original virtual machines and raw Wazuh alert exports are no longer available, so this is an evidence-led project case study—not a currently running lab or a fully reproducible deployment.

## At a glance

| Area | Details |
|---|---|
| Project type | Hands-on cybersecurity monitoring and risk analysis |
| Monitoring platform | Wazuh |
| Test environment | Kali Linux |
| Visualisation | Microsoft Power BI |
| Threat context | MITRE ATT&CK-related detections visible in Wazuh |
| Main focus | Event review, potential risk interpretation, and stakeholder communication |

## Project objective

The objective was to monitor security-related activity in a simulated environment, review selected alerts, identify patterns that may require investigation, and present security information in a form that is easier for non-technical stakeholders to understand.

The work connected technical monitoring with business questions: What happened? Why might it matter? Which activity may need further review? What management action could reduce exposure?

## Tools and technologies

| Tool | Role in the project |
|---|---|
| Wazuh | Security event monitoring and alert review |
| Kali Linux | Testing environment used to generate security-related activity |
| Power BI | Visual presentation of security monitoring information |
| MITRE ATT&CK | Context for interpreting selected detection techniques |

## Work performed

1. Set up a simulated security monitoring environment using Wazuh and Kali Linux.
2. Connected a Kali Linux agent to the Wazuh environment and reviewed its status.
3. Generated and observed security-related activity in the lab.
4. Examined authentication, privileged-user, system, and port-status events.
5. Reviewed selected detections with MITRE ATT&CK context.
6. Presented security information in a Power BI dashboard.
7. Interpreted the observations in terms of potential organisational risk and possible management actions.

## Selected observations visible in the archived screenshots

The original screenshots show the following values in their respective Wazuh views:

- **415 hits** in the Wazuh Discover view for the displayed time range.
- **61 events** in the Security Events dashboard view.
- **13 authentication successes** and **6 authentication failures** in the displayed security-event summary.

These are values from different interface views and/or visual summaries. They should not be added together or treated as one reconciled event total. The archived screenshots do not provide the underlying raw event export needed to independently recalculate them.

The Power BI screenshot also shows a dashboard built from a small displayed sample. It should be treated as a historical visualisation, not as a verified complete export of all 61 Wazuh events.

## Security areas reviewed

- Authentication successes and failures
- Password-guessing-related detections
- Privileged-user and sudo activity
- Port-status changes
- System and security event patterns
- Alert severity and agent-based distribution

## Business and risk interpretation

| Observation | Potential significance | Example follow-up |
|---|---|---|
| Repeated authentication failures | Possible password guessing or unauthorised access attempts | Review source, account, frequency, and authentication controls |
| Password-guessing-related detection | Potential account compromise risk | Review password policy, MFA coverage, and account protection |
| Privileged-user activity | Elevated access may increase incident impact | Validate whether the activity was authorised and review least privilege |
| Port-status change | May reflect an expected change or require investigation | Confirm the change against approved system and network activity |
| Recurring alerts | Could indicate persistent exposure or noisy detections | Group related alerts and prioritise investigation |

These are risk interpretations and suggested review actions, not confirmation that a breach occurred.

## Project documentation

- [Screenshot evidence](documentation/project-evidence.md)
- [Project methodology](documentation/methodology.md)
- [Findings and risk insights](documentation/findings-and-risk-insights.md)
- [Screenshots folder](screenshots/)

## Skills demonstrated

- Security event monitoring and review
- Authentication and privileged-activity analysis
- Basic threat-detection interpretation
- MITRE ATT&CK awareness
- Risk identification and prioritisation
- Power BI dashboard communication
- Translating technical observations into business language

## Scope, evidence and limitations

- The screenshots are historical evidence from the original practical project.
- The original VM files and raw Wazuh alert exports are currently unavailable.
- The archived screenshots do not establish that the lab is still operational.
- The displayed counts belong to their respective screenshots and have not been reconciled against raw data.
- No reconstructed or illustrative data should be mistaken for original Wazuh exports.
- This repository documents the work and available evidence; it does not claim a production SOC deployment or a confirmed real-world security incident.

---

**Project focus:** Connecting cybersecurity monitoring with business risk analysis and decision support.
