# Agent Skills

A personal library of reusable agent skills, with one copy of each package and clear credits.

## Browse

[CATALOG.md](CATALOG.md) groups the library by harness and distinguishes my custom skills, upstream skills, and adaptations.

```text
.agents/skills/<name>/    # One complete package per skill
plugins/cursor/pstack/   # Upstream plugin snapshot; see catalog for exclusions
CATALOG.md               # Harness categories, purpose, and credits
LICENSES/                # Third-party copyright and license notices
```

A skill shared by several harnesses stays in one folder. Selected plugins are preserved as upstream snapshots under their harness directory, with any exclusions recorded in the catalog; this library does not manage their updates.

## Give a cloud agent the library

Start with a request like:

> Download https://github.com/lev0a/agent-skills-public into this cloud environment. Read its catalog and install the skills needed for this task using your harness's supported skill location. Keep complete skill folders and their relevant license notices. Check for existing same-name skills; reuse identical copies and ask before replacing different ones. Do not run bundled scripts during installation, change my project, or commit installed copies. Report the revision, installed names, and anything you cannot load. Then demonstrate wait-what with a harmless explanation.

A public repository removes the need for GitHub credentials to download it. It does not automatically install skills into every cloud session. Use the environment's existing setup step when repeat installation is useful; no custom manager or synchronization service is required.

For the bundled pstack snapshot, read its [catalog entry](CATALOG.md#cursor-plugins) before installation. Keep the plugin directory intact and follow its upstream setup instructions for the target environment. Downloading the snapshot does not activate its skills or automations.

The skill format is shared, but discovery and available tools vary by harness. [Codex documents local skill locations](https://learn.chatgpt.com/docs/build-skills); [Cursor distinguishes local and cloud discovery](https://cursor.com/docs/skills); [Devin documents discovery across connected repositories](https://docs.devin.ai/product-guides/skills). A successful download is not proof that the agent loaded a skill. Cloud use must be tested in the actual environment.

## Sources and licenses

- 24 packages originate from [Matt Pocock's skills](https://github.com/mattpocock/skills); retain [his MIT notice](LICENSES/mattpocock.txt).
- Six packages originate from [DietrichGebert's Ponytail](https://github.com/DietrichGebert/ponytail); retain [its MIT notice](LICENSES/ponytail.txt).
- The pstack plugin originates from [Lauren Tan / poteto in cursor/plugins](https://github.com/cursor/plugins/tree/main/pstack); its [MIT notice](plugins/cursor/pstack/LICENSE) remains inside the snapshot.
- Two packages are custom work for this collection: `linear-cockpit` and `setup-project-tracking`. No additional reuse license is granted for these custom skills yet.
- `wayfinder` is adapted from Matt Pocock's work, not an original custom skill. See the catalog for the recorded change.

When copying individual third-party packages, include the applicable notice in each installed or redistributed package. Credits alone do not replace the license notice.

## Keep private material out

No credentials, account configuration, local environment files, personal session logs, or machine inventories belong here. A skill may describe using an authenticated service; its credentials remain in that environment.

Before publishing or adding skills, check the complete folders and Git history for secrets and personal/private context. Review scripts without executing them. A clean pattern scan is useful evidence, not a guarantee of safety.

The two custom tracking skills contain personal ownership and workflow conventions. They are provided as personal workflows, not generic organization policies.
