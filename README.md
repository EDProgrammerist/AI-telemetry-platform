# TLMTRY — AI Telemetry Platform

A polished, production-style landing page for **TLMTRY**, a unified telemetry and observability platform built for engineering teams monitoring distributed AI systems. Built with pure HTML, Tailwind CSS (CDN)  and Iconify icons.

---

## Overview

TLMTRY is a conceptual SaaS landing page that showcases a platform designed to help engineering teams monitor AI agents, track infrastructure health, analyze system telemetry, detect anomalies, and respond to operational events from a single dashboard.

---

## Features

### Page Sections

- **Header / Navigation** — Fixed frosted-glass navbar with logo, centered nav links, and CTA buttons (Book Demo, Start Free Trial). Mobile-responsive with a hamburger menu icon.
- **Hero Section** — Full-width hero with headline, subtext, dual CTAs, social proof micro-labels, and an interactive dashboard preview mockup.
- **Dashboard Preview** — A detailed visual mock of the TLMTRY interface including a sidebar, stat cards (Global Telemetry Throughput, Active Threat Signals), an agent status table, and an activity feed.
- **Platform Capabilities** — 4-card grid covering: Unified Telemetry, Anomaly Detection, Infrastructure Health, and Operational Logs.
- **System Performance** — Key metrics row (4,210+ Active AI Agents, 124.8 TB/s throughput, 99.99% uptime, 32 regions) alongside a live throughput chart simulation and cluster node status panels.
- **Testimonials** — 3-card testimonial grid featuring quotes from fictional engineers at Vercel, Stripe, and Databricks.
- **Pricing** — 3-tier pricing layout: Developer (Free), Production ($149/mo), and Enterprise (Custom).
- **CTA + Footer** — Dark full-width CTA banner and a minimal 5-column footer with social links and system status indicator.

### Design Details

- Editorial background grid system with subtle vertical/horizontal lines and intersection dots
- Emerald green (`#10B981`) as the primary accent color with glow effects
- Inter (sans-serif) for UI text, JetBrains Mono for data labels and system codes
- Consistent `tracking-tighter` / `tracking-tight` typography for a refined, modern feel
- Micro-animations: pulsing status indicators, hover lift transitions, and SVG chart lines
- `backdrop-blur` frosted glass navbar
- Horizontal scroll support on the dashboard mockup for smaller screens

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Page structure |
| Tailwind CSS (CDN) | Utility-first styling |
| Iconify (Solar icon set) | UI icons |
| Google Fonts | Inter + JetBrains Mono |
| Inline SVG | Chart visualizations |

> No Node.js, no bundler, no build step. Everything runs directly in the browser.

---
## Project Structure

```
AI_Telemetry_Platform.html   ← Single-file application
README.md
```

All styles, scripts, and markup are co-located in the HTML file. External dependencies are loaded via CDN:

```html
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>

<!-- Iconify (Solar icon set) -->
<script src="https://code.iconify.design/iconify-icon/1.0.7/iconify-icon.min.js"></script>

<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
```

---

## Responsive Behavior

| Breakpoint | Behavior |
|---|---|
| Mobile (`< 768px`) | Single-column layout, stacked nav, hamburger menu, horizontal scroll on dashboard mockup |
| Tablet (`md: 768px+`) | 2-column grids, full nav visible, expanded button groups |
| Laptop / Desktop (`lg: 1024px+`) | Full 4-column capabilities grid, 12-column layout for section headers |
| Wide (`max-w-[1360px]`) | Content capped and centered for ultra-wide displays |

---

## Pricing Tiers

| Plan | Price | Key Limits |
|---|---|---|
| Developer | Free | 5 AI Agents, 50GB throughput, 7-day log retention |
| Production | $149/mo | Unlimited agents, 5TB throughput, 30-day retention, anomaly detection |
| Enterprise | Custom | Unlimited throughput, dedicated nodes, custom retention, 24/7 SLA |

---

## Customization

Since the project uses Tailwind via CDN, you can customize it directly in the HTML:

- **Colors** — Swap `emerald-500` classes to any Tailwind color (e.g., `violet-500`, `sky-500`) to retheme the entire page.
- **Typography** — Update the Google Fonts import and `font-family` style on `<body>` to change the typeface.
- **Content** — All copy (headlines, feature descriptions, pricing, testimonials) is plain HTML text — just edit in place.
- **Dashboard Mockup** — The chart is a raw inline `<svg>` — update the `d` path values to change the chart shape.

---

## Potential Improvements

- [ ] Connect a hamburger mobile menu with JS toggle
- [ ] Add scroll-triggered animations (e.g., Intersection Observer)
- [ ] Replace static chart SVG with a real Chart.js or Recharts implementation
- [ ] Extract into a React/Next.js component-based project
- [ ] Add dark mode toggle
- [ ] Implement real navigation anchor links for each section

---

## License

This project is for portfolio / learning purposes. All company names and testimonials referenced (Vercel, Stripe, Databricks) are fictional and used for design demonstration only.

---

