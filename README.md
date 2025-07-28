# MISP to Jira Automation

This project demonstrates how to automatically create Jira issues from threat intelligence data (IoCs) published in MISP.

## What It Does

When a new IoC is tagged in MISP for review, it triggers a webhook that sends the IoC data to Jira. A Jira Automation rule then creates a task in the SOC project for investigation.

## Project Structure

- `jira-automation/automation-rule.json` – Example Jira automation rule (Incoming Webhook → Create Issue)
- `misp-example-payload/ioc-webhook-payload.json` – Sample data payload sent from MISP

## Workflow

[MISP IoC] → [Webhook Trigger] → [Jira Automation] → [SOC Task]

## Security Note

This project is for demonstration only and **does not contain any sensitive credentials or production data**.
