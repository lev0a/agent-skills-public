---
name: linear-cockpit
description: Keep Carl's Linear workspace readable, current, and useful as a phone-facing project cockpit while GitHub and project files remain canonical for technical truth. Use when an agent reads, creates, translates, starts, delegates, hands off, blocks, prioritizes, reviews, completes, or summarizes Linear-linked work; coordinates local, Linear-native, or direct-cloud AI execution; or when Carl asks for a plain-English Linear project update or freshness audit.
---

# Linear Cockpit

Use Linear to explain what work means to Carl. Keep technical commands, implementation evidence, exhaustive acceptance details, and version history in GitHub or the linked project files.

## Operating boundary

- Treat Linear as the human-readable project cockpit, not another vault and not the canonical technical record.
- Read the live Linear issue or project before proposing or applying a change.
- Verify material technical claims against the linked GitHub issue, project file, or fresh agent evidence. Never update Linear from memory alone.
- Keep Carl as the human owner. For new work, assign Carl unless he directs otherwise. Preserve an existing assignee unless the authorized task requires a change.
- Let the lead agent own the Linear narrative. Have subagents report to the lead unless the lead explicitly delegates the entire Linear issue, including its human-facing updates.
- Never treat project membership, Todo, `ready-for-agent`, or an agent label as permission to implement, deploy, spend, access credentials, contact people, or perform live effects.

## Execution lanes

Choose the lane that matches how the work is actually running. Do not make the workflow depend on a native agent integration, and do not create duplicate Linear issues when execution moves between lanes.

### Local or connector agent

- Keep Carl as assignee and leave the native delegate empty.
- Use the one current-agent label while work is active.
- Have the lead agent write meaningful starts, handoffs, gates, blockers, and verified results to Linear.
- Keep local thread details and subagent chatter out of Linear unless they change ownership, risk, the next step, or the outcome.

### Native Linear agent

- Only enter this lane when native delegation is available and the work itself is authorized.
- Keep Carl as assignee and use the native agent as delegate.
- Also use the one current-agent label so Carl can filter by executor on phone or desktop.
- Treat session creation, a delegate badge, or `Waiting` / `Thinking` text as launch attempts, not proof that a cloud task started.
- Verify that the native session reached a real running task before saying the agent is working. Record the task link when available.
- Use the native agent chat as execution activity; keep GitHub or the project files canonical for detailed technical evidence.

### Direct cloud fallback

- Keep Carl as assignee and leave the native Linear delegate empty.
- Use the one current-agent label while the cloud task is active.
- Link the direct cloud task in one compact start or handoff comment.
- Make the lead agent responsible for translating meaningful cloud progress, blockers, and the verified result back into Linear. Do not imply that direct cloud activity updates Linear automatically.
- Treat the cloud task as execution authority only for the work Carl actually authorized. It does not expand permission for live access, credentials, spending, delivery, deployment, or other outside effects.

Across all lanes, show only the lead executor as current. Preserve meaningful subagents and model history in handoff or completion comments instead of creating identities, labels, or duplicate issues for them.

## Agent and model identity

Record execution identity in provider-neutral fields so the cockpit remains accurate across Codex, Claude, Gemini, Hermes, Pi, Cursor, Linear-native agents, and future harnesses:

- **Currently working** is the agent harness or product surface, not the model family.
- **Model** is the complete model identity exposed by the active runtime or UI, including provider, family, version, and named variant when available. For example, record `GPT-5.6 Sol` rather than `5.6` or `GPT-5.6` when `Sol` is exposed.
- **Reasoning / thinking** is the exact configured effort, tier, or mode exposed by that runtime, such as `Light`, `Standard`, `High`, or an equivalent provider-specific name.
- Discover these values from current execution metadata, the active product UI, or a runtime-provided identity surface. Do not infer a variant or reasoning level from behavior, a generic agent label, prior comments, or a different thread.
- When a runtime does not expose a field, write `Not exposed` or qualify the known identity, such as `GPT-5.6 (variant not exposed)`. Never shorten a known full identity merely to normalize different providers.
- On a model, variant, reasoning-level, or harness change, record the new current identity in the next meaningful transition comment. Preserve older identities as history rather than rewriting past comments.

## Native launch failure

When a native delegate does not launch:

1. Check whether a real cloud task was created before retrying.
2. If task creation is uncertain, do not retry; record the uncertainty and reconcile first.
3. Retry at most once, only when Carl or the authorized workflow explicitly allows it and the retry has a concrete reason.
4. If the bounded attempt fails, clear the failed delegate and current-agent label because no agent is working.
5. Add `blocked` only when the integration failure prevents progress. Add `ready-for-human` only when Carl must take a specific action or make a decision.
6. Record the visible failure, whether a cloud task existed, what was ruled out, and the next targeted step. Do not keep retrying while waiting for support or an external-state change.

