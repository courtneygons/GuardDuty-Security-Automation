# GuardDuty-Security-Automation
Overview
This project demonstrates cloud security engineering fundamentals by detecting GuardDuty findings, sending real-time notifications through SNS (Simple Notification Service), and aggregating security alerts in AWS Security Hub. It simulates an automated threat detection and notification workflow commonly used in professional cloud security environments.

Tools and Services Used
AWS GuardDuty

AWS Simple Notification Service (SNS)

AWS EventBridge

AWS Security Hub

AWS Config

AWS Identity and Access Management (IAM)

Features
Detects suspicious or malicious activity using GuardDuty

Triggers real-time email notifications through SNS for security findings

Aggregates findings across AWS services in a centralized Security Hub dashboard

Parses raw event data for better visibility and incident triage

Demonstrates event-driven automation and secure architecture design

Project Contents
eventbridge_rule_config.json — Event pattern matching GuardDuty findings

sample_guardduty_finding.json — Example of raw finding data

screenshots/ — Visual examples of findings, email alerts, and dashboards

guardduty_summary.png

sns_email_alert.png

securityhub_dashboard.png

Purpose
The purpose of this project is to showcase the ability to:

Deploy secure and scalable cloud security monitoring

Understand and respond to real-world threat detection workflows

Automate alerts for faster incident response

Aggregate and analyze cloud security findings efficiently

Next Steps
Integrate Lambda functions for automatic remediation of critical alerts

Export findings to Splunk or a third-party SIEM

Develop fine-tuned IAM policies for advanced security hardening
