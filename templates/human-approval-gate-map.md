# Human Approval Gate Map

AI agents can prepare work, but some actions should not run without a human owner approving the risk.

## Approval Levels

| Level | Action type | Approval needed |
| --- | --- | --- |
| Low | Read-only analysis, local tests, draft docs | No approval after task is assigned |
| Medium | File edits, dependency installs, generated artifacts | Human can approve by task scope |
| High | Public posts, outreach, deploys, account settings, paid tools | Explicit approval before action |
| Critical | Production data mutation, payments, credentials, legal commitments | Named owner approval required |

## Workflow Map

| Step | System | Can mutate state? | Risk level | Approval owner | Evidence required |
| --- | --- | --- | --- | --- | --- |
| 1 |  | Yes / No | Low / Medium / High / Critical |  |  |
| 2 |  | Yes / No | Low / Medium / High / Critical |  |  |

## Required Stop Rules

- Stop if credentials, tokens, or secrets are requested.
- Stop before public outreach, comments, posts, or emails.
- Stop before payment, subscription, or paid API usage.
- Stop before deployment when rollback is unclear.
- Stop when generated code touches authentication, billing, user data, or infrastructure without a named reviewer.

## Approval Message Template

```text
Approval needed:

- Action:
- System affected:
- Risk:
- Cost:
- Rollback:
- Evidence:

Please approve or reject.
```
