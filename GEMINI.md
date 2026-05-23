# FATEC SP Healthcheck - Design Handoff

## Project Overview
This project is a design handoff and interactive prototype for the **FATEC SP Healthcheck**, a playfully designed, student-focused dashboard. It monitors the availability of the main FATEC SP website to infer if there's a power outage on the campus. The UI design combines the technical authority of FATEC with an approachable, irreverent personality inspired by the PostHog design system.

The application is currently implemented as a set of standalone HTML files using React (via unpkg CDNs) and Babel standalone, with all CSS styles and interactive logic contained inline.

## Building and Running
Currently, this project exists as a static, "no-build" prototype.

- To run the application locally, simply open `index.html` or `fatec-healthcheck.html` directly in any modern web browser.
- No package managers (like `npm` or `yarn`) or build steps are required to view the current state.

*TODO: Document the new build and run commands once the prototype is ported to a modern production framework (e.g., Next.js, Vite, React) as requested by the design handoff instructions.*

## Development Conventions & Handoff Guidelines
This repository acts as a strict visual and behavioral contract for turning the provided prototype into production code. When porting or expanding this UI, adhere to the following rules:

- **Implementation Target:** Build the production UI accurately from the exported design without loose reinterpretation. Keep generated product UI free of Open Design chrome or preview labels.
- **Design Fidelity:**
  - Extract reusable design tokens (background, surface, foreground, muted text, border, accent, radius, shadow, spacing, type scale) before writing components.
  - Preserve the typography scale (IBM Plex Sans & Source Code Pro), spacing rhythm, color tokens, and interactive states (hover, focus, disabled, etc.).
  - The `brand-spec.md` acts as a reference for visual direction, color tokens (OKLch), and typography.
- **Responsive Contract:** Validate the implementation across the 2025–2026 viewport matrix (ranging from 360×800 to 1920×1080) defined in `DESIGN-HANDOFF.md` and `DESIGN-MANIFEST.json`. Use fluid typography and container queries where appropriate.
- **Architecture & Structure:**
  - Use `DESIGN-MANIFEST.json` as the machine-readable map for screens, app modules, interactions, and viewports.
  - Implement each distinct user-facing screen or surface as its own file or route.
  - `index.html` serves as a launcher/overview when multiple screens exist; do not treat it as a combined final UI if migrating to a routed application.
