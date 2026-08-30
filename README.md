# Agent skills

These are the agent skills and plugins I use. I keep snapshots here so you can read what they do. Each entry links to its creator's original source.

## Browse

[Browse the catalog](CATALOG.md) for descriptions, snapshots, and source links. I've marked which skills I made and which I've adapted.

- [My custom skills](CATALOG.md#my-custom-skills)
- [Skills from others](CATALOG.md#skills-from-others)
- [Cursor plugins](CATALOG.md#cursor-plugins)

## Snapshots and original sources

The snapshots show the versions I've collected. They don't update automatically.

Get the latest version and installation instructions from the original source:

- [Matt Pocock's skills](https://github.com/mattpocock/skills)
- [DietrichGebert's Ponytail](https://github.com/DietrichGebert/ponytail)
- [Lauren Tan / poteto's pstack](https://github.com/cursor/plugins/tree/main/pstack)

Shared skills live in `.agents/skills/`. Plugin snapshots live in `plugins/<harness>/`, with their original folder structure. The catalog notes any changes or omitted files.

## Attribution

The catalog credits each creator. Their license notices are in [LICENSES/](LICENSES/) and [pstack's directory](plugins/cursor/pstack/LICENSE).

I made `linear-cockpit` and `setup-project-tracking` for my own project tracking. I haven't chosen a public reuse license for them yet.

## Keep private material out

Keep credentials, account settings, environment files, personal session logs, and machine inventories out of this repo. Skills that use authenticated services should leave credentials in the environment where they run.

Before adding a snapshot, check every file and the Git history for secrets or private information. Read scripts without running them. A secret scan helps, but it can miss things.
