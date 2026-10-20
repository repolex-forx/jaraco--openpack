# Repolex Knowledge Graph of jaraco/openpack

RDF knowledge graph data for [jaraco/openpack](https://github.com/jaraco/openpack), parsed by [repolex](https://repolex.ai).

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
rlex download jaraco/openpack
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 0ac21d13f63af383b50677da7ac32481259aae19
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 0ac21d13f63af383b50677da7ac32481259aae19
│           └── chunk-001.nq.gz
├── blob
│   ├── 104f6cba1972bb416ad7a2e125ac0599700b36c9.nq.gz
│   ├── 10d412f406891b9683f832fcbc134c9bdf4f916e.nq.gz
│   ├── 18ade35d2e1059033cfc83bee7b2d530eb38f0c9.nq.gz
│   ├── 1f2aa7533b0423a8eb943f6f4ec02498e39581a0.nq.gz
│   ├── 2109bf9515ac0fdc6e2fea530ef1564238d0fded.nq.gz
│   ├── 270dc67a78dcd2b341c13a81666c25d08c12f214.nq.gz
│   ├── 2e3f4dd791a6372b427d618eb0baa8c4dc58e5f0.nq.gz
│   ├── 304196f81e11a168c9894f966e4a617ebf4ed53c.nq.gz
│   ├── 38ecf286e6f4a2ad7bbb1d903df3b511cd5ac0a3.nq.gz
│   ├── 3caae064f05df56682a882fac6e186c65766e8a7.nq.gz
│   ├── 4d282dfde395366887fdae6b7efa39e25963d5f5.nq.gz
│   ├── 54c9000ec94341dd65c2053251b85b124017b9b5.nq.gz
│   ├── 54cc8303b22089e12053e552d4e6cb852a865b8a.nq.gz
│   ├── 577e87a793a20e413f7321f4f17ec1eba2ea1962.nq.gz
│   ├── 5bdc232005af9be104a00437ae9bc64417a4c1cc.nq.gz
│   ├── 5be631096d821e790bc4911b9d8971002efcc34a.nq.gz
│   ├── 5df0be0058d9fee0fabf0b23c48d5415001131d3.nq.gz
│   ├── 63997b0aa841dd814ca0163db1550f3e83f3ea4b.nq.gz
│   ├── 700235be57c1b2872455c0be5333f59cf568e252.nq.gz
│   ├── 72258e6907b45468d117b620d45725c665e16db7.nq.gz
│   ├── 724370638fc188317bbc7dc868f1a571995fd796.nq.gz
│   ├── 79bd3a35559a9edfa93dfff5caff98b6cedd2f5b.nq.gz
│   ├── 7b466ff3dd9e9a37726563a85df0cd8cb102f5e7.nq.gz
│   ├── 7b7700bcec0820724a6437bb282664b46531ef71.nq.gz
│   ├── 86e5c5a1d504ef745ae4ac7efd7cd3dcfac19cc2.nq.gz
│   ├── 8dd04bcdb8113195a9624878de641fbc0ad044fa.nq.gz
│   ├── 959116de9f5fc5e60afa9598b86de3da5fd6a000.nq.gz
│   ├── 9a0f3bce1395ae3819030b822e5d9076c85068ea.nq.gz
│   ├── 9c5a1f9fc8ba5a08c3015c84534739d4f3eb8281.nq.gz
│   ├── 9f28d4fa6ef333c0b83f84770637e98d4057650c.nq.gz
│   ├── a275cf417e01a78f9562b1b13725a404f234d5d1.nq.gz
│   ├── b0f4e6153a7ffc94d106e594b7fb6995d3c0a58b.nq.gz
│   ├── b420162d01a4b9f2f9328d0a60415449a7b7545b.nq.gz
│   ├── c908f686212ff93988de95f34f4ec51c6a73e1cb.nq.gz
│   ├── db8f076050090959aa9efdf4fc2954bb5cad4abd.nq.gz
│   ├── dd3f5ccde67497c4af7512b1fc3a4e74af6136bd.nq.gz
│   ├── e05a3d4a2ab888e32952006d8cd380864368db5f.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e75b04c9e8d44e6ccc65db6928eadec1c4083003.nq.gz
│   ├── ed0c85eb91e333ea239369c27ddc3d8d7b737348.nq.gz
│   ├── fbd540c1e0495c9412fe2436705fb7338262a56a.nq.gz
│   └── fc68174e8a1fc80ff0ad93d127c29846c6926d1f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 0ac21d13f63af383b50677da7ac32481259aae19.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 50 files
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

[jaraco/openpack](https://github.com/jaraco/openpack)

---
*Parsed on 2026-10-20 by [repolex](https://repolex.ai)*
