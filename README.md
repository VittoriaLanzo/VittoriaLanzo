<div align="center">

**Vittoria Lanzo**

Agentic Systems Designer · OSS Contributor · ML Researcher

</div>

---

<h2><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="20" height="20" align="absmiddle"/> Merged OSS</h2>

<a href="https://github.com/PrefectHQ/prefect/pull/21707"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="16" height="16" align="absmiddle"/></a> **PrefectHQ/prefect · #21707** — `count_flow_runs` re-evaluated one correlated EXISTS subquery per filter per candidate row: O(k · N · log M) → O(N + ΣMᵢ) for both dialects.
> Explicit JOINs (N:1 foreign keys only, task runs excluded) · SQLite: 51–66× at 100k rows · PostgreSQL: up to 18× at 100k rows · 21 regression tests

<a href="https://github.com/PrefectHQ/prefect/pull/21004"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-merge-purple.svg" width="16" height="16" align="absmiddle"/></a> **PrefectHQ/prefect · #21004** — `prefect worker start` had no way to skip pool creation; operators hitting pre-existing pools got silent creation side-effects.
> Fix introduced `--no-create-pool-if-not-found` flag, eliminating the side-effect entirely · orchestrated end-to-end via multi-agent workflow

---

<h2><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="20" height="20" align="absmiddle"/> In Review</h2>

<a href="https://github.com/sktime/sktime-mcp/pull/126"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="16" height="16" align="absmiddle"/></a> <a href="https://github.com/sktime/sktime-mcp/pull/124"><img src="https://raw.githubusercontent.com/VittoriaLanzo/VittoriaLanzo/main/assets/git-pull-request-green.svg" width="16" height="16" align="absmiddle"/></a> **sktime/sktime-mcp · #126 + #124** — 5 bugs in `RegistryInterface` (2 race conditions, 3 correctness errors) → open, awaiting review
> Double-checked locking, 100% branch coverage, 7.8× throughput improvement (239ms → 31ms, cold-cache registry lookup)

---

## 🔬 Research

**[windowed-minority-guidance](https://github.com/VittoriaLanzo/windowed-minority-guidance)** — Submitted to EEML 2026 · admission pending (independent)
> Tested whether minority guidance (Um, Song & Lim, ICLR 2024) produces timestep-localized effects in diffusion denoising. Split the chain into 3 equal windows; mid-phase guidance recovered 45.6% of full-chain loss reduction across 250 iterations / 50 seeds on LSUN Bedroom. Wilcoxon signed-rank p < 0.001 for mid, early, and full guidance vs. baseline.

---

## 🥈 Hackathon

**MEGA Hackathon 2026 — Silver Medal (900+ participants)**

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
