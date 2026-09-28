# Changelog — `toxi-db`

Per-crate history extracted from the monolith changelog
([meshackbahati/toxi](https://github.com/meshackbahati/toxi/blob/main/CHANGELOG.md)),
which remains the full documentation hub.

## [3.1.1] - 2026-09-28

- **toxi-db** (`3.1.1`): `QueryCache::get` serves hits under a single
  shared read plus the recency write instead of three acquisitions
  with a re-read. Adds `cache_get_hit` / `cache_get_miss` divan benches.
