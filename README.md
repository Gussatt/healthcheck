# FATEC SP Healthcheck

A playfully designed, student-focused dashboard monitoring the availability of the main FATEC SP website to infer if there's a power outage on the campus.

## Overview

The FATEC SP Healthcheck UI combines the technical authority of FATEC with an approachable, irreverent personality inspired by the PostHog design system. It is currently built as an interactive prototype to serve as a design handoff.

## Tech Stack (Prototype Phase)

The application is currently implemented as a set of standalone HTML files using:
- **React** (via unpkg CDNs)
- **Babel standalone** (for in-browser JSX compilation)
- **Vanilla CSS** (inline styles)
- No build steps or package managers required.

## How to Run

Since this project exists as a static, "no-build" prototype:
1. Clone this repository.
2. Open `index.html` or `fatec-healthcheck.html` directly in any modern web browser.

## Handoff & Future Development

This repository acts as a strict visual and behavioral contract for turning the provided prototype into production code. 

**TODOs:**
- Port the prototype to a modern production framework (e.g., Next.js, Vite, React).
- Extract reusable design tokens (background, surface, foreground, etc.) based on `brand-spec.md`.
- Implement responsiveness across the 2025–2026 viewport matrix as defined in `DESIGN-HANDOFF.md` and `DESIGN-MANIFEST.json`.
