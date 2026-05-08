<div align="center">

**Vittoria Lanzo**

Agentic Systems Designer · OSS Contributor · ML Researcher

</div>

---

<h2><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="20" height="20" align="absmiddle"/> Merged OSS</h2>

<a href="https://github.com/PrefectHQ/prefect/pull/21707"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="16" height="16" align="absmiddle"/></a> **PrefectHQ/prefect · [#21707](https://github.com/PrefectHQ/prefect/pull/21707)** — `count_flow_runs` re-evaluated one correlated EXISTS subquery per filter per candidate row: O(k · N · log M) → O(N + ΣMᵢ) for both dialects.
> Explicit JOINs (N:1 foreign keys only, task runs excluded) · SQLite: 51–66× at 100k rows · PostgreSQL: up to 18× at 100k rows · 21 regression tests

<a href="https://github.com/PrefectHQ/prefect/pull/21754"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="16" height="16" align="absmiddle"/></a> **PrefectHQ/prefect · [#21754](https://github.com/PrefectHQ/prefect/pull/21754)** — `read_block_schemas` performed a linear `next()` scan of flat results for every nested reference lookup: O(N<sup>2</sup>) → O(N). for bulk reads.
> Implemented a `checksum_index` dictionary with first-wins semantics to achieve O(1) lookups · ~125× speedup at 1,000 schemas (55.9ms → 0.39ms p50) · 12 new tests covering index threading and collision parity

<a href="https://github.com/PrefectHQ/prefect/pull/21004"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="16" height="16" align="absmiddle"/></a> **PrefectHQ/prefect · [#21004](https://github.com/PrefectHQ/prefect/pull/21004)** — `prefect worker start` had no way to skip pool creation; operators hitting pre-existing pools got silent creation side-effects.
> Fix introduced `--no-create-pool-if-not-found` flag, eliminating the side-effect entirely · orchestrated end-to-end via multi-agent workflow

---

<h2><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="20" height="20" align="absmiddle"/> In Review</h2>

<img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="16" height="16" align="absmiddle"/> **sktime/sktime-mcp · [#126](https://github.com/sktime/sktime-mcp/pull/126) + [#124](https://github.com/sktime/sktime-mcp/pull/124)** — 5 bugs in `RegistryInterface` (2 race conditions, 3 correctness errors) 
> Double-checked locking, 100% branch coverage, 7.8× throughput improvement (239ms → 31ms, cold-cache registry lookup)

<img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="16" height="16" align="absmiddle"/> **SWE-agent/mini-swe-agent · [#821](https://github.com/SWE-agent/mini-swe-agent/pull/821)** — `FormatError` discarded the raw model response on parse failure; trajectory logs showed the error marker but nothing to inspect
> `try/except FormatError` in all 7 model `query()` wrappers · `repr()` fallback when `model_dump()` fails · 16 regression tests

<img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="16" height="16" align="absmiddle"/> **fastapi/fastapi · [#15476](https://github.com/fastapi/fastapi/pull/15476)** — `jsonable_encoder` built `set(obj.keys())` unconditionally on every dict branch, causing pure overhead when `include` and `exclude` filters were `None`  
> Skipped set allocation and membership tests when filters are absent · 8.2% wall-time reduction on small dicts (5.37 µs → 4.93 µs) · 6.0% reduction on large nested dicts · 7 regression tests added
--- 

## 🔬 Research

**[windowed-minority-guidance](https://github.com/VittoriaLanzo/windowed-minority-guidance)** — Submitted to EEML 2026 · admission pending (independent)
> Tested whether minority guidance (Um,Lee & Ye , ICLR 2024) produces timestep-localized effects in diffusion denoising. Split the chain into 3 equal windows; mid-phase guidance recovered 45.6% of full-chain loss reduction across 250 iterations / 50 seeds on LSUN Bedroom. Wilcoxon signed-rank p < 0.001 for mid, early, and full guidance vs. baseline.

---

## 🥈 Hackathon

**MEGA Hackathon 2026 — Silver Medal (900+ participants)** <a href="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/mega-hackathon-cert.png" title="View Certificate"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/mega-hackathon-cert.png" width="18" height="18" align="absmiddle" alt="Certificate"/></a>

Built [**Sestara**](https://sestara.lovable.app) in-contest: AI study roadmap platform (personalized paths, flashcards, quizzes, study assistant) addressing SDGs 4 · 10 · 11 · 16. Stack: React · TypeScript · Vite · Supabase · Google Gemini · shadcn/ui · Framer Motion · Wolfram Alpha LLM.

---

## 🛠 Tech Stack

**Languages**

[![Languages](https://skillicons.dev/icons?i=python,c,mysql,latex,bash)](https://skillicons.dev)

**Multi-agent Systems**

![Claude Code](https://img.shields.io/badge/Claude_Code-CC785C?style=flat-square&logo=anthropic&logoColor=white)
<img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/antigravity-logo.png" height="20" alt="Antigravity"/>

**Dev Environment**

[![Dev](https://skillicons.dev/icons?i=vscode,debian,docker,raspberrypi,git)](https://skillicons.dev)

**Creative**

[![Creative](https://skillicons.dev/icons?i=figma,canva)](https://skillicons.dev)

**Infrastructure**

[![Infra](https://skillicons.dev/icons?i=githubactions,supabase)](https://skillicons.dev)

---

<div align="center">

17 · Cesena, Italy · [vittoria3103.123@gmail.com](mailto:vittoria3103.123@gmail.com) · [vittorialanzo.vercel.app](https://vittorialanzo.vercel.app)

</div>
