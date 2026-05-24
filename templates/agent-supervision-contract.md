# Agent Supervision Contract

Use this before an agent can run tools, modify code, touch data, send messages, deploy, or create external side effects.

## Action

- Agent or persona:
- Tool or action:
- Requested scope:
- Triggering issue, ticket, or run:
- Expected output:

## Risk Level

Choose one:

- Low: read-only or draft-only action.
- Medium: local file change, non-production change, or reversible workflow action.
- High: public content, customer-facing output, account setting, production config, paid API usage, or deployment.
- Critical: data deletion, credential rotation, billing change, security policy change, or irreversible external action.

## Allowed Scope

- Allowed repositories, files, systems, or data:
- Explicitly forbidden repositories, files, systems, or data:
- Network or API boundaries:
- Cost or runtime limit:

## Approval Rule

- Approval owner:
- Approval required before:
- Evidence required for approval:
- Expiration or re-approval condition:

## Execution Receipt

After the action, record:

- What changed:
- Commands, checks, or logs:
- Evidence links:
- Known gaps:
- Residual risk:
- Rollback or compensation path:

## Stop Conditions

Stop and request human approval if:

- The action expands beyond the approved scope.
- A secret, credential, customer record, or billing setting is involved.
- The agent cannot verify the result.
- The agent needs to contact a person, publish content, or spend money.
- The rollback path is unknown.
