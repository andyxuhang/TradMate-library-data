# Dataset version and release policy

## Current documentation version

2026-10-13: public repository initialized with license, attribution and version documents only. No database, model, index, sample or application package has been published.

[Build 73 metadata](versions/build73.json) describes the candidate associated with TradMate 0.31.73, build 73. App versions and dataset releases are separate: this documentation commit is neither a new App build nor a data release.

Candidate identity:

| Field | Local candidate |
|---|---|
| Database bytes | 36,794,368 |
| SHA256 | `d2ad4e72f96a1b6d2fcaaca98468fc51ae91ac853c0972adc20f908c422645b0` |
| Tunes | 23,300 |
| Settings | 54,997 |
| Aliases | 29,436 |
| Original upstream data revision | Unverified |
| Published dataset tag | None |
| Verified public database download URL | None |
| Rights and distribution confirmation | Pending |

## Future release requirements

Before any tune data is uploaded, confirm applicable source/content permissions, the custom upstream terms, required attribution and distribution conditions, and obtain approval for the actual publication.

An approved data release should include `tradmate_library.db`, a version-specific `dataset-manifest.json`, complete `LICENSE.md`, `ATTRIBUTION.md` and `SHA256SUMS`. Preserve unknown provenance fields as unknown. Do not invent original data revisions or transfer permission from one asset category to another.

Assign an immutable dataset tag tied to the App-compatible snapshot and full checksum. Do not create a dataset tag for a documentation-only placeholder. Verify the actual anonymous download, full database hash/size, read-only integrity and record counts, and include the complete notices. Only then record a real download URL and tag as published.

Corrections to provenance or rights status should have a dated new version rather than silently rewriting historical facts. Never overwrite an existing data release with different bytes under the same identity.

## Keep private content out

Do not upload the private application repository, user data, personal correspondence, signatures, recordings or keys. Models, retrieval/notation assets and soundbanks require their own rights evaluation and are not part of this initial publication.

Local ignore rules block common database, audio, model, binary and credential paths to reduce accidental uploads. They are a safeguard, not a permission decision. Any future approved data upload must explicitly change the relevant rule and review the exact files and entire Git history before pushing.

中文：版本说明和候选哈希已公开，数据库尚未发布。授权与分发条件确认后才创建真正的数据版本，并以匿名下载和完整校验作为发布依据；App build 不等于数据库版本。
