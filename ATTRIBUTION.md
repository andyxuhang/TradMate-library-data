# TradMate tune library attribution

Contains information from [The Session](https://thesession.org/), made available
under the [complete TheSession-data license](licenses/TheSession-data_LICENSE.md).
TradMate is independently developed and is not an official or endorsed product
of The Session. See the [license scope](LICENSE.md) for the separate asset scopes.

## Current published snapshot

[TradMate 1.0.3 build 220](datasets/build220-9272ecb3f8ea/) is exported byte-for-byte from
committed app assets at `823fbf4cb5941394d86b5dd476ba46cc6e891f47`. It is a complete adapted catalog, not an exact
copy of a single upstream dump and not the uncommitted local working tree.

| Component | Pinned upstream inputs | Coverage |
| --- | --- | --- |
| SQLite catalog, ABC and default popularity | `json/tunes.json`, `json/aliases.json`, `json/tune_popularity.json` at [`b3e7ba2c4a8f`](https://github.com/adactio/TheSession-data/tree/b3e7ba2c4a8f63a9fedb4518c1f0b0cfa279b088) (2026-11-08) | 23,423 tunes / 55,412 settings / 29,595 catalog aliases |
| Alias-search index | [`csv/aliases.csv`](https://github.com/adactio/TheSession-data/blob/511872c0565b46e929780928a70417694933fdbf/csv/aliases.csv) at `511872c0565b` (2026-11-15) | 29,223 linked strings / 8,669 tune IDs |
| Tune/setting publisher index | `csv/tunes.csv`, `csv/sets.csv`, `json/tunes.json` at the catalog update revision above | Counts and source hashes in the manifest |
| Catalog change ledger | Comparison of the previous adapted catalog and the updated catalog | 1,073 changed existing setting references; additions excluded from that count |

The [machine-readable manifest](versions/build220.json) records full revisions,
input hashes, packaged-file hashes, sizes and coverage. The license originally
copied from [`1d2bc823fd8f`](https://github.com/adactio/TheSession-data/blob/1d2bc823fd8f0f969b267df6c4713ab08ddccbe3/LICENSE.md)
is preserved unchanged. A license revision is not the original data revision.

## Adaptation and identifiers

The 2026-11-09 update retained stable local catalog IDs and existing setting
paths, including historically reassigned or absent upstream records. Source
tune IDs, source setting IDs and local IDs identify different things; a tune
can have several settings. Consult the manifest's table schema before joining.
The initial 2026-09-19 import's exact upstream revision remains unverified.
The full adapted bytes are supplied, so no claim of a fully reproducible fresh
upstream-only reconstruction is needed or made.

Popularity comes from public tunebook counts. Default stars are the number of
thresholds reached among `10, 19, 45, 135, 438`; they are not direct five-star
reviews from The Session. `rating_history` holds previous bundled defaults to
support upgrades, not a user's ratings or activity. Search aliases retain their
original public strings; matching normalization happens in the private app.
Runtime automatic score repairs are not written into this database snapshot.

## Scope

The complete upstream text contains ODbL and separate contents terms, including
the LLM restriction and accessibility exception. Database licensing is distinct
from rights in individual compositions, settings and arrangements. Publication
does not relabel every tune as public domain or grant rights in the app itself.
The additional [Unicode notice](licenses/Unicode_Tune_Search_LICENSE.txt) concerns
the app's Unicode search tables; it does not license The Session contents.

Personal favorites, learning levels, sets/setlists, imports, analytics, recordings,
private permission correspondence, signatures, soundbanks and models are excluded.

中文：曲库、搜索别名及发布者索引分别标明来源和版本。主曲库保留已有本地引用，
不是单次上游导出的原样副本；初次导入的历史来源仍保留未知状态。星级来自公开收藏
数量转换，历史星级表是内置默认数据，不是用户资料。完整许可与署名须随数据保留。
