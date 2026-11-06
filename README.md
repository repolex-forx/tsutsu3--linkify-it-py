# Repolex Knowledge Graph of tsutsu3/linkify-it-py

RDF knowledge graph data for [tsutsu3/linkify-it-py](https://github.com/tsutsu3/linkify-it-py), parsed by [repolex](https://repolex.ai).

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
rlex download tsutsu3/linkify-it-py
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 84af472a80932acaa102d016383fdd94f3c7743e
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 84af472a80932acaa102d016383fdd94f3c7743e
│           └── chunk-001.nq.gz
├── blob
│   ├── 0f717ba78c2b4cbf87ffafefdf320ed8c12f6b2d.nq.gz
│   ├── 2679c757794d33847fce23252b1fd6345c9dd415.nq.gz
│   ├── 273185b2c7b1c1ad3e5832ceda0797fbbbd70343.nq.gz
│   ├── 29b2a9ba4468c9b5e86eb7f4a63956903a1b6634.nq.gz
│   ├── 3102ac718ecb8658fb1b15689f4f82284e63e0df.nq.gz
│   ├── 3c2e4de33f5610829ee51b7100cae6c03f5acb16.nq.gz
│   ├── 3f2f99d8cc996c4c0671a789f7141f7b17152135.nq.gz
│   ├── 410f275e7b2ee3a6f4935c61b1d4f14df4b41bbd.nq.gz
│   ├── 47860603e059d812e438f5d3343ef39a725fa63c.nq.gz
│   ├── 645cb53b14ebb99635676ede700eaa6c7b055027.nq.gz
│   ├── 6810e586f8780f4d898c8da407514c2bd5f059ec.nq.gz
│   ├── 6c06b6503b97f12eb88895a2d62612a02b54d0d1.nq.gz
│   ├── 75603474589cc0c89b4ab086979ddbb2243a8ceb.nq.gz
│   ├── 797cd7694e8a75fce2696b0b903fe6c611338602.nq.gz
│   ├── 79bf2970fed75d87b63d120f1e58c2c40e30bc67.nq.gz
│   ├── 7cab9564a3738978adaf3f3e7bdb39ec5d66754a.nq.gz
│   ├── 7f156f3e783ae4007224f0e411b23582e6ecdecf.nq.gz
│   ├── 8ef7eeceec3c7a76936d2c85036e1a1602b51f8f.nq.gz
│   ├── 9191f1dc8926828b805539878554c4e7656edb58.nq.gz
│   ├── 922152e96a04a242e6fc40f124261d74890617d8.nq.gz
│   ├── 9436c8de3e87f058ba6f14700db5374633c41f87.nq.gz
│   ├── 9cad9c8b39f1d5bd6df46413bbfd626bf375e3f1.nq.gz
│   ├── 9ec9a62d9e9bf3545e25dd68fdead0b69b21e650.nq.gz
│   ├── 9f2f833f362c6ddee512bceb572ba29c2d49349a.nq.gz
│   ├── a0140d1b7158775e1bd45ae2b08a2555158823d7.nq.gz
│   ├── a85db292f04e1883d18b7b978b93564aaf5918c9.nq.gz
│   ├── acb88a3c1cf2250b7f727fa841643acaa001bb5e.nq.gz
│   ├── aed2885a7b22704d8c64f62947a38f5a79ee0ec1.nq.gz
│   ├── b9474769b3aa4aeb1f46738528d5b8c4664addce.nq.gz
│   ├── bec37b16cdf3b1ea4c597d16062619b1db41e9e5.nq.gz
│   ├── bfc6e1069f77f78148b023db72b5f9297b1c1fbb.nq.gz
│   ├── c14a5dd623ea37170ea5bf4f2a460860be5361ad.nq.gz
│   ├── c1507ea29d7e2f3704c84c68169a8303dcbcb130.nq.gz
│   ├── c2c26c4db9e72ee408799b67034846ae8aa5caee.nq.gz
│   ├── c8bffb11be6689d0fa7625872e183fa0e9609677.nq.gz
│   ├── d4bb2cbb9eddb1bb1b4f366623044af8e4830919.nq.gz
│   ├── da3fefbb00a68de776412915dd617c0af01df227.nq.gz
│   ├── deb8c86672bb8efb1972f0c73566f2962b5e1c62.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ee5163bd6fba379534eb269dffb0428f613306d2.nq.gz
│   └── f32856ad1652157d5a5d1877071e18de01455bae.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 84af472a80932acaa102d016383fdd94f3c7743e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[tsutsu3/linkify-it-py](https://github.com/tsutsu3/linkify-it-py)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
