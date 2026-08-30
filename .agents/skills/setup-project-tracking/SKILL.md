---
name: setup-project-tracking
description: Set up or retrofit project tracking when Carl explicitly asks for it. Selects Linear-only or Linear + GitHub from live project context, with Wayfinder as an optional approved overlay. Use for new projects, mid-project migrations, or incomplete tracker setup.
---

# Set Up Project Tracking

Set up the smallest tracking system that fits the project.

Treat `linear-cockpit`, `wayfinder`, and the Matt Pocock skills as read-only dependencies. This skill does not modify them.

## 1. Discover

Determine:

- Is this a new or active project?
- Does a Linear project already exist?
- Is there an authoritative GitHub repository with Issues enabled?
- Is tracking partially configured?
- Where does current project truth live?
- Does Carl already want Wayfinder?

For an active project, read [references/retrofit.md](references/retrofit.md).

Use the current conversation as context, not as the only project record. Read available project files, live trackers, Git state, and GitHub issues.

Completion criterion: completed, active, blocked, and next work is accounted for or explicitly marked unknown.

## 2. Recommend a tracking mode

Choose one base mode.

### Linear only

Use when there is no authoritative GitHub repository.

Linear owns project state, ownership, priority, blockers, human gates, and next steps. Link other authoritative records where available.

### Linear + GitHub

Recommend when an authoritative GitHub repository with Issues enabled exists.

- Linear owns readable project state, ownership, priority, current agent, blockers, and next steps.
- GitHub owns technical questions, implementation detail, evidence, code-linked discussion, and agent receipts.
- Pair technical work items. Keep administrative or human-only work in Linear unless a GitHub record adds value.

Read [references/github-pairing.md](references/github-pairing.md).

Use Linear-only when no repository exists. Creating a repository is a separate decision that requires Carl's approval.

## 3. Consider the Wayfinder overlay

Wayfinder is independent of the base mode.

Recommend it only when:

- Carl requests Wayfinder; or
- the destination is clear but the route contains several unresolved decisions that exceed one normal session.

Explain the recommendation. Obtain approval before creating a map or decision tickets.

When approved, load and follow the existing `wayfinder` skill unchanged.

## 4. Present the plan

Show:

- new or retrofit setup;
- selected base mode;
- whether Wayfinder is included;
- project and issue structure;
- existing items to reuse;
- new items to create;
- proposed relationships and labels;
- authoritative records;
- unknown history that cannot be reconstructed.

Obtain Carl's approval before creating a Linear project, importing an issue batch, creating GitHub issues, or changing shared labels. Do not repeat questions Carl already answered.

Completion criterion: Carl approved the exact structure and write set.

## 5. Configure

Read `linear-cockpit` completely before any Linear write.

Create or reconcile exact matches. Preserve unrelated metadata and the complete existing label set.

For a repository project:

- create reciprocal Linear and GitHub links;
- preserve existing GitHub and Linear metadata;
- add a project-local tracker contract;
- add one concise pointer to the existing `AGENTS.md` or `CLAUDE.md`;
- leave commit and push for separate authorization.

For a non-repository project, record the tracker contract in the Linear project overview or another approved project record.

## 6. Verify

Re-read every changed tracker item.

Verify:

- titles and reciprocal links;
- assignee and project;
- statuses and complete labels;
- parent and blocking relationships;
- current, completed, blocked, and next work;
- Wayfinder frontier when Wayfinder is enabled.

Write an owner-safe setup receipt. Include IDs, URLs, verification, and unresolved uncertainty. Exclude credentials and private raw data.

Completion criterion: a fresh agent can read the approved surfaces and compute the same current state.
