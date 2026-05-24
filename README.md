# AI Workflow Guardrails Kit

Practical templates for teams using AI coding agents such as Codex, Claude Code, Cursor, GitHub Copilot, n8n, or custom agent workflows.

The goal is simple: ship faster with AI-generated code while keeping review quality, traceability, ownership, and human approval boundaries clear.

## What Is Included

- [AI-generated PR review checklist](templates/ai-pr-review-checklist.md)
- [Agent handoff template](templates/agent-handoff-template.md)
- [Workflow trace log](templates/workflow-trace-log.md)
- [Human approval gate map](templates/human-approval-gate-map.md)
- [7-day rollout plan](docs/7-day-rollout-plan.md)
- [Sample workflow risk map](examples/sample-workflow-risk-map.md)

## Who This Is For

This kit is useful if your team is already using AI coding agents and starting to see:

- review fatigue from large AI-generated diffs,
- unclear ownership between human developers and agents,
- scripts or CI steps running before someone has approved the risk,
- missing evidence for what was tested,
- agent handoffs that are hard to audit later.

## How To Use It

1. Pick one repository or one workflow.
2. Fill out the workflow trace log for a recent AI-assisted change.
3. Use the PR checklist during review.
4. Mark every step that can mutate code, data, deployments, accounts, or public content.
5. Add explicit human approval gates before those steps.
6. Review the process after one week and remove anything that adds paperwork without reducing risk.

## Paid Audit

If you want this adapted to your actual repository or AI development workflow, I offer a focused AI Workflow Guardrails Audit.

Offer page: https://market-intel-os-ai-dev.pages.dev/

Contact: oneseven.huang@gmail.com
