<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/hero-dark.png">
    <img src=".github/assets/hero.png" alt="design.me.at landing page" width="880">
  </picture>
</p>

<h1 align="center">design.me.at</h1>

<p align="center"><strong>Animated React components, installed as source.</strong></p>

<p align="center">
  <img src="https://img.shields.io/badge/status-live-171717?style=flat-square" alt="Status: live">
  <img src="https://img.shields.io/badge/license-source--available-404040?style=flat-square" alt="License: source-available">
  <img src="https://img.shields.io/badge/part%20of-me.at-737373?style=flat-square" alt="Part of me.at">
</p>

<p align="center">
  <a href="https://design.me.at">Website</a> ·
  <a href="#features">Features</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#screenshots">Screenshots</a> ·
  <a href="#built-with">Built with</a>
</p>

Component libraries arrive as a package you depend on, and design tokens drift because nothing pins them. I built design.me.at to fix both: an installable catalog of animated components and page sections you add to your project as source with the shadcn CLI, and a token studio where you author the color, type, space and motion behind your own brand once. Publish an immutable version and consume it as CSS custom properties, a Tailwind theme, DTCG JSON or TypeScript.

> **Status:** the site is live, and the catalog, registry and studio are built. Production storage and pricing are not finalized.

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/overview-dark.svg">
    <img src=".github/assets/overview.svg" alt="design.me.at at a glance: components as source, install with shadcn, tokens with a version, four outputs pinned" width="880">
  </picture>
</p>

## Why design.me.at

| The usual component library | design.me.at |
| --- | --- |
| A package you depend on | Source copied into your project with the shadcn CLI |
| Colors baked into the component | Themed from your own CSS custom properties |
| Tokens that change under you | Immutable versions, pinned by version and content hash |
| A runtime theme client | No runtime client: CSS, Tailwind, DTCG JSON or TypeScript at build time |

## Features

- **Component registry**: 22 components and page sections (text effects, light, marquees, backdrops and landing-page blocks), each with a live demo, props, theme properties and source.
- **Install with the shadcn CLI**: every component is a registry item, so `npx shadcn add` copies the source into your project with no dependencies beyond React.
- **Themed from your tokens**: components read your CSS custom properties, and you can try a palette on a live example.
- **Token studio**: edit a DTCG token document, inspect resolved values and alias paths, and check declared contrast pairs.
- **Four output formats**: CSS, Tailwind, DTCG JSON and TypeScript, emitted deterministically.
- **Immutable, versioned publishing**: published versions are content-addressed, with semver derived from the change (removed or retyped tokens imply a major).
- **Pin at build time**: consumers pin an exact version and content hash, and there is no runtime token client.
- **Respects reduced motion**: animated components hold still under `prefers-reduced-motion`.

## How it works

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/assets/flow-dark.svg">
    <img src=".github/assets/flow.svg" alt="How design.me.at works: browse, install, author, publish, consume" width="880">
  </picture>
</p>

Browse a component with its live demo, props and source, then install it with `npx shadcn add`. For your own brand, edit a DTCG token document in the studio and publish it as an immutable version, with semver derived from what changed. Consumers pin that version and content hash at build time, and the components read the resulting CSS custom properties.

## Screenshots

<table>
  <tr>
    <td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/components-dark.png"><img src=".github/assets/components.png" alt="Components"></picture><br><sub>Components: the catalog, themed from your own CSS custom properties.</sub></td>
    <td width="50%"><picture><source media="(prefers-color-scheme: dark)" srcset=".github/assets/pricing-dark.png"><img src=".github/assets/pricing.png" alt="Pricing"></picture><br><sub>Pricing: where the commercial side stands today.</sub></td>
  </tr>
</table>

## Built with

<p>
  <img src="https://img.shields.io/badge/Next.js-16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js 16">
  <img src="https://img.shields.io/badge/React-19-171717?style=flat-square&logo=react&logoColor=white" alt="React 19">
  <img src="https://img.shields.io/badge/TypeScript-5-262626?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-4-404040?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS 4">
  <img src="https://img.shields.io/badge/Drizzle-Postgres-525252?style=flat-square&logo=drizzle&logoColor=white" alt="Drizzle ORM and Postgres">
  <img src="https://img.shields.io/badge/shadcn-registry-737373?style=flat-square&logo=shadcnui&logoColor=white" alt="shadcn registry">
</p>

- Next.js 16 (App Router), React 19, TypeScript
- Tailwind CSS 4
- shadcn registry format
- DTCG design tokens
- oRPC + TanStack Query
- Drizzle ORM + Postgres
- Better Auth (shared `*.me.at` account)

## Part of the me.at family

design.me.at is one of my [`*.me.at`](https://me.at) apps. They share one design system, one account, and one app shell. Development happens in a private monorepo; this repository is the project's public-facing home.

## License

Source-available. See [LICENSE](LICENSE).
