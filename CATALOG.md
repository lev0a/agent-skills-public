# Skill catalog

These are the skills and plugins I use. The snapshot links open the copies kept here. For downloads and updates, follow the original source links. Snapshots don't update automatically.

## By harness

I list shared skills once and group plugins by the agent they're built for.

| Category | Browse | Notes |
| --- | --- | --- |
| Shared skills | [Custom skills](#my-custom-skills) and [skills from others](#skills-from-others) | Skills originally selected from my Pi Wayfinder setup. |
| Cursor | [pstack](#cursor-plugins) | Plugin snapshot in its original folder structure. |

## Cursor plugins

| Browse snapshot | What it does | Original source / latest |
| --- | --- | --- |
| [pstack](plugins/cursor/pstack/) | Choose a workflow for a coding task, delegate work to agents, and verify the result. | [Lauren Tan / poteto](https://github.com/cursor/plugins/tree/main/pstack) |

This is pstack version 0.14.5 from [`cursor/plugins` commit `68836ddaf5697224520f1847d90cdb90ca8babaa`](https://github.com/cursor/plugins/tree/68836ddaf5697224520f1847d90cdb90ca8babaa/pstack). I removed `.gitignore`. The other 156 files and their Git file modes are unchanged, including the [MIT license](plugins/cursor/pstack/LICENSE).

The snapshot includes 45 plugin skills and three automation skills, along with scripts, agents, documentation, and images. Read its [README](plugins/cursor/pstack/README.md), [skills](plugins/cursor/pstack/skills/), or [setup guide](plugins/cursor/pstack/docs/guide/01-setup.md) here. Get the latest version from [pstack's original repository](https://github.com/cursor/plugins/tree/main/pstack).

Some pstack skills share names with the standalone skills below. They stay in their own package. Pstack's instructions include autonomous work and reading chat transcripts. Keeping a copy here doesn't activate those workflows or authorize messages, account changes, or automations. User instructions and environment permissions still apply.

## My custom skills

Custom skills by [Carl / lev0a](https://github.com/lev0a).

| Browse snapshot | Purpose | Origin |
| --- | --- | --- |
| [`linear-cockpit`](.agents/skills/linear-cockpit/) | Maintain Carl's human-readable Linear project cockpit. | Custom · Carl / lev0a |
| [`setup-project-tracking`](.agents/skills/setup-project-tracking/) | Set up or update approved project tracking. | Custom · Carl / lev0a |

## Skills from others

| Browse snapshot | Purpose | Original source / latest |
| --- | --- | --- |
| [`ask-matt`](.agents/skills/ask-matt/) | Choose an appropriate skill or workflow. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`code-review`](.agents/skills/code-review/) | Review a change against repository standards and its specification. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`codebase-design`](.agents/skills/codebase-design/) | Organize code into modules with simple interfaces. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`diagnosing-bugs`](.agents/skills/diagnosing-bugs/) | Find the causes of bugs and slowdowns. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`domain-modeling`](.agents/skills/domain-modeling/) | Define domain terms and document design decisions. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grill-me`](.agents/skills/grill-me/) | Ask detailed questions about a plan or design. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grill-with-docs`](.agents/skills/grill-with-docs/) | Question a plan and record decisions and definitions. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`grilling`](.agents/skills/grilling/) | Stress-test a plan, decision, or idea. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`handoff`](.agents/skills/handoff/) | Summarize a conversation for another agent. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`implement`](.agents/skills/implement/) | Implement work from a specification or tickets. | [Matt Pocock](https://github.com/mattpocock/skills) |
| [`improve-codebase-architecture`](.agents/skills/improve-codebase-architecture/) | Find places to hide complexity behind simpler module interfaces. | [Matt Pocock](https://github.com/mattpocock/skills) |
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

- 24 skills come from [Matt Pocock](https://github.com/mattpocock/skills). I adapted `wayfinder` to delegate research directly to child agents.
- Six skills come from [DietrichGebert's Ponytail](https://github.com/DietrichGebert/ponytail).
- Pstack comes from [Lauren Tan / poteto](https://github.com/cursor/plugins/tree/main/pstack). Only `.gitignore` is omitted.
- I made `linear-cockpit` and `setup-project-tracking`.

License notices are in [LICENSES/](LICENSES/) and [pstack's directory](plugins/cursor/pstack/LICENSE). I haven't chosen a public reuse license for my two custom skills yet.

## Scope

I keep credentials, account settings, personal session logs, and machine inventories out of this directory.

The directory currently shows 32 standalone skill snapshots and one pstack plugin snapshot.
