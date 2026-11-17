# test/

The tests of pkgm-base-manager, a section per file, each test by its name.

## `pkgm.test.js`

A package in miniature, as the package writer makes them, in a temporary folder: assembled, tested, verified, deployed.

- closure: ours by name and by relative path, third-party all the way down; nothing else
- assemble: a swarm's codebase into a repository, its contents said; again: unchanged; a name the package lacks: refused
- test: bottom up, the modules, the swarms, the named tests; a failure said with its output
- test: a run that does not end is stopped, and fails; the rest still run
- test: a set, its in-place tests and (or not) the modules; a booted test listed, not run
- verify: a package intact against the hash it was written with; changed, or one file replaced: said, not intact
- deploy: staged beside, intact, validated, then in place; a changed or failing package changes nothing

## `sources.test.js`

- sign and verify: the publisher's signature over the canonical form
- loadManifest: the newest signed one, never older than seen
- loadPackage: checked by hash, from the first source that matches; addons only if missing
- a web source: downloaded with curl (here a file:// URL)
