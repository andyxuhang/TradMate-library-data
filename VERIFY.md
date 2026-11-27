# Verify the published snapshot

Download or clone this public repository, then verify the immutable snapshot:

```sh
git checkout library-build220-9272ecb3f8ea
cd datasets/build220-9272ecb3f8ea
shasum -a 256 -c SHA256SUMS
```

On Linux, `sha256sum -c SHA256SUMS` is equivalent. For a direct SQLite download,
its expected SHA-256 is `9272ecb3f8eaa238106afe37f981d1eda1aed4843c8ddf3d5d956780f8939def` and size is **34,881,536 bytes**.
No Git LFS client or application login is required to obtain these files.

Use SQLite's read-only mode for structural checks:

```sh
sqlite3 -readonly tradmate_library.db 'PRAGMA integrity_check; PRAGMA foreign_key_check;'
sqlite3 -readonly tradmate_library.db 'SELECT count(*) FROM tunes; SELECT count(*) FROM tune_versions; SELECT count(*) FROM aliases;'
```

Expected: integrity `ok`, no foreign-key rows, followed by `23423`, `55412`,
`29595`. `rating_history` has **23,300** rows of previous bundled default stars;
it is not personal activity. The only tables are `metadata`, `tunes`,
`tune_versions`, `aliases`, `rating_history`.

See `dataset-manifest.json` for per-file hashes, schema and upstream input
identities. The root `versions/build220.json` is an identical manifest copy.
Checksums establish file identity, not independent clearance of every work.
Keep `LICENSE.md` and `ATTRIBUTION.md` with redistributed data.
