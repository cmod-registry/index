# cmod Registry Policy

This index lists Git-native C++20 module packages consumable by
[cmod](https://github.com/satishbabariya/cmod). Listing here is metadata
only — source distribution stays in each module's own Git repository.

## Listing requirements

Enforced by `cmod`'s governance validation (`validate_for_publishing`):

- **License** — an SPDX identifier is required.
- **Description** — required.
- **Semver** — every published version must parse as semantic versioning.
- **Naming** — reverse-domain module names (e.g. `com.github.owner.repo`),
  2–128 chars, `[a-zA-Z0-9._-]` only.
- **Reserved names** — `std`, `std.*`, `stdx`, `stdx.*` are banned.

## Submissions

Open a pull request adding your entry to `index.json` — `cmod publish`
prints a ready-made fragment when it lacks push access. The **Validate
submission** CI check enforces the rules above plus the no-deletions
policy; a maintainer merge completes the listing.

## Yanking

Versions are never deleted; a yanked release keeps its row with
`"yanked": true` so existing lockfiles continue to resolve.

## Disputes

Name disputes and takedowns are decided by the cmod maintainers
(currently @satishbabariya). Open an issue on this repository.
