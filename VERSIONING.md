# Dataset version and release policy

## Current snapshot

Published on 2026-11-27: **`library-build220-9272ecb3f8ea`**, matching committed TradMate **1.0.3 (220)**,
source revision `823fbf4cb5941394d86b5dd476ba46cc6e891f47`. Its [manifest](versions/build220.json) and
[download directory](datasets/build220-9272ecb3f8ea/) describe the actual published files.
The database SHA-256 is
`9272ecb3f8eaa238106afe37f981d1eda1aed4843c8ddf3d5d956780f8939def` (34,881,536 bytes).

This publication was explicitly requested by the repository owner on 2026-11-27.
The earlier documentation-only restriction is superseded for this snapshot;
the upstream license originals and individual-content scope are retained.
No private permission correspondence or signatures are published.

The database update is based on upstream data dated 2026-11-08; the separate
alias-search index is dated 2026-11-15. These are not the publication date or
the original import date. Each component keeps its own provenance and checksum.

## History

| Snapshot | App | Database status | Tunes | Settings | Catalog aliases |
| --- | --- | --- | ---: | ---: | ---: |
| [Build 73](versions/build73.json) | 0.31.73 (73) | Historical metadata only; original record unchanged | 23,300 | 54,997 | 29,436 |
| [Build 220](versions/build220.json) | 1.0.3 (220) | Complete adapted data published | 23,423 | 55,412 | 29,595 |

The catalog update added 123 tune records, 415 settings and 159 SQLite aliases;
959 existing ABC settings changed. The user-facing change ledger additionally
tracks names, meters, dance types and keys across 1,073 existing references.
The later alias-search index has a different source date and different counts.

## Stable publication rules

- App builds and dataset versions are separate. Point [versions/index.json](versions/index.json)
  at the chosen committed snapshot; do not silently include uncommitted changes.
- Use immutable, version-specific directories and tags. Never replace their
  bytes or move their tags; issue a new dataset identity for changed contents.
- Include the complete adapted machine-readable database, pinned source
  information, notices, file sizes, SHA-256 values and read-only integrity checks.
- Verify anonymous downloads before calling a dataset available. Root documents
  can be updated while previously published snapshots remain unchanged.
- Keep unknown historical provenance explicitly unknown. Retaining old references
  means the adapted database may differ from a fresh upstream dump.
- Publish only the exact allowlisted files. Review database tables and the Git
  tree; never include personal collections, imports, activity, samples, models,
  private emails, signatures or credentials.

中文：本次已公开220版对应的实际曲库，73版仅保留历史元数据。数据目录和标签固定，
后续更新使用新的数据版本；不能将上游日期、App build与数据公开日期混为一谈。
