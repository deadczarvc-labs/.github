<div align="center">

# deadczarvc labs

**Evidence-first tooling for coding agents: context compaction that keeps the facts, measured on blind held-out data.**

[Projects](#projects) · [How we work](#how-we-work) · [Contributing](https://github.com/deadczarvc-labs/.github/blob/main/CONTRIBUTING.md) · [Security](https://github.com/deadczarvc-labs/.github/blob/main/SECURITY.md)

</div>

## Projects

| Project | What it does | Latest |
|---|---|---|
| [jev-factkeep-compaction](https://github.com/deadczarvc-labs/jev-factkeep-compaction) | Claude Code plugin. Jev-guided context compaction that never erases a tool call: reproducible reads shrink to a note, observations keep their errors, ids, codes and counts. A fork of [tamaratran/fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction). | [0.3.0-astra.7](https://github.com/deadczarvc-labs/jev-factkeep-compaction/releases/latest) |
| [hermes-jev-compaction](https://github.com/deadczarvc/hermes-jev-compaction) | The same rules as a context engine for [Hermes Agent](https://github.com/NousResearch/hermes-agent). | [v0.6.0](https://github.com/deadczarvc/hermes-jev-compaction/releases/latest) |

On blind held-out rounds the compaction rules kept 304 of 336 preregistered facts, against 36 for the original
engine. The analysis, with per-call data and a script that recomputes every number:
[why facts are lost](https://github.com/deadczarvc-labs/jev-factkeep-compaction/blob/main/docs/why-facts-are-lost.md).

## How we work

- **Claims come with data.** Measurements are preregistered before any run, repeated, and published with the tables
  and scripts needed to recompute them.
- **Upstream first.** Fixes go back to the original project as pull requests, for example
  [tamaratran/fast-jev-compaction#118](https://github.com/tamaratran/fast-jev-compaction/pull/118).
- **Forks stay compatible.** A fork keeps the upstream license, history and plugin names, so it can replace the
  original without reconfiguration.
- **Known limits are stated.** Every release lists what it still loses.
