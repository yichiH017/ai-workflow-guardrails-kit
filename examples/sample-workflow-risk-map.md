# Sample Workflow Risk Map

This example shows the style of output produced by an AI Workflow Guardrails Audit.

## Context

A team uses AI coding agents to draft code changes, run local commands, and prepare pull requests. Reviews are getting slower because reviewers have to reconstruct the agent's intent from the diff.

## Observed Risk Areas

| Area | Risk | Guardrail |
| --- | --- | --- |
| Prompt scope | The agent may solve a broader task than requested. | PR description must include the original task and out-of-scope items. |
| File ownership | Multiple agents may edit the same files without coordination. | Handoff template must list files changed and files not to change. |
| Verification | The agent may report success without exact evidence. | Trace log must include commands and results. |
| Side effects | Scripts may contact APIs, deploy, or mutate state. | Human approval gate before external state-changing actions. |
| Review load | Large generated diffs overwhelm reviewers. | Split PRs by owner, behavior, and risk category. |

## Recommended First Change

Start by adding the PR review checklist and workflow trace log to one active repository. Do not automate enforcement until the team has used the templates on at least three real PRs.

## Stop Rule

Pause the rollout if developers start filling the templates mechanically without improving review clarity. Guardrails should reduce uncertainty, not create ritual paperwork.
