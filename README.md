# Repolex Knowledge Graph of blitz-js/superjson

RDF knowledge graph data for [blitz-js/superjson](https://github.com/blitz-js/superjson), parsed by [repolex](https://repolex.ai).

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
lexq download blitz-js/superjson
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 4e708c11b8ae510008c42fbc445ff0e0e683417e
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 4e708c11b8ae510008c42fbc445ff0e0e683417e.nq.gz
│   └── repolex
│       └── 4e708c11b8ae510008c42fbc445ff0e0e683417e
│           └── chunk-001.nq.gz
├── blob
│   ├── 009da4668975025ca5a0462e9662fb0394fe3b8c.nq.gz
│   ├── 0b63577fa3abed7eeb6fb563ddf965c3c31a10b1.nq.gz
│   ├── 13a5288c11ed5beebc71b5e2a55260e4789ca3b4.nq.gz
│   ├── 20b106df1d0cac47752574c117c047fec83349b3.nq.gz
│   ├── 27894cb5631e9f97e8a8dace9c9265c0b5aa85af.nq.gz
│   ├── 28b8766f36cfab2f19936e41fdf31b1f87e3a352.nq.gz
│   ├── 31354ec1389994b5f6708c7d915fdcc6bb76ba6e.nq.gz
│   ├── 349f0d56dfd5cfc026865ba45f74cf630028fcb9.nq.gz
│   ├── 35b1a725fdec58d4119b855445ef6e52619dadef.nq.gz
│   ├── 438ea498f206bf94b0a64d6276dadb538b98afc1.nq.gz
│   ├── 44ccd11d6939c0f132f6938c05775e7004795f36.nq.gz
│   ├── 532ad1287a4ea5874c58ef58f1b8dabc18ce1b25.nq.gz
│   ├── 5e64fad1849923814806c2e1d4dbdee726f0ef90.nq.gz
│   ├── 5f8e5e41675e74b1016d1145153926bb67d1065a.nq.gz
│   ├── 67774dfa6b0b6a9f9ebd5a5d0b38ca25d2813713.nq.gz
│   ├── 6dff1e52eb7d76268ff814417f6ef02e0dea00c8.nq.gz
│   ├── 7217f9db309bd9ac5200b9dac5fb15898de2873b.nq.gz
│   ├── 73fd6b72520a7be1c3694dea0742c038b5e4e4a7.nq.gz
│   ├── 8383605a3127380a1e6fd74e9986560f923c789a.nq.gz
│   ├── 8e9059f1e61858abb30939ad78f47e53e276d987.nq.gz
│   ├── 9a11ad74456e11ca4a707c6a856ef272fa71288c.nq.gz
│   ├── 9ff5d3290ff639acc345e98a32e7a27c5ad9f9ca.nq.gz
│   ├── a007127588f6d01b4959575f9506260af088cd5e.nq.gz
│   ├── a2f9a256aa7eba8b3cba71f53d3a243f8fcbafa5.nq.gz
│   ├── ab7e017442f033ac19173928865cd1487b235c64.nq.gz
│   ├── ac8ffdfbdb652401baa88068f319a5a9db1a32d1.nq.gz
│   ├── b24081276914fb25a3a712c1d86856435d2e3b42.nq.gz
│   ├── b6ef6e4e90b7525a7e2ac732c5a3f1e47bd8c696.nq.gz
│   ├── c25bf745df01a7161881289416775726eddab962.nq.gz
│   ├── c48a015e17c3df43088b87e7f9b0c72745babd2c.nq.gz
│   ├── d98b6b7980283ae73a87edcdfcbaa707825b8cb3.nq.gz
│   ├── e84162b04ee43689b026eb573e71cbc3c5da516b.nq.gz
│   ├── e8cf5bbefdc3ca7364a9584854162cb4e653899b.nq.gz
│   ├── ea986130c395928467c369b7c9c00d7856e2175d.nq.gz
│   ├── ebd3db6a6175d5c611f176d66041ba923c7311f2.nq.gz
│   ├── efbf867dc2370a26359780b9d1c013a410c144a4.nq.gz
│   └── f0c5c5d0fc80c68650e5dd9714237e1cdc376d41.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 4e708c11b8ae510008c42fbc445ff0e0e683417e.nq.gz
├── filetree
│   └── 4e708c11b8ae510008c42fbc445ff0e0e683417e.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 47 files
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

[blitz-js/superjson](https://github.com/blitz-js/superjson)

---
*Parsed on 2026-09-17 by [repolex](https://repolex.ai)*
