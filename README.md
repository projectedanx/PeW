# Prompt Engineering Workbench

> A research-to-implementation platform for systematic prompt engineering — translating advanced framework theory into a structured, interactive application.

[![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)](https://nextjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.2-blue?logo=typescript)](https://www.typescriptlang.org)
[![Prisma](https://img.shields.io/badge/Prisma-6.7-2D3748?logo=prisma)](https://www.prisma.io)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.3-38BDF8?logo=tailwindcss)](https://tailwindcss.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## Overview

The Prompt Engineering Workbench (PEW) is an open research platform that bridges the gap between prompt engineering theory and practice. It provides interactive tools for each of its core framework areas — from structural prompt composition to context-execution pipeline simulation — backed by a rigorous research corpus of 50+ prompting methodology studies.

The project was seeded by a multi-session analysis run in July 2025 using Abacus AI, which produced the foundational framework synthesis documents now forming the research layer of this repository. The application layer translates those frameworks into interactive modules built on Next.js 15, TypeScript, and a full Radix UI component library.

---

## Framework Baseline

PEW is organized around five foundational frameworks, each with a corresponding interactive module in the application:

| Framework | Route | Description |
|---|---|---|
| **PALS** — Promptcraft-Aware Linguistic Stack | `/pals-builder` | Multi-layer structural prompt composition across structural, meaning, cognitive, functional, and trust dimensions |
| **Context Engineering 2.0** | `/cxep-simulator` | Interactive simulation of the Context-to-Execution Pipeline (CxEP) for verifiable, antifragile AI execution |
| **AI Prompts Systemic Analysis** | `/systemic` | Critical systems lens for failure cascade analysis, cognitive friction mapping, and governance trade-offs |
| **Role Prompting Research** | `/role` | Persona engineering, role anchoring, synergistic role stacking, and multi-agent orchestration |
| **LensGPT Deep Prompting** | `/lens` | Reflexive and epistemic deep inquiry, scaffolding, bias detection, and recursive refinement |

---

## Application Routes

The Next.js App Router exposes the following modules:

| Route | Purpose |
|---|---|
| `/` | Dashboard — framework navigator and research corpus overview |
| `/pals-builder` | PALS Framework interactive builder |
| `/lens` | LensGPT Deep Prompting workspace |
| `/geometric` | Geometric / polygonal prompt composition tools |
| `/cxep-simulator` | Context-to-Execution Pipeline simulator |
| `/creative` | Creative prompt generation workspace |
| `/compare` | Side-by-side framework and prompt comparison |
| `/cross` | Cross-framework integration analysis |
| `/exercises` | Guided prompt engineering exercises |
| `/integration` | Framework integration mapping and architecture tools |
| `/library` | Prompt library — browse, search, tag, and manage prompts |
| `/meta` | Meta-cognitive and recursive prompting workspace |
| `/quality` | Prompt quality evaluation and scoring |
| `/role` | Role Prompting Research workspace |
| `/systemic` | Systemic Analysis workspace |

---

## Tech Stack

**Application layer**

- [Next.js 15](https://nextjs.org) — App Router, React Server Components
- [React 18](https://react.dev) + [TypeScript 5.2](https://www.typescriptlang.org)
- [Tailwind CSS 3.3](https://tailwindcss.com) + [tailwindcss-animate](https://github.com/jamiebuilds/tailwindcss-animate)
- [Radix UI](https://www.radix-ui.com) — full headless component library (accordion, dialog, dropdown, tabs, toast, and more)
- [shadcn/ui](https://ui.shadcn.com) — component registry (`components.json`)
- [Framer Motion 10](https://www.framer.com/motion/) — animation
- [Lucide React](https://lucide.dev) — icons

**Data & state**

- [Prisma 6.7](https://www.prisma.io) — ORM + schema (`app/prisma/`)
- [NextAuth 4](https://next-auth.js.org) + [`@next-auth/prisma-adapter`](https://authjs.dev/reference/adapter/prisma) — authentication
- [TanStack Query 5](https://tanstack.com/query) — server state
- [Zustand 5](https://zustand-demo.pmnd.rs) + [Jotai 2](https://jotai.org) — client state
- [SWR 2](https://swr.vercel.app) — data fetching

**Visualization & analysis**

- [Plotly.js 2](https://plotly.com/javascript/) + [react-plotly.js](https://github.com/plotly/react-plotly.js) — scientific charts
- [Recharts 2](https://recharts.org) + [Chart.js 4](https://www.chartjs.org) — standard charts
- [Mapbox GL 1](https://docs.mapbox.com/mapbox-gl-js/guides/) — spatial visualization

**Forms & validation**

- [React Hook Form 7](https://react-hook-form.com) + [Zod 3](https://zod.dev) + [Yup 1](https://github.com/jquense/yup)

**Tooling**

- [Yarn Berry](https://yarnpkg.com) (`.yarnrc.yml`)
- [ESLint 9](https://eslint.org) + Prettier
- [tsx](https://github.com/privatenumber/tsx) for seed scripts

---

## Repository Structure

```
prompt_engineering_workbench/
│
├── .github/                          # GitHub configuration (Actions, templates)
│
├── Uploads/                          # Raw source research documents and corpus inputs
│
├── app/                              # Next.js 15 application
│   ├── app/
│   │   ├── api/                      # API routes
│   │   ├── compare/                  # Framework comparison module
│   │   ├── creative/                 # Creative prompting workspace
│   │   ├── cross/                    # Cross-framework integration
│   │   ├── cxep-simulator/           # Context-to-Execution Pipeline simulator
│   │   ├── evaluate/                 # Ablation harness and promotion tracker
│   │   ├── exercises/                # Guided exercises
│   │   ├── geometric/                # Geometric prompt composition
│   │   ├── governance/               # Governance Dashboard and Decorator Registry
│   │   ├── integration/              # Integration mapping tools
│   │   ├── lens/                     # LensGPT Deep Prompting workspace
│   │   ├── library/                  # Prompt library
│   │   ├── meta/                     # Meta-cognitive workspace
│   │   ├── pals-builder/             # PALS Framework builder
│   │   ├── quality/                  # Quality evaluation
│   │   ├── role/                     # Role Prompting workspace
│   │   ├── stacks/                   # Stack Profile selector
│   │   ├── systemic/                 # Systemic Analysis workspace
│   ├── app/                          # App Router pages and layouts
│   │   ├── api/                      # API routes
│   │   ├── compare/                  # Framework comparison module
│   │   ├── creative/                 # Creative prompting workspace
│   │   ├── cross/                    # Cross-framework integration
│   │   ├── cxep-simulator/           # Context-to-Execution Pipeline simulator
│   │   ├── exercises/                # Guided exercises
│   │   ├── geometric/                # Geometric prompt composition
│   │   ├── integration/              # Integration mapping tools
│   │   ├── lens/                     # LensGPT Deep Prompting workspace
│   │   ├── library/                  # Prompt library
│   │   ├── meta/                     # Meta-cognitive workspace
│   │   ├── pals-builder/             # PALS Framework builder
│   │   ├── quality/                  # Quality evaluation
│   │   ├── role/                     # Role Prompting workspace
│   │   ├── systemic/                 # Systemic Analysis workspace
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   └── page.tsx                  # Dashboard / root
│   ├── components/                   # Shared UI components
│   ├── hooks/                        # Custom React hooks
│   ├── lib/                          # Utilities and shared logic
│   ├── prisma/                       # Database schema and migrations
│   ├── scripts/                      # Seed and utility scripts
│   ├── .env                          # Environment variables (see setup below)
│   ├── next.config.js
│   ├── tailwind.config.ts
│   └── package.json
│
├── prompt_engineering_analysis.md    # Foundational analysis: PALS + Context Engineering 2.0
├── additional_frameworks_analysis.md # Analysis: Systemic, Role Prompting, LensGPT
├── advanced_frameworks_synthesis.md  # Synthesis and roadmap across extended corpus
│
├── CONTRIBUTING.md                   # Contribution rules and Workbench Analysis Agent spec
└── README.md
```

---

## Getting Started

### Prerequisites

- Node.js 20+
- Yarn Berry (`corepack enable`)
- A supported database (PostgreSQL recommended for Prisma)
- API keys as required by `.env`

### Installation

```bash
# Clone the repository
git clone https://github.com/projectedanx/prompt_engineering_workbench.git
cd prompt_engineering_workbench/app

# Install dependencies
yarn install

# Configure environment
cp .env .env.local
# Edit .env.local with your database URL and API keys

# Run database migrations
yarn prisma migrate dev

# Seed the database (optional)
yarn prisma db seed

# Start the development server
yarn dev
```

The application will be available at `http://localhost:3000`.

### Environment Variables

| Variable | Required | Description |
|---|---|---|
| `DATABASE_URL` | ✅ | Prisma database connection string |
| `NEXTAUTH_SECRET` | ✅ | NextAuth signing secret |
| `NEXTAUTH_URL` | ✅ | Base URL for NextAuth callbacks |
| Additional keys | See `.env` | Provider-specific API keys |

---

## Research Layer

The research layer is the epistemic foundation of the workbench. It consists of structured analysis documents produced by running a multi-document synthesis process against the prompt engineering corpus.

### Core Analysis Documents

**[`prompt_engineering_analysis.md`](./prompt_engineering_analysis.md)**
Foundational analysis establishing the PALS and Context Engineering 2.0 frameworks. Defines the initial workbench architecture and transitions from ad-hoc prompting to systematic, auditable prompt design.

**[`additional_frameworks_analysis.md`](./additional_frameworks_analysis.md)**
Extended analysis covering Systemic Analysis, Role Prompting Research, and LensGPT Deep Prompting. Introduces systemic critique, persona orchestration, and epistemic inquiry layers.

**[`advanced_frameworks_synthesis.md`](./advanced_frameworks_synthesis.md)**
Broader synthesis across the full corpus with integration mapping, proposed architecture upgrades, phased implementation roadmap, and success metrics.

### Workbench Analysis Agent

New research documents can be analyzed and integrated using the **Workbench Analysis Agent** prompt defined in [`CONTRIBUTING.md`](./CONTRIBUTING.md). This agent:

1. Extracts frameworks and methodologies from source documents
2. Normalizes them into a consistent framework catalog
3. Maps them against the existing PEW baseline
4. Proposes architectural, service, and evaluation implications
5. Designs a phased implementation roadmap

The `Uploads/` directory holds raw source documents for batch analysis runs.

---

## Contributing

All contributions follow the systematic research-to-implementation workflow defined in [`CONTRIBUTING.md`](./CONTRIBUTING.md).

**In brief:**

1. Add source research to `Uploads/`
2. Run the Workbench Analysis Agent against it (see CONTRIBUTING.md for the full prompt)
3. Produce a normalized framework analysis document
4. Map findings to the PEW baseline and propose integration
5. Submit a pull request with analysis artifact + any application changes

Contributions that are modular, traceable, systematic, and honest about uncertainty are strongly preferred. See CONTRIBUTING.md for the full standard.

---

## Project Status

| Layer | Status |
|---|---|
| Research corpus | ✅ Established — 3 core documents, 50+ source studies |
| Framework baseline | ✅ Defined — PALS, CxEP, Systemic, Role, LensGPT |
| Governance Core | ✅ Defined — PDL, SCOS, Dichotomic Scaffolds |
| Contribution rules | ✅ Formalized |
| Application — routing | ✅ 14 module routes implemented |
| Application — data layer | ✅ Prisma schema (including Governance Core) + NextAuth in place |
| Application — UI | 🔄 In active development |
| Deployment | 🔜 Not yet documented |

---

## Design Principles

- **Modular** — each framework module is separable and independently usable
- **Traceable** — architectural claims link back to explicit research artifacts
- **Systematic** — all contributions use a consistent extraction and integration protocol
- **Research-first, implementation-aware** — theory is always translated into buildable structure
- **Honest about uncertainty** — speculative or experimental areas are labeled as such

---

## Who This Is For

- Prompt engineers and context engineers building systematic workflows
- AI systems designers working with multi-agent architectures
- Researchers studying emergent LLM behaviors and evaluation
- AI safety and governance researchers
- Anyone moving from ad-hoc prompting to auditable, framework-driven interaction design

---

## License

[MIT](LICENSE)

---

> **Note on the Google AI Studio apps:** A parallel collection of 40+ experimental AI Studio applications spans creative writing tools (Fanon Forge), semantic analysis engines (CogniLexicon, Unified Word Explorer), context pipelines (NexusFlow, CxEP Explorer), architectural governance platforms (Architector AI, Architecture AI), and multi-agent workspaces (Sovereign Cognitive OS, Epistemic Nexus). These apps represent the broader research surface from which workbench frameworks are derived. Selected apps may be documented and linked here as the project matures.