## Write authority

Allow a lead agent to update an existing issue autonomously when it represents already-authorized, Linear-linked work the lead owns. This includes status, current-agent label, readable progress, blockers, handoffs, priority with rationale, and verified completion.

Require Carl's approval before:

- creating a Linear project;
- creating or importing a batch of issues;
- changing the shared status or label vocabulary;
- reorganizing milestones across an existing project;
- canceling meaningful work.

Propose those changes without applying them when approval is absent. Creating one issue is allowed only when Carl explicitly requests it or an approved plan clearly requires that exact issue.

## Read-write-verify workflow

1. Confirm the workspace, team, project, and exact issue identifiers.
2. Read the current issue or project, its labels, comments, relations, and relevant source link.
3. Decide which meaningful transition is occurring: create, start, handoff, human gate, block, prioritize, review, complete, or project update.
4. Translate the change into plain English using the rules below.
5. Preserve unrelated metadata. When changing labels, read the full current label set and submit the intended full set because Linear label updates may replace the entire set.
6. Apply only the authorized, minimum change.
7. Re-read the changed item and verify its status, labels, assignee, priority, relations, description, and comment or update.
8. Report what changed and any remaining uncertainty.

## Plain-language standard

Make every issue answer:

1. What are we trying to accomplish?
2. Why does it matter to Carl?
3. What is happening now?
4. Who assigned, owns, and is executing the work?
5. Is anything blocked or waiting on Carl?
6. What happens next?
7. How can Carl recognize success?

Prefer everyday language. Explain unavoidable technical terms on first use. Link to technical evidence instead of copying commands, schemas, commit lists, test matrices, raw logs, or exhaustive failure cases into Linear.

## Status policy

Use the existing Levoa statuses:

- **Backlog:** Retain the work, but it is not ready or chosen next.
- **Todo:** The work is ready to begin.
- **In Progress:** Carl or a lead agent has actively taken responsibility.
- **In Review:** The work appears complete, but its result or evidence still needs verification.
- **Done:** Verify the promised outcome in the technical source before using this status.
- **Canceled:** Intentionally stop or supersede the work. Require Carl's approval for meaningful cancellation.
- **Duplicate:** Another issue represents the same work; link or name it.

Do not create lifecycle labels that duplicate these statuses.

## Label policy

Preserve existing labels and use them as follows:

- `ready-for-human`: Carl must take a specific action or make a decision.
- `ready-for-agent`: The issue is fully specified, unblocked, and available for an agent. Remove it when an agent starts.
- `needs-info`: Missing information prevents progress.
- `needs-triage`: The issue has not been evaluated and routed.
- `wontfix`: The work will deliberately not be pursued.
- `Bug`, `Feature`, `Improvement`: Optionally describe the work type.
- `blocked`: A concrete obstacle or unfinished dependency prevents progress.

Track the current executing harness with exactly zero or one of:

- `Agent · Codex`
- `Agent · Claude`
- `Agent · Hermes`
- `Agent · Pi`
- `Agent · Cursor`
- `Agent · Other`

Do not create labels for model versions, individual threads, named subagents, lifecycle phases, projects, milestones, priority, or technical specialties. Preserve model and contributor history in comments.

When another Linear issue causes a block, add a native blocking relation as well as `blocked`. Remove temporary labels promptly when they stop being true.

## Priority policy

Use best judgment and these meanings:

- **Urgent:** Carl should interrupt other work.
- **High:** One of the next important outcomes.
- **Medium:** Important, but not next.
- **Low:** Worth retaining with little current pressure.
- **No priority:** Default when there is no useful ordering signal.

Whenever changing priority, immediately leave a short plain-English reason in an issue comment or project update:

> **Priority set to High:** This is one of the next important outcomes because it unblocks Gmail collection and the combined digest.

Do not comment when merely preserving the current priority.

## Issue structure

Use these sections when creating or materially rewriting an issue. Omit a section only when it truly does not apply.

```markdown
## Current status

One or two sentences describing where this stands now.

## Why this matters

What this gives Carl in practical terms.

## What is happening

A plain-English summary of the work, without engineering instructions.

## How we will know it worked

- Three to seven understandable completion checks.

## Needs from Carl

The exact action or decision, or `Nothing right now.`

## Next step

The next expected movement.

## Agent activity

- Assigned by: lead agent or task
- Execution lane: local/connector, native Linear, or direct cloud
- Currently working: harness or `No agent currently working`
- Model: complete current model identity, including version and named variant when exposed
- Reasoning / thinking: exact current effort, tier, or mode when exposed
- Meaningful contributors: names or `None yet`

## Technical record

Canonical GitHub issue, project file, or other authoritative link.
```

