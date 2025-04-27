# GuardDuty Security Automation

This project demonstrates how to automate real-time security alerting in AWS by integrating Amazon GuardDuty, Amazon SNS, EventBridge, and Security Hub. It showcases a practical cloud security workflow where findings are detected, processed, and notified automatically without manual intervention.

## Tools Used
- **Amazon GuardDuty** — Threat detection service for identifying suspicious activity.
- **Amazon SNS (Simple Notification Service)** — Sends real-time alert notifications via email.
- **Amazon EventBridge** — Routes GuardDuty findings to trigger actions automatically.
- **AWS Security Hub** — Aggregates and prioritizes security findings across AWS services.
- **AWS Config** — Monitors and records resource configurations and changes.

## Project Highlights
- Detected potential threats using GuardDuty.
- Automated event-driven notifications with EventBridge and SNS.
- Subscribed to security alerts via email for immediate visibility.
- Aggregated findings in Security Hub for centralized security posture management.
- Enabled AWS Config to continuously monitor and record resource configurations.
- Simulated security findings to validate the alerting and response pipeline.

## Project Contents
- **SNS Topic:** `GuardDutyAlerts` for publishing GuardDuty notifications.
- **EventBridge Rule:** `GuardDutyFindingsToSNS` forwarding GuardDuty findings to SNS.
- **Security Hub Integration:** Centralized visualization of parsed findings.
- **Screenshots:** Included showing real-time alerts, event patterns, and security summary dashboards.

## Purpose
This project simulates a real-world cloud security monitoring environment where automated detection and rapid notification are critical. It demonstrates hands-on skills in threat detection, event automation, and cloud-native security operations — key competencies for cloud security engineering roles.

---

## Project previews

### Summary Dashboard
![Summary Dashboard](summary_dashboard.png)

### Findings by Severity
![Findings by Severity](findings_by_severity.png)

### Least Occurring Findings
![Least Occurring Findings](least_occurring_findings.png)

### Security Hub Findings View
![Findings](images_findings.png)


## Architecture Flow

'''
┌────────────────────────────┐
│    AWS GuardDuty            │
│ (Detects Threats)           │
└───────────────┬─────────────┘
                ↓
┌────────────────────────────┐
│    AWS EventBridge          │
│ (Triggers Rule on Findings) │
└───────────────┬─────────────┘
                ↓
┌────────────────────────────┐
│    AWS SNS Topic            │
│ (Publishes Notification)    │
└───────────────┬─────────────┘
                ↓
┌────────────────────────────┐
│    Email Alert to User      │
│ (Real-Time Notification)    │
└───────────────┬─────────────┘
                ↓
┌────────────────────────────┐
│    AWS Security Hub         │
│ (Centralized Findings View) │
└────────────────────────────┘
'''

---

> Built as part of a focused journey toward cloud security engineering excellence.  
> By Courtney Gonsalves.
