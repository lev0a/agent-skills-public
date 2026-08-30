# Pair Linear with GitHub

Use this branch only when an authoritative GitHub repository with Issues enabled already exists.

## Role split

- Linear is the readable project cockpit: state, owner, current agent, priority, blockers, human needs, and next step.
- GitHub is the technical ledger: full technical question, implementation detail, evidence, code links, agent receipts, and verification.

Pair an item when technical evidence or code-linked discussion belongs in GitHub. Keep administrative and human-only items in Linear when a GitHub twin would be empty.

## Reconcile before creating

Read live state first:

```bash
gh repo view <owner/repo> --json nameWithOwner,isPrivate,hasIssuesEnabled,url
gh issue list --repo <owner/repo> --state all --limit 100 --json number,title,state,url,labels
```

Search exact titles on both trackers. Reuse one exact match. Stop for reconciliation if duplicates or conflicting candidates exist.

## Create and link

1. Create or reuse the GitHub technical issue.
2. Create or reuse the Linear issue using the `linear-cockpit` structure.
3. Put the GitHub URL under Linear **Technical record**.
4. Put the Linear URL under GitHub **Linear counterpart**.
5. Add native parent and blocking relations when the approved project structure requires them.
6. Re-read both items and verify reciprocal navigation.

Use existing labels where they express the approved meaning. Shared label changes require Carlos's approval. Wayfinder labels belong only to an approved Wayfinder overlay.

## Work and completion

Linear is the claim surface. GitHub records detailed starts, evidence, and completion receipts.

After technical verification:

1. close the GitHub technical issue or verify its code-linked completion state;
2. move Linear to `Done`;
3. remove temporary workflow and current-agent labels;
4. preserve the final evidence link and executor history.

Keep credentials, private raw data, identities, and complete private transcripts out of both trackers. Link an owner-only source location when evidence cannot be copied safely.

Completion criterion: each paired item independently reaches its counterpart, and both surfaces report the same verified outcome.
