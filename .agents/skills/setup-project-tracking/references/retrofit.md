# Retrofit an active project

Reconstruct the current project state without inventing history.

## Source order

Read the highest-trust available sources:

1. live Linear and GitHub items;
2. canonical project files, plans, and decision records;
3. Git history, pull requests, releases, and the current worktree;
4. durable agent receipts and session handoffs;
5. the current conversation.

The conversation can explain intent. Use durable evidence to verify completed work and live state.

## Build the crosswalk

Account for each meaningful work item as:

- completed;
- active;
- blocked;
- ready next;
- retained for later;
- unknown.

For each item, record its name, practical outcome, evidence location, current owner, blockers, next step, and proposed tracker destination. Group commits and chat fragments by meaningful outcome instead of creating one issue per artifact.

Use `Done` only when current evidence verifies the outcome. Preserve uncertainty as uncertainty. Do not assign invented dates, owners, or decisions.

## Reconcile

Search exact project and issue names before creating anything. Reuse exact matches and preserve unrelated metadata. Treat partial prior setup as state to repair, not a reason to restart.

Present the crosswalk and unresolved gaps before writes. Carlos approves the imported batch and any shared vocabulary changes.

Completion criterion: every meaningful known work item has one proposed live state, and every unresolved gap is visible to Carlos.
