# Inventory Management Dashboard — App Documentation

> Brief project documentation for the **Nextjs-Inventory-Management-System-Dashboard** repository.  
> Last updated: 2026-07-24

## Overview

This repository is intended to host an **inventory management dashboard** web application. The active Next.js application lives in the `inventory-management/` subdirectory.

| Item | Detail |
|------|--------|
| **Purpose** | Inventory management dashboard (planned) |
| **Current stage** | Initial scaffold — default Next.js starter UI |
| **App location** | `inventory-management/` |

## Tech Stack

| Layer | Technology |
|-------|------------|
| Framework | Next.js **16.2.11** (App Router) |
| Language | TypeScript |
| UI | React **19.2.4** + Tailwind CSS **4** |
| Fonts | Geist Sans & Geist Mono (`next/font`) |
| Linting | ESLint 9 + `eslint-config-next` |
| Package manager | npm |

## Repository Structure

```
Nextjs-Inventory-Management-System-Dashboard/
├── AppDocumentation.md          # This file — repo-level documentation
└── inventory-management/        # Next.js application
    ├── app/
    │   ├── layout.tsx           # Root layout, fonts, metadata
    │   ├── page.tsx             # Home page (starter content)
    │   └── globals.css          # Global styles + Tailwind theme
    ├── public/                  # Static assets (Next.js starter SVGs)
    ├── package.json
    ├── next.config.ts
    ├── tsconfig.json            # Path alias: @/* → ./*
    ├── PROJECT.md               # Detailed living project document
    └── README.md                # Default create-next-app README
```

## Current Implementation Status

**Implemented:** Only the default Next.js starter page.

- The home route displays the standard “To get started, edit the page.tsx file” message.
- App metadata still uses the default `"Create Next App"` title and description.
- No API routes, database, authentication, domain components, or automated tests exist yet.

**Not yet implemented:**

- Dashboard metrics and operational summaries
- Product and stock-level management
- Inventory adjustments and movement history
- Low-stock alerts and replenishment workflows
- Search, filtering, and reporting
- User roles and access control

## Getting Started

All commands should be run from the `inventory-management/` directory:

```bash
cd inventory-management
npm install
npm run dev      # Dev server → http://localhost:3000
npm run lint     # Run ESLint
npm run build    # Production build
npm run start    # Run production server
```

## Key Application Files

| File | Role |
|------|------|
| `inventory-management/app/page.tsx` | Main entry UI (starter template) |
| `inventory-management/app/layout.tsx` | HTML shell, fonts, and page metadata |
| `inventory-management/app/globals.css` | CSS variables, dark mode, Tailwind `@theme` |
| `inventory-management/next.config.ts` | Next.js configuration |
| `inventory-management/PROJECT.md` | Detailed living project document with scope and open decisions |

## Open Decisions

The following items are not yet defined and should be resolved before feature development begins:

- Core user workflows and product requirements
- Persistence layer (database) and hosting environment
- Data models for products, inventory, suppliers, locations, and transactions
- Authentication, authorization, and audit-log requirements
- Testing strategy, CI/CD, and deployment process

## Summary

This repository contains a **fresh Next.js 16 + React 19 + Tailwind 4 scaffold** named for an inventory dashboard. The foundation is in place inside `inventory-management/`; the next step is to define requirements and replace the starter page with real dashboard functionality.

For ongoing, detailed project tracking, see `inventory-management/PROJECT.md`.
