# mailcellar

Local backups of Gmail accounts, kept as an archive you control: back mail up
in [Got Your Back](https://github.com/GAM-team/got-your-back)'s format, remove
duplicates, move old mail out of Gmail while the backup keeps it, put it back
when it's needed, and report on what's there.

## The project

**[mailcellar/mailcellar](https://github.com/mailcellar/mailcellar)** is one
Python package behind one `mailcellar` command:

| Command | What it does |
| --- | --- |
| `backup`, `count`, `meta`, `verify` | Incremental backups, a comparison with Gmail, and a check that the files are intact |
| `dedup` | Find duplicate messages within and across accounts and remove them from Gmail, in stages |
| `offload` | Take old mail out of Gmail by rule, keeping it in the backup |
| `restore` | Put backed-up mail back into Gmail |
| `report` | Storage, bulk mail, volume, threads, labels, correspondents, backup health |

Anything that changes Gmail is a dry run first, then an explicit flag, and
nothing is ever deleted permanently from Gmail.

## Start here

- [README and quick start](https://github.com/mailcellar/mailcellar#readme)
- [Guides](https://github.com/mailcellar/mailcellar/tree/main/docs/guide):
  setting up Google Cloud, migrating from gyb, offloading old mail safely,
  recovery, troubleshooting
- [How it fits together](https://github.com/mailcellar/mailcellar/blob/main/docs/architecture.md)
- [Contributing](https://github.com/mailcellar/mailcellar/blob/main/CONTRIBUTING.md)

## Mail is personal data

Issues, pull requests and discussions here are public. Please never post real
mail, addresses, names, subjects, tokens or `client_secrets.json`; use
placeholders such as `alex@example.com`. For a security problem, report it
privately: see
[SECURITY.md](https://github.com/mailcellar/mailcellar/blob/main/SECURITY.md).

## About

Licensed under the Apache License 2.0. mailcellar is a separate project from
Got Your Back and is not affiliated with or endorsed by Google or the gyb
project. Gmail and Google Workspace are trademarks of Google LLC.

