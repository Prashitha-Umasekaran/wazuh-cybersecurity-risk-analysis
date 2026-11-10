# Findings and Risk Insights

## 1. Authentication Activity

The Wazuh environment displayed authentication successes and failures.

**Risk relevance:** Repeated authentication failures may indicate password-guessing attempts or unauthorised access attempts. Successful authentication should also be reviewed when it occurs in unusual circumstances.

**Business implication:** Unauthorised account access can expose confidential information and disrupt business operations.

## 2. Password-Guessing Detection

Password-guessing-related detections were observed in the security monitoring environment.

**Risk relevance:** These detections can indicate attempts to gain access through repeated password combinations.

**Business implication:** Weak passwords and inadequate access controls can increase the likelihood of account compromise.

## 3. Privileged User Activity

Sudo and authentication-related events were examined.

**Risk relevance:** Privileged activities require monitoring because administrator-level access can affect critical systems and configurations.

**Business implication:** Poor privileged-access management may increase the impact of security incidents.

## 4. Port-Status Changes

A port-status change alert was observed from the Kali Linux agent.

**Risk relevance:** Unexpected changes in network port status may require investigation to determine whether they are authorised.

**Business implication:** Unmonitored network changes may create additional exposure or service disruption.

## 5. Security Event Visibility

Wazuh provided visibility into security events, agent activity, and selected threat detections.

**Risk relevance:** Centralised monitoring helps security teams identify and investigate potentially suspicious activity.

**Business implication:** Better security visibility supports informed decisions about incident response and risk prioritisation.

## 6. Risk Management Perspective

The project demonstrated how technical security events can be interpreted through a business-risk perspective.

| Security observation | Potential risk | Suggested management action |
|---|---|---|
| Repeated authentication failures | Unauthorised access | Review authentication logs and account protection |
| Password-guessing detection | Account compromise | Strengthen password and access policies |
| Privileged activity | Misuse of elevated access | Review privileged account permissions |
| Port-status changes | Unauthorised network changes | Investigate unexpected configuration changes |
| Recurring security alerts | Persistent security exposure | Prioritise investigation and remediation |

## Conclusion

This project strengthened the understanding that cybersecurity monitoring is not limited to identifying technical alerts. Security events can also provide valuable information for evaluating organisational exposure, prioritising risks, and supporting business decisions.

**Evidence limitation:** These findings describe the activities and detections represented in the available project screenshots. They should not be interpreted as proof of a confirmed real-world security breach.
