# Agent Skills

A browsable directory of the agent skills and plugins I use, with snapshots of their contents and credit to their creators.

## Browse

[Browse the catalog](CATALOG.md) to see what each skill does, inspect its recorded snapshot, and follow its original source. Entries distinguish my custom skills, skills by other people, and adaptations.

- [My custom skills](CATALOG.md#my-custom-skills)
- [Skills from others](CATALOG.md#skills-from-others)
- [Cursor plugins](CATALOG.md#cursor-plugins)

## Snapshots and original sources

The files here show the versions recorded in my setup. They make the directory inspectable; they are not maintained as a download or update channel for other people's skills. Snapshots can lag behind upstream.

For downloads, installation instructions, and the latest updates, follow each entry's original source:

- [Matt Pocock's skills](https://github.com/mattpocock/skills)
- [DietrichGebert's Ponytail](https://github.com/DietrichGebert/ponytail)
- [Lauren Tan / poteto's pstack](https://github.com/cursor/plugins/tree/main/pstack)

Shared skills are recorded once in `.agents/skills/`; plugin snapshots retain their structure under `plugins/<harness>/`. The catalog records adaptations and exclusions. There is no installer or automatic synchronization.

## Attribution

Original creators and source repositories are linked in the catalog. Upstream license notices remain in [LICENSES/](LICENSES/) and [pstack's directory](plugins/cursor/pstack/LICENSE).

My custom skills are `linear-cockpit` and `setup-project-tracking`. They contain personal tracking conventions; no additional public reuse license has been selected for them.

## Keep private material out

No credentials, account configuration, local environment files, personal session logs, or machine inventories belong here. A skill may describe using an authenticated service; its credentials remain in that environment.

Before publishing or adding skills, check the complete folders and Git history for secrets and personal/private context. Review scripts without executing them. A clean pattern scan is useful evidence, not a guarantee of safety.