Do not maintain manual issue counts in permanent descriptions when Linear can calculate them.

## Project structure

Create a project only for work with independently meaningful issues, observable phases, several sessions, or project-level decisions and risks. Use milestones only when their names communicate meaningful progress to Carl.

Use the project page as the project overview. Avoid a duplicate parent-summary issue unless it represents a genuine deliverable that can independently become Done.

Keep the overview readable:

```markdown
## Goal

The practical outcome.

## Current state

Where the project stands now.

## Now

What is actively moving.

## Needs from Carl

Decisions or actions, or `Nothing right now.`

## Next

The next expected movement.

## Risks

Only meaningful concerns.

## Technical record

Canonical source links.
```

Do not invent dates. Use due dates or target dates only for real external commitments. Do not use cycles or estimates by default.

## Agent activity and handoffs

On start:

- read the touched issue and technical source;
- move Todo work to In Progress;
- replace `ready-for-agent` with the one current-agent label;
- record the assigning lead, execution lane, executor, complete model identity, reasoning / thinking mode, task link when available, and next step.

On handoff:

- keep the status In Progress unless the work state truly changed;
- replace the current-agent label;
- leave a compact comment:

```text
Assigned by: <lead agent or task>
Execution lane: <local/connector | native Linear | direct cloud>
Currently working: <agent harness>
Model: <complete model identity, including version and named variant when exposed>
Reasoning / thinking: <exact effort, tier, or mode when exposed>
Work delegated: <plain-English bounded responsibility>
Meaningful contributors: <agents or none yet>
Technical task: <link when available>
Next: <expected movement>
```

On completion, remove the current-agent label but preserve the final execution lane, executor, complete model identity, reasoning / thinking mode, and meaningful contributors in the completion comment.

## Human gates and blockers

For a human gate:

- add `ready-for-human`;
- leave one concise comment that mentions Carl using his current Linear display name when the writing agent has a distinct Linear identity;
- when the Linear connection writes as Carl, do not claim that a self-mention created an Inbox notification; state the request in the issue and surface it in the active agent conversation or handoff instead;
- state the exact question or action Carl needs to address, what waits on it, and how he can answer;
- keep the underlying work status accurate;
- do not also add `blocked` unless progress is genuinely prevented.

Use this shape and do not post repeated reminder comments:

> @Carl Monroy - decision needed: <plain-English question or action>. Until then, <what is waiting>. Reply here with <the needed answer>.

Treat any Inbox item as a temporary alert, never as proof that Carl saw the request. Keep `ready-for-human` on the issue as the durable state until Carl responds, even if the Inbox notification is read, snoozed, deleted, or never generated. Do not make Inbox cleanup or Inbox zero part of the workflow.

For a blocker:

- add `blocked` and remove `ready-for-agent`;
- name the obstacle, consequence, and unblocking action;
- add the native blocking relation when another issue is responsible;
- add `ready-for-human` only when Carl specifically must act;
- keep In Progress when the lead still owns active resolution; use Backlog only when the work is no longer active or ready.

## Review and completion

Use In Review when work appears complete but verification is outstanding. Use Done only after fresh evidence verifies the promised outcome.

When completing:

- translate the result into `Done - what now works` language;
- link the authoritative evidence;
- remove resolved `blocked`, `ready-for-human`, `ready-for-agent`, and current-agent labels;
- preserve unrelated labels;
- leave the final executor, complete model identity, reasoning / thinking mode, contributors, residual risks, and next meaningful step in a concise comment;
- never turn uncertain, assumed, or second-hand completion into Done.

When evidence is unclear, keep In Progress or In Review, explain the uncertainty plainly, and name the next verification step.

## Project updates

Post a project update only when Carl requests one or when progress, risk, a human gate, or the next direction changes meaningfully. Include:

- what changed;
- what is moving now;
- what needs Carl;
- meaningful risks or blockers;
- what happens next;
- on-track, at-risk, or off-track health with a plain-English reason.

Let Linear calculate issue and milestone progress. Do not copy manual status counts into permanent project descriptions.

## Touched-item freshness check

Do not schedule or run automatic cleanup audits.

When a lead agent starts, hands off, blocks, or completes Linear-linked work, quickly check only the issue already being touched for stale:

- status;
- labels;
- agent identity;
- priority and its rationale;
- next-step information.

Broaden cleanup only when Carl requests it or when preparing a meaningful project update. Do not turn a transition update into an unsolicited workspace reorganization.
