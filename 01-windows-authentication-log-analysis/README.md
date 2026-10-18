# Project 01 — Windows Authentication Log Analysis

## Objective

Review Windows authentication events to identify repeated failed logons and determine whether a successful logon followed them.

## Skills demonstrated

- Understanding Windows Security Event IDs `4624` and `4625`
- Sorting events chronologically
- Grouping activity by account and source address
- Building an evidence-based investigation summary
- Identifying follow-up checks before drawing a conclusion

## Files

- `data/authentication_events.csv` — sample authentication event dataset
- `analysis/analyst_findings.md` — findings and recommended next steps

## Investigation workflow

1. Review the event timeline.
2. Separate successful logons (`4624`) from failed logons (`4625`).
3. Group repeated failures by account and source IP.
4. Check whether a success follows a series of failures.
5. Review logon type, user context, MFA/identity logs, and endpoint activity.
6. Document what the evidence supports and what still needs validation.

## Key finding

The included dataset contains several failed logons for one account, followed by a successful logon from the same example source address. This pattern is worth investigating in a real environment, but it is not enough by itself to confirm account compromise.

## Example Windows event IDs

| Event ID | Meaning |
|---|---|
| `4624` | An account successfully logged on |
| `4625` | An account failed to log on |

## Outcome

This project demonstrates a repeatable first-pass method for reviewing authentication activity and documenting next steps in a SOC workflow.
