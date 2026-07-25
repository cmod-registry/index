## Module submission

<!-- Paste the entry fragment printed by `cmod publish` (or hand-write it)
     into index.json under "modules", keyed by the module name. -->

- [ ] Entry added under `"modules"` with the module name as the key
- [ ] `license` is a valid SPDX identifier and `description` is set
- [ ] Every version parses as semver and its `tag` + `commit` exist in the linked repository
- [ ] No existing listings or version rows were removed (yanks set `"yanked": true`)

The **Validate submission** check runs `cmod registry validate` — the same
governance rules the client enforces. See [POLICY.md](../POLICY.md).
