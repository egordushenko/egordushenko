# Egor Dushenko

AI Engineer / AI-first Developer focused on LLM integrations, automation, and full-cycle product development.

I build practical AI-powered products end-to-end: product logic, architecture, backend, LLM pipelines, payments, deployment, and iteration.
My work is focused on using LLMs as engineering tools to ship real products faster, not as decoration.

## Selected Projects

### [Alterega Platform](https://github.com/egordushenko/alterega-platform)

Architecture showcase for a commercial ecosystem of video-editing tools for Adobe Premiere Pro and After Effects, built and operated solo.

Three product lines across five builds (AEGACut plugin and desktop, AEGAPanel, AEGA Sync for Premiere and After Effects), a central licensing service, payment pipeline, storefront, and Telegram-based delivery. Actively operated in production.

Frontend case study: [Alterega Storefront](https://github.com/egordushenko/alterega-storefront) — public frontend-only showcase of the real commercial storefront, built with Next.js, React, TypeScript, Tailwind CSS, Framer Motion, Three.js / React Three Fiber, and next-intl.

**What it demonstrates:**

* full-cycle commercial product engineering as a single operator
* HWID-bound licensing core shared across five product builds
* Adobe CEP panel development with ExtendScript and Python sidecars
* Electron desktop packaging on Windows
* server-side payment confirmation pipeline (Robokassa) with Telegram and SMTP delivery
* frontend storefront architecture: multilingual catalog, product modals, SEO, motion, and 3D hero scene
* VPS operations: Nginx, systemd, PostgreSQL, GitHub Actions

**Stack:** Node.js, Fastify, Next.js, React, TypeScript, Tailwind CSS, Framer Motion, Three.js, Python, Electron, Adobe CEP, ExtendScript, PostgreSQL, ffmpeg, Linux VPS.

Website: [alterega.ru](https://alterega.ru)

---

### [Redmine AI Technical Planner](https://github.com/egordushenko/redmine-ai-technical-planner)

AI automation tool for engineering teams.

It reads a Redmine issue, resolves the related Git repository, selects relevant files, asks an LLM for a technical implementation plan, and posts the result back to Redmine.

**What it demonstrates:**

* repository-aware LLM automation
* context selection under token limits
* Redmine REST API integration
* safe handling of untrusted issue text
* Docker-based local demo
* tests, linting, and practical CLI workflow

**Stack:** Python, Redmine REST API, OpenAI-compatible LLM API, SQLite, Docker, pytest, ruff.

---

### [goload](https://github.com/egordushenko/goload)

HTTP load-testing CLI with multi-step YAML scenarios — a systems-engineering piece in idiomatic Go.

Benchmarks a single endpoint or drives a full virtual-user flow: login, extract a token from one response, chain it into the next request, and fan out parallel calls inside one session. Reports to terminal, JSON, and a standalone HTML page.

**What it demonstrates:**

* idiomatic Go and concurrency design (producer → worker pool → single-writer collector, no locks on the hot path)
* `context.Context`-driven cancellation, duration limits, and RPS throttling
* CLI engineering with Cobra and a focused internal-package architecture
* a feature competitors lack: multi-step scenarios with response chaining and in-flow parallelism
* race-enabled tests and cross-platform CI (Linux, macOS, Windows) with golangci-lint

**Stack:** Go, Cobra, net/http, html/template, YAML, GitHub Actions.

---

### [CardBot](https://github.com/egordushenko/CardBot)

Telegram bot for generating marketplace product cards for Wildberries and Ozon sellers.

The bot generates SEO titles, descriptions, keywords, characteristics, and AI product images from ordinary product photos and a short text prompt.

**What it demonstrates:**

* LLM-powered product generation pipeline
* AI image generation workflow
* Telegram bot product UX
* payments, trial logic, and user balance system
* cost optimization through combining multiple product photos into one model input
* full product cycle from idea to launched bot

**Stack:** Python, Telegram Bot API, PostgreSQL, OpenRouter, DeepSeek, GPT Image, payment integration.

---

### [PAI Methodology](https://github.com/egordushenko/pai-methodology)

A typed knowledge-ops methodology for running a solo multi-product operation. Documents the system that backs the Alterega platform: typed separation between identity, applications, projects, research, stacks, and tasks; explicit source-of-truth boundaries; privacy auditing and context recovery for agent-assisted work.

**What it demonstrates:**

* operational maturity beyond product code
* designing systems that scale a single engineer across multiple shipping products
* agent-ready knowledge architecture (ISA, privacy zones, context search, instruction diet)

---

## Tech Stack

- **Languages:** Python, TypeScript, JavaScript, Node.js
- **Backend / Data:** PostgreSQL, REST APIs, FastAPI / Fastify, Next.js, Telegram Bot API
- **AI / LLM:** OpenRouter, GPT / Claude / Gemini, GPT Image, structured output, prompt engineering, LLM orchestration, AI automation
- **Infra:** Linux, Ubuntu, Nginx, Docker, GitHub Actions, VPS, systemd
- **Workflow:** Codex, Claude Code, MCP servers, agentic coding workflows

---

## Links

- Website: [alterega.ru](https://alterega.ru)
- Telegram: [@alterega](https://t.me/alterega)
