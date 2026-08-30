# Skill Catalog

A directory of the skills and plugins I use. Browse a snapshot to inspect its contents; follow the original source for downloads, installation instructions, and the latest updates. Recorded snapshots are not automatically synchronized with upstream.

## By harness

Shared skills appear once; harness-specific plugins have their own category. This is a showcase of the recorded setup, not a compatibility matrix or a live inventory of every machine.

| Category | Browse | Notes |
| --- | --- | --- |
| Shared skills | [Custom skills](#my-custom-skills) and [skills from others](#skills-from-others) | Standalone skill snapshots, originally selected from my Pi Wayfinder setup. |
| Cursor | [pstack](#cursor-plugins) | Plugin snapshot with its upstream structure preserved. |

## Cursor plugins

| Browse snapshot | What it does | Original source / latest |
| --- | --- | --- |
| [pstack](plugins/cursor/pstack/) | Coordinate engineering tasks through skills, playbooks, verification, and model delegation. Includes its scripts, documentation, agents, and automation pack. | [Lauren Tan / poteto](https://github.com/cursor/plugins/tree/main/pstack) |

pstack comes from [`cursor/plugins` commit `68836ddaf5697224520f1847d90cdb90ca8babaa`](https://github.com/cursor/plugins/tree/68836ddaf5697224520f1847d90cdb90ca8babaa/pstack), version 0.14.5. Its `.gitignore` is excluded at the repository owner's request; all 156 remaining files and their Git file modes are unchanged, including the [MIT license](plugins/cursor/pstack/LICENSE). The snapshot contains 45 plugin skills and three additional skills in the automation pack.

Inspect the recorded [README](plugins/cursor/pstack/README.md), [skills](plugins/cursor/pstack/skills/), and [setup guide](plugins/cursor/pstack/docs/guide/01-setup.md) here. For the current version and installation instructions, go to [pstack's original repository](https://github.com/cursor/plugins/tree/main/pstack). Its same-name skills remain separate from the standalone snapshots because they belong to a different upstream package.

The snapshot retains upstream behavior, including its autonomy rules and transcript-reading workflows. Inclusion here does not activate it or grant permission to send messages, change accounts, or start automations; the user's instructions and environment permissions still govern use.

## My custom skills

Custom skills by [Carl / lev0a](https://github.com/lev0a), including personal tracking conventions.

| Browse snapshot | Purpose | Origin |
| --- | --- | --- |
| [`linear-cockpit`](.agents/skills/linear-cockpit/) | Maintain Carl's human-readable Linear project cockpit. | Custom · Carl / lev0a |
| [`setup-project-tracking`](.agents/skills/setup-project-tracking/) | Set up or retrofit approved project tracking. | Custom · Carl / lev0a |

## Skills from others

| Browse snapshot | Purpose | Original source / latest |
| --- | --- | --- |
| [`ask-matt`](.agents/skills/ask-matt/) | Choose an appropriate skill or workflow. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`code-review`](.agents/skills/code-review/) | Review a change against repository standards and its specification. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`codebase-design`](.agents/skills/codebase-design/) | Design deep modules and useful seams. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`diagnosing-bugs`](.agents/skills/diagnosing-bugs/) | Diagnose hard bugs and performance regressions. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`domain-modeling`](.agents/skills/domain-modeling/) | Sharpen terminology, context documents, and ADRs. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grill-me`](.agents/skills/grill-me/) | Relentlessly interview the user about a plan or design. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grill-with-docs`](.agents/skills/grill-with-docs/) | Grill while producing ADR and glossary documentation. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grilling`](.agents/skills/grilling/) | Stress-test a plan, decision, or idea. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`handoff`](.agents/skills/handoff/) | Compact a conversation for another agent. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`implement`](.agents/skills/implement/) | Implement work from a specification or tickets. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`improve-codebase-architecture`](.agents/skills/improve-codebase-architecture/) | Find and review opportunities to deepen modules. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`ponytail`](.agents/skills/ponytail/) | Prefer the smallest solution that actually works. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`ponytail-audit`](.agents/skills/ponytail-audit/) | Audit a repository for over-engineering. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`ponytail-debt`](.agents/skills/ponytail-debt/) | List deliberate shortcuts recorded in `ponytail:` comments. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`ponytail-gain`](.agents/skills/ponytail-gain/) | Show Ponytail's benchmark impact. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`ponytail-help`](.agents/skills/ponytail-help/) | Show the Ponytail command reference. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`ponytail-review`](.agents/skills/ponytail-review/) | Review a change only for removable complexity. | [DietrichGebert / Ponytail](https://github.com/DietrichGebert/ponytail) |
| [`prototype`](.agents/skills/prototype/) | Build a throwaway artifact to answer a design question. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`resolving-merge-conflicts`](.agents/skills/resolving-merge-conflicts/) | Resolve an active merge or rebase conflict. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`setup-matt-pocock-skills`](.agents/skills/setup-matt-pocock-skills/) | Prepare a repository for the engineering workflow skills. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`tdd`](.agents/skills/tdd/) | Develop features or fixes test-first. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`teach`](.agents/skills/teach/) | Teach a concept within the current workspace. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`to-questionnaire`](.agents/skills/to-questionnaire/) | Turn unresolved decisions into a questionnaire. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`to-spec`](.agents/skills/to-spec/) | Turn an existing discussion into a specification. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`to-tickets`](.agents/skills/to-tickets/) | Break a plan into dependency-aware tickets. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`triage`](.agents/skills/triage/) | Categorize, verify, and prepare issues or pull requests. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`wait-what`](.agents/skills/wait-what/) | Re-explain something that did not land. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`wayfinder`](.agents/skills/wayfinder/) | Map and resolve work too large for one session. | [Matt Pocock](https://github.com/mattpocock/skills) · adapted |
| [`wizard`](.agents/skills/wizard/) | Generate an interactive wizard for steps only a human can perform. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`writing-for-agents`](.agents/skills/writing-for-agents/) | Write or edit skills and agent instruction files. | [Matt Pocock](https://github.com/mattpocock/skills) |

## Attribution and snapshot notes

- [Matt Pocock's skills](https://github.com/mattpocock/skills) — 24 skills; `wayfinder` includes a local adaptation for direct research delegation.
- [DietrichGebert's Ponytail](https://github.com/DietrichGebert/ponytail) — six skills.
- [Lauren Tan / poteto's pstack](https://github.com/cursor/plugins/tree/main/pstack) — one Cursor plugin snapshot, with only `.gitignore` excluded.
- [Carl / lev0a](https://github.com/lev0a) — `linear-cockpit` and `setup-project-tracking`.

The shared snapshots' upstream license notices are in [LICENSES/](LICENSES/); pstack's notice remains in its [plugin directory](plugins/cursor/pstack/LICENSE). The license for the two custom skills is pending selection.

## Scope

Entries reflect the skills selected for this showcase, not every package found in an earlier audit. Credentials, local account settings, personal session logs, and machine-specific inventories remain excluded.

The directory currently shows 32 standalone skill snapshots and one pstack plugin snapshot.
