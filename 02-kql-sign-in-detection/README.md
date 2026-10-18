# Project 02 — Repeated Sign-in Failure Detection with KQL

## Objective

Use Kusto Query Language (KQL) to review sign-in failures, summarize repeated activity, and identify accounts that experience a high number of failures in a short time window.

## Skills demonstrated

- Filtering data by time
- Filtering failed versus successful sign-ins
- Selecting useful fields with `project`
- Aggregating events with `summarize`
- Grouping by account, IP address, and time window
- Applying a configurable detection threshold

## Requirements

The examples below use the Microsoft Entra ID `SigninLogs` table in a Log Analytics workspace. Available fields and result-code formats can vary by connector and workspace, so confirm your table schema before running the queries.

## Query file

Open `queries/sign_in_detection.kql` for three investigation queries.

## Tuning notes

- The sample threshold of five failures in 15 minutes is a starting point, not a universal rule.
- Tune thresholds to the organization's normal sign-in patterns and detection requirements.
- Consider MFA results, conditional access, user risk, source reputation, and successful sign-ins before assigning severity.
- A detection result is an investigation lead, not proof of compromise.

## Outcome

This project demonstrates how KQL can turn sign-in events into a concise, reviewable list of potentially unusual authentication patterns.
