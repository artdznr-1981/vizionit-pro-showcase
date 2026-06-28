# VizionIt Pro

**AI-Powered Catalog Production Pipeline for Lighting Manufacturers**

*One product photo to a complete marketing content library in under 4 minutes.*

**[▶ Watch the demo on LinkedIn](https://www.linkedin.com/posts/susanmcleannangle_lightingdesign-productmarketing-interiordesign-ugcPost-7440468882349309952-WGd4)**

> This repository is a project showcase. The application source code and the proprietary AI pipeline are private. The sections below describe the product, the architecture, and the engineering challenges it solves.

---

## The Problem

Lighting manufacturers spend $15K-$30K and weeks of production time per product line on catalog photography, 3D room rendering, and marketing content.

## The Solution

VizionIt Pro replaces that entire workflow with a single product photo and AI. Upload one fixture image and the pipeline handles product analysis, creative naming with trademark verification, photorealistic room staging, SEO-optimized marketing copy, PDF catalog brochures, and social media posts.

## Highlights

- **Intelligent product analysis** that extracts 8 specifications from a single image and auto-generates a trademark-checked product name.
- **12 photorealistic room scenes** across interior and exterior environments, generated in one click.
- **Architecturally correct placement engine** — a proprietary system of 156 rules (13 fixture types x 12 rooms) that places fixtures where they actually belong, rather than the generic "hero product in foreground" default.
- **Professional exports** including SEO-optimized copy, 300ppi print-ready image bundles, branded PDF spec catalogs, and a Social Media Studio for Instagram, Facebook, and LinkedIn.

## Architecture

A separated image + copy pipeline ensures consistent marketing descriptions regardless of model text variability, and a custom multi-step process solves precise fixture placement across all 156 fixture-room combinations.

## Engineering Challenges Solved

- **Precise fixture placement** against generative models' bias toward foreground composition.
- **Consistent marketing copy** via a decoupled image and copy architecture.
- **A 13 x 12 placement matrix** where each fixture behaves differently per room (a mini-pendant is a row of three over an island, but a flanking pair beside a bed).

## Tech Stack

React, TypeScript, Vite, and Tailwind CSS on the frontend, with a proprietary AI pipeline on the backend.

---

(c) 2026 Susan McLean Nangle. All Rights Reserved. This repository is published for portfolio and demonstration purposes only.
