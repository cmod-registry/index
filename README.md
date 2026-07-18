# cmod-registry/index

The module index for [cmod](https://github.com/satishbabariya/cmod) — the
Git-native package and build tool for C++20 modules.

`cmod search <query>` clones/pulls this repository and queries
`index.json`. The format is `cmod-resolver`'s `RegistryIndex`
(`version: 1`); entries point at Git repositories, which remain the source
of truth for code.

Currently seeded with the nine validated
[cmod-ecosystem](https://github.com/cmod-ecosystem) ports. See
[POLICY.md](POLICY.md) for listing rules and the submission roadmap.
