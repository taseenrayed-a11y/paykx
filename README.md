# PAYKX

  **Pre-execution verification and safety layer for high-friction and agentic payments.**

  PAYKX provides a deterministic decision layer that evaluates payments **before** money moves. It returns a clear `GO`, `DEGRADED`, or `NO-GO` signal with explainable risk factors.

  This helps reduce failed transactions, trapped liquidity, and operational risk — whether the payment is initiated by a human or an autonomous AI agent.

  ## The Problem

  Most innovation in payments today focuses on **moving money faster**. However, as payments become more automated and AI agents start initiating transactions, the real challenge shifts to **deciding whether a payment should happen at all**.

  Current systems are largely reactive — they detect problems *after* a payment has been sent. On complex cross-border corridors, this often leads to failed transactions, manual investigations, compliance issues, and poor customer experiences.

  ## Our Solution

  PAYKX introduces a **pre-transaction decision layer** that sits before money moves. It assesses risk and intent upfront and provides a clear signal on whether a payment is safe to execute, should be delayed, or requires further review.

  Rather than replacing existing payment rails or PSPs, PAYKX acts as an independent verification layer that adds clarity and control before execution.

  ## Current Status

  - **Stage**: Pre-pilot (Demo / Shadow Mode)
  - **Focus**: High-friction corridors (e.g. UK–Nigeria) and emerging agentic payment flows
  - **Testing**: Validated using 750,000+ synthetic transactions in the FCA Digital Sandbox
  - **Live Demo**: [https://api.paykx.co.uk](https://api.paykx.co.uk)

  > **Note**: The system is currently running in demo/shadow mode. No real transactions are processed.

  ## Key Features

  - Real-time pre-transaction decisioning
  - Explainable scoring with multiple risk signals
  - Corridor health and compliance evaluation
  - Support for idempotent and secure API requests
  - Designed to work alongside existing payment infrastructure

  ## Tech Stack

  - **Frontend**: React 18 + Vite + TypeScript + shadcn/ui
  - **Backend**: Express + TypeScript + Drizzle ORM
  - **Database**: PostgreSQL
  - **Other**: Zod, TanStack Query, Recharts

  ## Live Demo

  Try the current version here:

  **[→ Live Demo](https://api.paykx.co.uk)**

  ## Screenshots

  ### Dashboard
  ![Dashboard](screenshots/dashboard.jpg)

  ### Demo Verification Page
  ![Demo Page](screenshots/demo.jpg)

  ### Verification Result
  ![Result](screenshots/result.jpg)

  ## Roadmap

  - Production deployment and real corridor integrations
  - Enhanced support for agentic and autonomous payment flows
  - Self-hosted deployment option
  - Expanded risk models and corridor coverage

  ## Contact

  - **Website**: [https://paykx.co.uk](https://paykx.co.uk)
  - **LinkedIn**: [Taseen Rayed](https://www.linkedin.com/in/taseen-r-5299b92a7)

  ---

  **Status**: Early stage • Actively building • Open to conversations with potential partners and co-founders.
  