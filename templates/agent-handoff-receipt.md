# Agent Handoff Receipt

Use this receipt when an agent handoff needs to be inspectable after a failure, retry, or resumed session.

## Handoff Identity

- Sender:
- Receiver:
- Handoff created at:
- Source session or task:
- Fingerprint:
- Fingerprint method:

## Context Budget Decision

- Requested context budget:
- Selected token count:
- Selection rule:
- Confidence threshold:
- Recency window:
- Quorum rule:

## Included Context

| Item | Why included | Confidence | Source |
| --- | --- | --- | --- |
|  |  |  |  |

## Omitted High-Confidence Items

Use this section for facts that were probably true but did not fit the target budget or were intentionally excluded.

| Item omitted | Confidence | Reason omitted | Risk if needed later |
| --- | --- | --- | --- |
|  |  |  |  |

## Open Questions

- Question:
- Why it matters:
- Suggested next check:

## Stop Receipt

Use this when the sender stopped because continuing would be unsafe, noisy, too expensive, or blocked.

- Stop reason:
- Stop category: `blocked` / `needs-human-approval` / `low-confidence` / `tool-failure` / `budget-exhausted` / `policy-boundary` / `other`
- Original stop evidence:
- Can retry:
- Retry condition:
- Retry must reference this receipt:

## Receiver Acknowledgement

- Injected:
- Facts loaded:
- Token count used:
- Tensions loaded:
- Questions preserved:
- Approval gates preserved:
- Receiver notes:

## Resume Prompt

```text
Resume from this handoff receipt:

- Fingerprint:
- Sender:
- Receiver:
- Selected context:
- Omitted high-confidence context:
- Stop/open questions:
- Do next:
- Do not do:
```
