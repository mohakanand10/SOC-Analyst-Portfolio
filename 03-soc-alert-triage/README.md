# Project 03 — SOC Alert Triage and MITRE ATT&CK Mapping

## Objective

Follow a structured workflow for validating an authentication alert, assessing available evidence, identifying useful next checks, and documenting a clear disposition.

## Scenario

An alert reports repeated failed sign-ins followed by a successful sign-in for the same account. The analyst must determine what is known, what remains uncertain, and what evidence to collect next.

## Skills demonstrated

- Initial alert validation
- Timeline and identity review
- Evidence-based assessment
- MITRE ATT&CK technique awareness
- Incident notes and escalation recommendations

## Files

- `triage/triage_report.md` — example case notes and follow-up plan
- `triage/investigation_checklist.md` — reusable checklist for similar alerts

## Potential ATT&CK mapping

MITRE ATT&CK technique **T1110 — Brute Force** may be relevant when evidence supports repeated attempts to guess or obtain credentials. Choose a more specific sub-technique only when the activity supports it.

## Outcome

This project demonstrates a consistent approach to first-line triage without treating a single alert as a confirmed incident.
