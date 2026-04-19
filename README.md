# Repolex Knowledge Graph of NMFR/optimize-css-assets-webpack-plugin

RDF knowledge graph data for [NMFR/optimize-css-assets-webpack-plugin](https://github.com/NMFR/optimize-css-assets-webpack-plugin), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download NMFR/optimize-css-assets-webpack-plugin
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── e896b9786d272323db70ced09ea4f2d8cbfc22ef
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── e896b9786d272323db70ced09ea4f2d8cbfc22ef.nq.gz
│   └── repolex
│       └── e896b9786d272323db70ced09ea4f2d8cbfc22ef
│           └── chunk-001.nq.gz
├── blob
│   ├── 03996099e5a4bfc1670d07060d2697070861c27e.nq.gz
│   ├── 03cb4adc7f8e88efdf7bc94d0733a9c40e313c49.nq.gz
│   ├── 060068b7d1b8183e7df35b62afb2f081f2472b2d.nq.gz
│   ├── 060a716e6b6aa7805cf52fca609fd69e84a0ec68.nq.gz
│   ├── 1234f95d623d45e8991472d21fdace0a745267b5.nq.gz
│   ├── 1284ba6ea7dfa95bec288b5f76f7659a7d2c0b78.nq.gz
│   ├── 167889f5db4fd34f6a8ade495eb6837711359935.nq.gz
│   ├── 1973738e1a0ba6ceeeed9cbdb97623293b1b3073.nq.gz
│   ├── 1ec829f02c256bc4ca896764ac1e5f654faa19e8.nq.gz
│   ├── 1eff4c2db0a0fa230f6b3cef28b19de5250a2ce7.nq.gz
│   ├── 3229bfdcba78db7764851a8c5cfdd49463a7ea68.nq.gz
│   ├── 3d11b7fc04471960f8864eb4a89849255b7156e3.nq.gz
│   ├── 424a74c49a2db04cd3764c9569ae8205d37f4574.nq.gz
│   ├── 4c8f5c627e451b44db13a397bea7635b655d5e59.nq.gz
│   ├── 55eb08a78c8fa35999a4fbd2162de77953c442e9.nq.gz
│   ├── 5d659bfb02e244387f2c21272fa3f979d73e1011.nq.gz
│   ├── 8c584564c00ea4e42805d5b9ef57bbc106f82017.nq.gz
│   ├── 8e7ce09f34d5e601c080b92363ed35171a91c13a.nq.gz
│   ├── a26aba2efc628c7cdc840ef67e244ef9fca8503c.nq.gz
│   ├── a286d3e3242fc1b1ed171c1a372564197713b1af.nq.gz
│   ├── a2a7578acce6aa3f5b39a76c89b35a29c8f376de.nq.gz
│   ├── b1c34c279a8caf7df70f3aaa47e204c1cc1e3555.nq.gz
│   ├── b42f4b6e90b0500f27ebc98fba66f33f540fd2c9.nq.gz
│   ├── b69f093a85349181b4d09bc9d1490635a841a505.nq.gz
│   ├── bd4aa1845b12ad781f587d1b7a1b462617905f1e.nq.gz
│   ├── c97baf7feaea685c12cb1287c52666f17c9a7cf9.nq.gz
│   ├── ce9d7bb08c6849477b6d868852dab43975e68408.nq.gz
│   ├── d889e4ce9a852b4b226641477e2bc1dc8f10ef6f.nq.gz
│   ├── e2dbd7e54602fac210784f40340dce0b9eab3ce5.nq.gz
│   ├── ea3e09eec566bef0e1b70070b543389ccc6f36fb.nq.gz
│   ├── eb6fe16cba376577168d7a34e7c0c224f2ee78d8.nq.gz
│   ├── ec063b3100a60a97383e66fb554c9e706c00c6c7.nq.gz
│   ├── ed4e5ad0a20051dc6d168cb62525c3bb08978054.nq.gz
│   └── f576af5f55008a79efc6e5903b1765ed422bfbf8.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── e896b9786d272323db70ced09ea4f2d8cbfc22ef.nq.gz
├── filetree
│   └── e896b9786d272323db70ced09ea4f2d8cbfc22ef.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 44 files
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

## Source repository

[NMFR/optimize-css-assets-webpack-plugin](https://github.com/NMFR/optimize-css-assets-webpack-plugin)

---
*Parsed on 2026-04-19 by [repolex](https://repolex.ai)*
