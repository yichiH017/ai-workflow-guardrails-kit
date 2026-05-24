# AI-Generated PR Review Checklist

Use this when a pull request was created or heavily modified with help from an AI coding agent.

## 1. Scope

- [ ] The PR has one clear purpose.
- [ ] The PR description explains what the agent was asked to do.
- [ ] The changed files match the stated task.
- [ ] Unrelated refactors are called out or removed.

## 2. Ownership

- [ ] A human owner is responsible for the final diff.
- [ ] Agent-generated assumptions are listed.
- [ ] Any copied or generated third-party code is identified.
- [ ] Security-sensitive, billing, account, data, or deployment changes have a named reviewer.

## 3. Evidence

- [ ] Tests or checks run are listed with exact commands.
- [ ] Failing or skipped checks are disclosed.
- [ ] Manual verification steps are described.
- [ ] Remaining risks are written in plain language.

## 4. Risk Gates

- [ ] The PR does not mutate production data without approval.
- [ ] The PR does not add secrets, credentials, or tokens.
- [ ] Any external API, browser automation, or account action is behind an explicit approval step.
- [ ] Deployment impact is clear before merge.

## 5. Review Quality

- [ ] The reviewer can explain the core change without relying on the agent's summary.
- [ ] The diff is small enough to review responsibly.
- [ ] The agent did not silently change formatting, generated files, or lockfiles outside scope.
- [ ] The merge plan includes rollback or stop rules when needed.
