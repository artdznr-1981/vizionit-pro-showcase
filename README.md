# VizionIt Pro

**AI-Powered Catalog Production Pipeline for Lighting Manufacturers**

*One product photo to a complete, client-ready marketing content library in under 4 minutes.*

**[Watch the demo on LinkedIn](https://www.linkedin.com/posts/susanmcleannangle_lightingdesign-productmarketing-interiordesign-ugcPost-7440468882349309952-WGd4)**

_This repository is a project showcase. The application source code and the proprietary AI pipeline are private. The sections below describe the product, its capabilities, and the engineering challenges it solves. (Formerly developed under the name SnapIt Pro.)_

## The Problem

Lighting manufacturers spend $15K-$30K and weeks of production time per product line on catalog photography, 3D room rendering, and marketing content.

## The Solution

VizionIt Pro replaces that entire workflow with a single product photo and AI. Upload one fixture image and the pipeline handles product analysis, creative naming with trademark verification, photorealistic room staging, SEO-optimized marketing copy, PDF catalog brochures, and social media posts, all automatically.

## What It Does

- **Upload** a single product image (chandelier, pendant, sconce, and more).
- **Analyze**: AI extracts 8 product specifications (name, design style, dimensions, bulb info, hanging height, ETL listing, finish color, shade) into editable fields.
- **Name and verify**: AI generates a creative product name and runs an automatic trademark check, flagging results with an AI Verified or AI Revised badge.
- **Configure**: adjust lighting intensity, color temperature (warm 2700K to cool 5000K), and architectural style.
- **Stage**: generate photorealistic room scenes across interior and exterior environments, each with tailored marketing copy.
- **Export**: download a branded multi-page PDF catalog, a 300ppi print-ready image bundle, or ready-to-post social media content.

## Highlights

- **Intelligent product analysis** that auto-extracts 8 specifications from a single image with editable fields and a trademark-checked product name.
- **Photorealistic room staging** across residential interior and exterior scenes, generated individually or in one batch run.
- **Architecturally correct placement engine**: a proprietary system of 156 rules (13 fixture types x 12 rooms) that places fixtures where they actually belong, rather than the generic hero-product-in-foreground default.
- **Full creative control** over lighting intensity, color temperature, and architectural style (Transitional, Modern, Contemporary, Industrial, Traditional, Sustainable Organic, Modern Farmhouse, Modern Retro, and more).
- **Professional exports**: SEO-optimized copy, 300ppi print-ready image bundles, branded multi-page PDF spec catalogs, and a Social Media Studio for Instagram, Facebook, and LinkedIn.

## Architecture

A separated image and copy pipeline ensures consistent marketing descriptions regardless of model text variability, and a custom multi-step process solves precise fixture placement across all 156 fixture-room combinations.

## Engineering Challenges Solved

- **Precise fixture placement**: the hardest problem was getting generative image models to respect real-world spatial rules instead of defaulting to hero-product composition. This required a custom multi-step architecture built specifically for this use case.
- **Consistent marketing copy** via a decoupled image and copy architecture.
- **A 13 x 12 placement matrix** where each fixture behaves differently per room (a mini-pendant is a row of three over a kitchen island, but a flanking pair beside a bed; a bath fixture mounts above the vanity mirror).
- **Robust generation at scale** with retry handling and rate-limit safeguards for reliable batch output.

## Tech Stack

- **Frontend:** React, TypeScript, Vite, TailwindCSS, Framer Motion
- **Backend:** Python, FastAPI
- **AI:** Generative AI APIs for image analysis and scene generation
- **Export:** Client-side PDF catalog and image-bundle generation

---

(c) 2026 Susan McLean Nangle. All Rights Reserved. This repository is published for portfolio and demonstration purposes only.
