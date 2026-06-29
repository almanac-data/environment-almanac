# Environment Almanac

[![CI](https://github.com/almanac-data/environment-almanac/actions/workflows/ci.yml/badge.svg)](https://github.com/almanac-data/environment-almanac/actions/workflows/ci.yml)
[![good first issues](https://img.shields.io/github/issues/almanac-data/environment-almanac/good%20first%20issue?label=good%20first%20issues&color=7057ff)](https://github.com/almanac-data/environment-almanac/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22)

**An open, versioned index of public environmental data — so the record stays findable when the websites move.**

Environment Almanac is a **catalog, not a data warehouse**. Each entry is a small, human-reviewed,
machine-validated record pointing to an authoritative public dataset — its canonical source,
how to access it, where it's archived, and whether it is still reachable today. A daily job
re-checks every source and opens an issue when one goes dark.

It covers EPA and USGS data — air quality, toxic chemical releases, environmental enforcement, and water quality — the datasets researchers, journalists, and communities rely on.

## What's in the catalog

`catalog.json` is the machine-readable index; browse `catalog/` for the human-readable source.
The catalog starts with a few seed datasets (EPA Air Quality System (AQS), Toxics Release Inventory (TRI), Enforcement and Compliance History Online (ECHO), AirNow, Water Quality Portal) and grows by contribution.

## Contributing

You don't need to write code: **[suggest a dataset](../../issues/new/choose)** with a short form
and a curator will turn it into an entry. Prefer a PR? Adding a dataset is one file in `catalog/` —
see [CONTRIBUTING.md](CONTRIBUTING.md). CI validates every entry against the schema.

Stewards: see [docs/STEWARDING.md](docs/STEWARDING.md).

## The one rule

**Catalog, don't host.** This repo maps data; it does not store data bytes. See [AGENTS.md](AGENTS.md).

## License

- **Catalog data** (`catalog/`, `catalog.json`) — [CC0 1.0](LICENSE-DATA). Per-dataset licenses are
  recorded in each entry's `license` field.
- **Tooling** (`scripts/`, schema, CI) — [MIT](LICENSE-CODE).

---

A vertical of [The Almanac](https://github.com/almanac-data) — a community-maintained commons for
public data worth keeping findable. Built from [almanac-template](https://github.com/almanac-data/almanac-template).
