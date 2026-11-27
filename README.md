# TradMate-library-data

Public, versioned tune-library data, provenance, attribution and licenses for
TradMate. The application source remains private.

**The complete adapted SQLite catalog is now available.** This snapshot matches
the latest committed TradMate main revision checked on 2026-11-27:
**1.0.3 (build 220), `823fbf4cb594`**. App builds, upstream data dates and dataset
publication dates are separate; later uncommitted local app changes are excluded.

## Download

- [Download the SQLite database](https://raw.githubusercontent.com/andyxuhang/TradMate-library-data/library-build220-9272ecb3f8ea/datasets/build220-9272ecb3f8ea/tradmate_library.db) — 34,881,536 bytes (33.27 MiB).
- [Complete snapshot: database, alias/publisher indexes, change ledger and notices](datasets/build220-9272ecb3f8ea/).
- [Version manifest](versions/build220.json) · [Checksums](datasets/build220-9272ecb3f8ea/SHA256SUMS) · [Verification](VERIFY.md).
- Immutable dataset tag: [`library-build220-9272ecb3f8ea`](https://github.com/andyxuhang/TradMate-library-data/tree/library-build220-9272ecb3f8ea).

| Catalog records | Count |
| --- | ---: |
| Tunes | 23,423 |
| Settings / ABC versions | 55,412 |
| Aliases in the SQLite catalog | 29,595 |

The separate alias-search index contains 29,223 linked alias strings for 8,669
tune IDs, based on a later upstream snapshot. Its counts are not added to the
SQLite alias count. The publisher index also has its own coverage and provenance.

## Sources and license

Data originates from [The Session](https://thesession.org/) and
[adactio/TheSession-data](https://github.com/adactio/TheSession-data).
Read [attribution and component sources](ATTRIBUTION.md), the
[license scope](LICENSE.md), the [complete upstream license](licenses/TheSession-data_LICENSE.md),
and [version history](VERSIONING.md). The original license includes ODbL and
additional contents terms; it is preserved without removing its LLM restriction
or accessibility exception. TradMate is independent and is not an official or
endorsed product of The Session.

No application source, instrument samples, finished audio, album-cover images,
recognition models, private user collections, recordings, credentials or private
correspondence are included. The historical [build 73 metadata](versions/build73.json)
remains unchanged as an unpublished record from that time.

## 中文

已公开与主工程 Git 最新提交对应的 **1.0.3（220）完整适配曲库**，包含23,423首
曲目、55,412个版本，以及别名索引、发布者索引、差异表、完整许可证和校验值。
数据库主更新来源日期为2026-11-08；别名搜索索引来源日期为2026-11-15。
本次发布日为2026-11-27。App版本、上游数据日期与公开数据版本分别记录。
主程序保持私有；本地尚未上传的234版修改不包含在本快照内。
