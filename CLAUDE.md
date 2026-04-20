# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Landing page for "Café Arquitetura do Lucro" — an in-person business event in São Paulo (May 13, 2026). The site is a single-page static site in Brazilian Portuguese targeting entrepreneurs who revenue 100k+/month.

## Architecture

- **Single-file site**: Everything lives in `index.html` — HTML structure, all CSS (in a `<style>` block), and minimal JS (FAQ accordion toggle at the bottom).
- **No build tools or dependencies**: Plain HTML/CSS/JS. No bundler, no package manager, no framework. Open `index.html` directly in a browser to preview.
- **Assets**: `assets/` contains images (e.g., `fotobecaelucas.webp`).
- **Fonts**: Google Fonts (Montserrat) loaded via CDN.
- **Ticket sales**: CTA buttons link to an external Sympla event page.

## Design System

CSS custom properties defined in `:root`:
- Primary accent (neon green): `--neon: #00E5A0`
- Dark background palette: `--bg` through `--bg4`
- Typography: Montserrat, weights 300–900

The page follows a dark theme with neon green accents throughout. Sections alternate between `--bg` and `--bg2` backgrounds separated by `.divider-neon` gradient lines.

## Page Sections (top to bottom)

Topbar → Hero → Pain points → Solution intro → 6-block methodology → Hosts (Lucas & Rebeca) → Testimonials → "Is this for you?" → Pricing/offer card → Final CTA → Sticky mobile CTA → Footer

## Notes

- The language is Brazilian Portuguese — all copy, labels, and CTA text must stay in pt-BR.
