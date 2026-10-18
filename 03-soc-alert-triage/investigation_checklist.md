# Authentication Alert Investigation Checklist

## Validate
- [ ] Confirm alert time range and detection rule.
- [ ] Identify affected user, source address, application, and host.
- [ ] Confirm event fields and time zone.

## Investigate
- [ ] Review failed and successful authentication events.
- [ ] Check MFA and conditional-access results where available.
- [ ] Compare source, location, device, and sign-in pattern with expected activity.
- [ ] Correlate identity, endpoint, VPN, and firewall telemetry.
- [ ] Review actions taken after the successful authentication.

## Decide and document
- [ ] Record supporting evidence and benign explanations considered.
- [ ] State what remains unknown.
- [ ] Assign disposition based on the available evidence and local policy.
- [ ] Escalate when required and document the handoff.
