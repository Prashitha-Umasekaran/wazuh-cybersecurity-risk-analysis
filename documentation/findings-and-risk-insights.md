# Findings and Risk Insights

This document interprets the security activity visible in the archived Wazuh screenshots. It distinguishes observed interface information from potential risk implications.

## 1. Authentication activity

The archived Security Events view displays **13 authentication successes** and **6 authentication failures** for the period shown in that screenshot.

**Risk relevance:** Repeated authentication failures may indicate password-guessing attempts or other unsuccessful access attempts. Successful authentication is not inherently suspicious; it should be reviewed in context, especially if the account, source, time, or behaviour is unusual.

**Business implication:** Account compromise can expose confidential information and disrupt business operations.

**Suggested review:** Correlate failures by account and source, check whether the activity is expected, and review password and multi-factor authentication controls.

## 2. Password-guessing-related detection

A password-guessing-related detection is visible among the Wazuh/MITRE ATT&CK-related evidence.

**Risk relevance:** This type of detection may indicate repeated attempts to discover valid credentials.

**Business implication:** Weak credentials or insufficient account protections can increase the likelihood of unauthorised access.

**Suggested review:** Validate the alert details, affected account, source, frequency, and whether any subsequent successful login is related.

## 3. Privileged-user activity

Sudo and authentication-related events were examined.

**Risk relevance:** Privileged activity deserves attention because administrator-level access can change configurations, access sensitive information, or affect critical services.

**Business implication:** Inadequate privileged-access management may increase the impact of an incident.

**Suggested review:** Confirm that the activity was authorised, review the account's need for elevated privileges, and retain appropriate audit logs.

## 4. Port-status changes

A port-status change alert from the Kali Linux agent is visible in the archived evidence.

**Risk relevance:** A port-status change may be expected during testing or maintenance, but an unexpected change may require investigation.

**Business implication:** Unreviewed network changes can affect service availability or create unintended exposure.

**Suggested review:** Compare the event with approved testing or change activity and validate the affected host and service.

## 5. Security-event visibility and displayed counts

The archived screenshots show different values in different Wazuh views:

- Wazuh Discover: **415 hits** for the displayed time range.
- Security Events dashboard: **61 events** in the displayed view.
- Authentication summary: **13 successes** and **6 failures**.

These figures are reported separately because the screenshots represent different views, filters, or summaries. They are not a single reconciled dataset and must not be summed or interpreted as mutually exclusive categories without the original event export.

The Power BI screenshot contains a small displayed sample of records. It is useful as evidence of the visualisation work, but it does not establish that the dashboard contains every event represented in the Wazuh views.

## 6. Risk interpretation

| Security observation | Potential risk | Suggested management action |
|---|---|---|
| Repeated authentication failures | Unauthorised access attempts | Review authentication logs, account protection, and MFA |
| Password-guessing-related detection | Potential account compromise | Validate the detection and strengthen credential controls |
| Privileged activity | Misuse or overuse of elevated access | Verify authorisation and apply least privilege |
| Port-status changes | Unexpected network or service exposure | Investigate against approved change records |
| Recurring security alerts | Persistent exposure or detection noise | Correlate related alerts and prioritise investigation |

## Conclusion

The project demonstrates how security monitoring information can be interpreted beyond the technical alert itself. Reviewing authentication activity, privileged actions, and port-status changes can help identify questions for investigation and support risk-based prioritisation.

**Evidence limitation:** These are observations and interpretations based on the available historical screenshots. They do not prove that a real-world breach occurred, and the underlying raw Wazuh records are not available for independent validation.
