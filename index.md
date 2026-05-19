---
layout: default
title: Auto Alt-Text for Confluence
---

# Auto Alt-Text for Confluence

AI-generated alt text and visible captions for images in Confluence Cloud. Bring your own AI provider key (Google Gemini, OpenAI GPT-4o, Anthropic Claude, or xAI Grok); your images and key never touch the publisher's servers.

## Install

[Atlassian Marketplace listing](https://marketplace.atlassian.com/) <!-- TODO: replace with the actual marketplace listing URL once published -->

## Documentation

- [Privacy policy](privacy-policy.html) (English)
- [Datenschutzerklärung](privacy-policy-de.html) (Deutsch)
- [Terms and Conditions / Allgemeine Geschäftsbedingungen](terms.html)
- [Data Processing Agreement / Auftragsverarbeitungsvertrag (AVV)](dpa.html)
- [Imprint / Impressum](imprint.html)

## Support

[Open an issue on GitHub](https://github.com/Phalamar/AutoAltText/issues) — bug reports, feature requests, and questions.

## What it does

Auto Alt-Text watches Confluence Cloud pages for image uploads. When you publish a page with an image whose alt text is empty or just a filename, the app sends the image to the AI provider you configured (your key, your space's settings) and writes the description back. Optionally, the same description is written as a visible caption — searchable in Confluence and read aloud by Confluence's narration feature.

Three modes, configurable per Confluence space:

- **Off** — the app is dormant in this space.
- **Alt text only** (default) — generates hidden alt text for screen readers.
- **Alt text and visible caption** — also writes the description as a caption below each image.

Existing manually-written alt text and captions are never overwritten — only empty fields get filled.
