# AGENTS.md

## Project Overview

This repository contains the source code for the personal website of Roman Czerkies. It is designed as a minimalist, ultra-fast, and highly accessible web platform experiment. The primary technical objective is to implement, test, and showcase the absolute latest web technologies and specifications.

## Core Constraints

- **NO JavaScript:** Do not write, suggest, or include any JavaScript. The UI and interactions must be handled entirely through HTML and CSS.
- **NO Build Environment:** Do not use, suggest, or configure Node.js, package managers (npm, pnpm, yarn), transpilers, bundlers, Sass, or PostCSS. All code is raw, vanilla, and runs directly in the browser.

## Technology & Code Style

- **Bleeding-Edge CSS & HTML:** Prioritize the use of the latest HTML and CSS features proposed by the W3C, currently in RFC, or recently deployed in the latest versions of major browsers (based on MDN Baseline). Examples include `@layer`, `@property`, `@view-transition`, `@scope`, `color-scheme`, and `oklch()`.
- **Target Audience (Browsers):** The CSS and HTML must work flawlessly on the *latest versions* of each major web browser. Do not write legacy fallbacks or use polyfills for older browser versions.
- **Simplicity & Performance:** Keep the codebase minimal. Avoid unnecessary bloat and strictly use native browser capabilities.

## Accessibility (a11y)

- **RGAA Compliance:** The website must be rigorously accessible and adhere to RGAA (Référentiel Général d'Amélioration de l'Accessibilité) standards.
- **Semantic HTML:** Always use the most semantic HTML5 elements available. Use attributes like `aria-label` or `title` carefully and only when native semantics are insufficient.
- **User Preferences:** Respect user system preferences via CSS media queries. You must account for `prefers-color-scheme`, `prefers-reduced-motion`, `prefers-reduced-transparency`, and `prefers-contrast`.
- **Structured Data:** Maintain and update Microdata (`itemscope`, `itemtype`, `itemprop`) following schema.org standards where applicable.

## Workflow Instructions for Agents

- If asked to implement a new interaction or visual effect, you must solve it using modern CSS (e.g., CSS scroll-driven animations, state pseudo-classes, etc.) rather than scripting.
- Do not provide commands like `npm run dev` or `npm install`. There are no dependencies to install. 
- Ensure that any new properties or elements introduced align with the project's brutalist and minimalist design system.
