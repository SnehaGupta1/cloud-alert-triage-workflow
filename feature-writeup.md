## Proposed Features

The proposed alert triage workflow focuses on simplifying how security engineers review and resolve cloud security alerts. The design includes three core components.

**1. Centralized Alert Dashboard**
A dashboard that displays all alerts across cloud accounts in a single view. Alerts can be filtered by severity, resource type, cloud account, and status. This allows engineers to quickly identify high-priority alerts and focus on the most critical issues first.

**2. Alert Investigation View**
Selecting an alert opens a detailed investigation page that provides relevant context such as the affected resource, severity level, recent configuration changes, and related activity logs. Presenting this information in one place reduces the need to switch between multiple tools and speeds up the investigation process.

**3. Remediation and Response Actions**
The interface provides quick response options such as marking alerts as false positives, assigning the alert to a team member, applying suggested fixes, or closing resolved alerts. This helps security engineers take action quickly once the root cause has been identified.


## Feature Prioritization

The design prioritizes features that directly reduce investigation time and improve the efficiency of alert handling.

The **alert dashboard** is prioritized first because engineers must quickly identify which alerts require attention. Without a clear overview, important alerts may be missed.

The **investigation view** is the second priority since security engineers need immediate context to determine whether an alert represents a real threat. Providing relevant information in a single interface reduces the time spent gathering data from multiple sources.

Finally, **remediation actions** are included to streamline the response process. Once an alert is verified, engineers should be able to take action quickly without leaving the investigation workflow.

This prioritization ensures a smooth flow from **alert detection → investigation → response**, which mirrors the real workflow of security teams.


## Success Metrics

The effectiveness of the proposed solution can be measured using the following metrics:

* **Reduction in Mean Time to Investigate (MTTI)** for alerts
* **Reduction in Mean Time to Respond (MTTR)** to security incidents
* **Percentage of alerts resolved within defined response time targets**
* **Decrease in time spent gathering context during investigations**

These metrics help evaluate whether the system improves the speed and efficiency of security operations.


## (Bonus) Development Action Items

To implement this workflow, the following items needs to be discussed:

* Integration with cloud provider APIs to ingest security alerts
* Aggregation of activity logs and configuration change history
* Real-time alert updates within the dashboard
* Implementation of role-based access control for analysts
* Development of automated remediation suggestions for common misconfigurations
