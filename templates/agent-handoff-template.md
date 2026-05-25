# Agent Handoff Template

Use this when one human or AI agent hands work to another agent, reviewer, or operator.

## Task

- Goal:
- User request:
- Current status:
- Next best action:

## Handoff Metadata

- Sender:
- Receiver:
- Fingerprint:
- Requested context budget:
- Selected token count:
- Confidence threshold:
- Stop/open questions:

## Files And Ownership

- Files changed:
- Files intentionally not touched:
- Generated artifacts:
- Human owner:

## Decisions Made

- Decision:
- Reason:
- Tradeoff:

## Budget And Omission Notes

- Context budget requested:
- Context selected:
- High-confidence context omitted:
- Why omitted:
- Risk if omitted context becomes relevant:

## Verification

- Commands run:
- Results:
- Manual checks:
- Known gaps:

## Risk Notes

- Can this change affect production?
- Can this change mutate data?
- Can this change contact users, publish content, spend money, or change accounts?
- Does the next step require human approval?
- Is there a stop receipt the next attempt must reference?

## Continuation Prompt

Use this section to give the next agent exact context without forcing it to rediscover the whole workflow.

```text
Continue from this state:

- Goal:
- Completed:
- Blocked by:
- Do next:
- Do not change:
```
