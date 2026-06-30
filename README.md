# PAYKX Rail — Payment Corridor Risk Intelligence

  **The pre-execution verification and safety layer for high-friction and agentic payments.**

  ![Status](https://img.shields.io/badge/status-demo%20%2F%20shadow%20mode-f59e0b)
  ![Stage](https://img.shields.io/badge/stage-pre--pilot-0ea5e9)
  ![Stack](https://img.shields.io/badge/stack-TypeScript%20%C2%B7%20React%20%C2%B7%20Express-1e293b)

  🔗 **Live demo:** [https://api.paykx.co.uk](https://api.paykx.co.uk) · **Docs:** [https://api.paykx.co.uk/docs](https://api.paykx.co.uk/docs)

  PAYKX Rail provides deterministic, explainable risk verification for high-friction
  payment corridors (e.g. UK–Nigeria, US–UK). Each verification combines behavioral,
  network, and historical data signals into a single **GO / DEGRADED / NO-GO** decision
  with a confidence score and a volatility measure — *before* any capital moves.

  This helps reduce failed transactions, trapped liquidity, and operational risk —
  whether the payment is initiated by a human or an autonomous AI agent.

  > ⚠️ **Note:** The current deployment runs in **demo / shadow mode**. All data is
  > simulated for evaluation purposes only. The platform never touches or moves real funds.

  > ℹ️ This is the **public overview** of PAYKX Rail. The application source code is
  > private and proprietary. To request access or a walkthrough, see [Contact](#contact).

  ---

  ## Live Demo

  Try the current version of PAYKX here:

  **[→ Live Demo](https://api.paykx.co.uk)**

  > The system is currently running in **demo / shadow mode**. All data is simulated.

  ---

  ## Current Status

  - **Stage** — Pre-pilot / Demo mode
  - **Focus** — High-friction corridors (e.g. UK–Nigeria)
  - **Testing** — Validated against 750,000+ synthetic transactions in the FCA Digital Sandbox
  - **Deployment** — Running in shadow / demo mode (no real funds processed)

  ---

  ## Screenshots

  ### Dashboard
  ![PAYKX dashboard](screenshots/dashboard.jpg)

  ### Live Demo Interface
  ![PAYKX live demo](screenshots/demo.jpg)

  ### Verification Result (GO / DEGRADED / NO-GO)
  ![PAYKX verification result](screenshots/result.jpg)

  ---

  ## What It Does

  - **Deterministic GO / DEGRADED / NO-GO decisions** with a confidence score and volatility measure
  - **Explainable scoring** — multiple risk signals across behavioral, network, and historical
    dimensions are weighted and combined into a single auditable result
  - **Corridor-aware** — only explicitly supported corridors return a full decision;
    unsupported corridors are reported as DEGRADED rather than guessed
  - **Idempotent & secure API design** — safe retries via idempotency keys; fails closed on auth
  - **Per-corridor cooldowns** to rate-limit repeated live verification calls
  - **Built for human and agentic flows** — designed for both traditional operators and autonomous AI agents
  - **Interactive dashboard, API tester, and access-request workflow** in the browser

  ---

  ## High-Level Architecture

  A full-stack **TypeScript** application:

  - **Frontend** — React 18 + Vite, lightweight client-side routing, server-state caching,
    type-safe forms with schema validation, an accessible component system (Radix + Tailwind CSS),
    motion, and charts. Dark / light theming.
  - **Backend** — Express 5 (TypeScript, ESM). A REST API for verification, health, and
    access requests, plus an admin workflow for reviewing requests and issuing keys.
  - **Database** — PostgreSQL via a type-safe ORM, storing verifications, access requests,
    and corridor cooldowns.
  - **Shared contracts** — route paths and validation schemas are shared across the client
    and server so the two never drift.

  > The implementation details, scoring logic, and data pipelines are proprietary and
  > kept in a private repository.

  ---

  ## Tech Stack

  | Layer       | Technologies |
  |-------------|--------------|
  | Frontend    | React 18, TypeScript, Vite, TanStack Query, React Hook Form, Zod, shadcn/ui (Radix + Tailwind CSS), Framer Motion, Recharts |
  | Backend     | Node.js, Express 5, TypeScript (ESM) |
  | Database    | PostgreSQL, Drizzle ORM |
  | Tooling     | Vite, esbuild, drizzle-kit |
  | Hosting     | Replit Deployments (autoscale), custom domain |

  ---

  ## Roadmap

  - [ ] Production deployment with live corridor integrations
  - [ ] Expanded corridor coverage beyond UK–Nigeria
  - [ ] First-class agentic payment support
  - [ ] Self-hosted / on-prem option
  - [ ] Public API documentation & SDKs

  ---

  ## Contact

  - **Website** — [https://paykx.co.uk](https://paykx.co.uk)
  - **Live demo** — [https://api.paykx.co.uk](https://api.paykx.co.uk)
  - **LinkedIn** — Taseen Rayed

  > Early stage • Actively building • Open to conversations with potential partners and co-founders.

  ---

  © PAYKX Rail. All rights reserved. This overview is provided for informational purposes;
  the source code is proprietary and not licensed for reuse.

  Built in London. Designed for global agentic finance.
  