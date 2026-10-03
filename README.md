# Bungee Funded Perp Rulebook

This repository maintains the current Bungee Funded Perp rulebook and permanent snapshots of every published version.

## Current rulebook

**Current version:** v0.2<br>
**Last updated:** October 3, 2026

[Read the current rulebook](./RULEBOOK.md)

## Version history

| Version | Date | Snapshot | Changes |
| ------- | ---- | -------- | ------- |
| v0.2 | September 29, 2026 | [View v0.2](./versions/v0.2.md) | [Changelog](./CHANGELOG.md#v02---2026-09-29) |
| v0.1 | September 2, 2026 | [View v0.1](./versions/v0.1.md) | [Changelog](./CHANGELOG.md#v01---2026-09-02) |

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
