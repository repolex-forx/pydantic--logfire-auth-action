# Repolex Knowledge Graph of pydantic/logfire-auth-action

RDF knowledge graph data for [pydantic/logfire-auth-action](https://github.com/pydantic/logfire-auth-action), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download pydantic/logfire-auth-action
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 5bc43913fd88758f7974d7c7ca857001e2b628d2
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 5bc43913fd88758f7974d7c7ca857001e2b628d2
│           └── chunk-001.nq.gz
├── blob
│   ├── 112c596d1dc03753d2f135a5ccbdaacf9ab02716.nq.gz
│   ├── 12495d67fd96c8d233b9bd0580cc59f7bb3c9ad0.nq.gz
│   ├── 12926387ff44df9975f69a80d207de538bddbfb2.nq.gz
│   ├── 18478371a97bddd6b4762206dbb54ddafa5b3918.nq.gz
│   ├── 1c215d290e7095509d00a3924ce82bd7abb9b03f.nq.gz
│   ├── 20cf255d188c5d49da99d3249be94cc3cbfc9f06.nq.gz
│   ├── 29b951dcb6dfa5f9d1693e7886f307d94fcb4d8b.nq.gz
│   ├── 3bbc5e3140417036b29491797ffe0f8e2423b1b1.nq.gz
│   ├── 4386e904c14fbe5b14e9f3f69d6bb83ff5893867.nq.gz
│   ├── 473d195b58c6aff76de641d8d3f97cf997f2140f.nq.gz
│   ├── 4bf6c01d405de121b4301c4c4c3bb2c0ed6686ca.nq.gz
│   ├── 4ddaff1a62c69565f3be182ea1a8e84efe2de451.nq.gz
│   ├── 530f25922d9cacd8beb3261f36c78dd3e728cba2.nq.gz
│   ├── 6752dba41a365f93e524e1b0c1c31607fe82c75f.nq.gz
│   ├── 71843cd299154fd26e286f33620ec62481b06bbe.nq.gz
│   ├── 863ebd1ba75bf1d8ec8858ef1ddf7e13bd9745d2.nq.gz
│   ├── 8dd18b7fbef16b0db2ea0d61c266bd296dec6eba.nq.gz
│   ├── 9a378462ec0d9a484102c90b127d13176bea7b61.nq.gz
│   ├── 9c225e7e2d8add2587d5cc26b22f379e7b4e5106.nq.gz
│   ├── a45fd52cc5891570d6299fab38643103c3955474.nq.gz
│   ├── a925775db1f1984316cd4e2b2b5f82df2af50d51.nq.gz
│   ├── b2d1f452eda011386e836009a7d4ce1192425d3e.nq.gz
│   ├── b54e05bfd0e840c8cce0f1a09b7d465aca70d928.nq.gz
│   ├── c37443b8a9545996961e87eae8be7fd9c9a16f50.nq.gz
│   ├── c7cf6138e24cd59bb6fc56da5d5495fc1e43421e.nq.gz
│   ├── dc14bbb9a9c8cf70482c3ba557c27baee6cd4d64.nq.gz
│   ├── e4c81e38bdc6162da1b117fed8793f5e41c3e0ad.nq.gz
│   ├── e78a706dec13f2991af5913f158365d1a8d6a7f7.nq.gz
│   ├── ef973ffda15e3fa7055f7eb1b08855a179dfe67b.nq.gz
│   └── fd0e085b76b00395f9f43c59140d98ac09570026.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 5bc43913fd88758f7974d7c7ca857001e2b628d2.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 37 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[pydantic/logfire-auth-action](https://github.com/pydantic/logfire-auth-action)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
