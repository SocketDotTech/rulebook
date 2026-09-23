# Bungee Funded Perp Rulebook

This repository maintains the current Bungee Funded Perp rulebook and permanent snapshots of every published version.

## Current rulebook

**Current version:** v0.1 - Working Draft<br>
**Last updated:** September 23, 2026

[Read the current rulebook](./RULEBOOK.md)

## Version history

| Version | Date | Status | Snapshot | Changes |
| ------- | ---- | ------ | -------- | ------- |
| v0.1 | September 2, 2026 | Working Draft | [View v0.1](./versions/v0.1.md) | [Changelog](./CHANGELOG.md#v01---2026-09-02) |

## Repository structure

- [`RULEBOOK.md`](./RULEBOOK.md) - current rulebook
- [`versions/`](./versions/) - permanent version snapshots
- [`CHANGELOG.md`](./CHANGELOG.md) - material changes in each version

## Publishing a new version

1. Update `RULEBOOK.md`, including its version and last-updated date.
2. Copy the completed document to `versions/vX.Y.md`.
3. Add the version and change summary to `README.md` and `CHANGELOG.md`.
4. Commit the files and create the matching `vX.Y` Git tag.

Published snapshots and version tags should not be modified. Corrections should be released as a new version.
