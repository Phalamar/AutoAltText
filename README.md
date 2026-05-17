# Auto Alt-Text for Confluence

This repository is the **public-facing home** for the Atlassian Marketplace app *Auto Alt-Text for Confluence*. It hosts:

- **Issues** — bug reports, feature requests, questions: [open an issue](https://github.com/Phalamar/AutoAltText/issues)
- **Privacy policy** ([English](https://phalamar.github.io/AutoAltText/privacy-policy.html) / [Deutsch](https://phalamar.github.io/AutoAltText/privacy-policy-de.html))
- **Imprint / Impressum** ([English / Deutsch in one document](https://phalamar.github.io/AutoAltText/imprint.html))

The app's source code is in a private repository.

## What the app does

Auto Alt-Text watches Confluence Cloud pages for image uploads, sends each new image to your configured AI provider (Google Gemini, OpenAI GPT-4o, Anthropic Claude, or xAI Grok), and writes the returned description back as the image's alt-text attribute. Optionally, the same description can be written as a visible image caption — searchable in Confluence and read aloud by Confluence's narration feature.

Install from the Atlassian Marketplace: [TODO: add marketplace listing URL once published]

## Three modes (per Confluence space)

- **Off** — the app is dormant in this space.
- **Alt text only** (default) — generates hidden alt text for screen readers.
- **Alt text and visible caption** — also writes the description as a caption below each image; indexed by Confluence search and audible via Confluence's narration.

Manually written alt text and captions are never overwritten — only empty fields get filled in.

## License

The contents of this repository (docs + issues) are © Rouven Hohlstein-Thiel. The app's source code is proprietary. Customer use of the app is governed by Atlassian's standard EULA (EULA-V), accepted at install time via the Atlassian Marketplace.
