# 7-Day AI Workflow Guardrails Rollout

This is a lightweight rollout for one repository or one agent-assisted development workflow.

## Day 1: Map The Current Workflow

- Identify the agent tools in use.
- List where prompts, commands, diffs, tests, and deployment actions happen.
- Pick one recent PR or task as the sample case.

## Day 2: Add Trace Logging

- Use `templates/workflow-trace-log.md`.
- Require exact commands and verification results.
- Require residual risks to be written before review.

## Day 3: Add PR Review Rules

- Use `templates/ai-pr-review-checklist.md`.
- Add a short AI-generated code section to PR descriptions.
- Reject PRs where scope, owner, or verification is unclear.

## Day 4: Define Handoffs

- Use `templates/agent-handoff-template.md`.
- Require every agent handoff to name completed work, blockers, next action, and files not to change.

## Day 5: Add Human Approval Gates

- Use `templates/human-approval-gate-map.md`.
- Mark deploys, account actions, paid tools, public content, and data mutation as approval-gated.

## Day 6: Run One Real PR Through The Process

- Keep the process small.
- Remove any field nobody uses.
- Add only the missing evidence reviewers needed.

## Day 7: Review And Decide

- Keep guardrails that reduced review uncertainty.
- Drop guardrails that created paperwork without reducing risk.
- Decide whether to expand to more repositories.
