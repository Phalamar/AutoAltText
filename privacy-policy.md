# Privacy Policy — Auto Alt-Text for Confluence

**Last updated:** 2026-05-17

This Privacy Policy explains how the Atlassian Marketplace app "Auto Alt-Text for Confluence" (the "App") processes personal data.

> **Pre-publication checklist (remove this block before publishing):**
> - Insert real postal address in section 1 (currently bracketed placeholder).
> - Have a lawyer with experience in German GDPR / DDG enforcement review the full document.
> - Verify the "Last updated" date reflects the lawyer-reviewed final version.

---

## 1. Controller and contact

The App is published by:

> Rouven Hohlstein-Thiel
> [INSERT POSTAL ADDRESS — required under GDPR Art. 13 and German DDG §5]
> [Postal code, City], Germany
> Email: Phalamar@googlemail.com

Rouven Hohlstein-Thiel is an individual based in Germany and offers this App in a private capacity.

**Note on roles:** When your organization installs the App in your Confluence Cloud instance, your organization is the **data controller** for the content the App processes (your Confluence pages and the personal data they may contain). The App's publisher acts as a **data processor** on your behalf, processing data only as necessary to provide the App's functionality.

## 2. What the App processes

The App is a Forge app running on Atlassian's infrastructure. It processes data only when a Confluence page is updated by a user in a space where the App has been configured.

For each page-update event, the App may process:

- **Page content** in Atlas Document Format — to find images that lack alt text.
- **Image attachments** (binary content) — to send to the AI provider chosen by your space administrator.
- **Generated alt text** — returned by the AI provider and written back to the page.
- **Page IDs and space IDs** — used to scope settings and prevent the App from re-triggering on its own page updates.
- **AI provider API keys** — supplied by your space administrator and stored in Atlassian-managed Forge storage.

The App does **not** process or store:

- User identities, names, email addresses, or other directly identifying user data from Confluence
- Usage analytics or telemetry sent to the publisher
- Any data on servers operated by the publisher (the publisher does not operate any servers)

## 3. Where data goes

The App transmits data to the following recipients:

| Recipient | Data | When |
|---|---|---|
| Atlassian (Forge runtime and app storage) | Settings, suppression markers, and — transiently during execution — page content and image bytes | Always — Atlassian hosts the App |
| AI provider configured by your space administrator (one of: Google Gemini, OpenAI, Anthropic, xAI/Grok) | Image bytes and a short language-specific prompt, authenticated with your stored API key | Each time the App processes a candidate image |

Data is **not** sent to the publisher (Rouven Hohlstein-Thiel). The publisher does not operate any servers and does not have access to your Confluence content, your API keys, or generated alt text.

## 4. Sub-processors

| Sub-processor | Role | Data shared |
|---|---|---|
| Atlassian | Cloud platform and runtime hosting the App | All processed data passes through Atlassian's infrastructure under your existing Atlassian Cloud agreement |
| AI provider chosen by the customer (per Confluence space) | Generates alt text from images | Image bytes and a short prompt |

You choose the AI provider on a per-space basis and may switch providers at any time. Each AI provider's data handling is governed by their own terms:

- Google (Gemini): https://ai.google.dev/terms
- OpenAI: https://openai.com/policies/
- Anthropic: https://www.anthropic.com/legal
- xAI (Grok): https://x.ai/legal

Review the chosen provider's terms before configuring the App for spaces containing sensitive content.

## 5. Retention

- **Settings (provider choice, output language, API key) and self-update suppression markers** are retained in Forge app storage for as long as the App is installed in your Confluence instance.
- **Image bytes, prompts, and generated alt text** are not retained by the App after a page-update event finishes processing. The Forge function holds them only during execution.
- **Retention by the chosen AI provider** is governed by that provider's terms.

When the App is uninstalled, Atlassian Forge purges the App's storage in accordance with Atlassian's data deletion policies.

## 6. Legal basis (GDPR)

The App processes personal data on the following legal bases:

- **Art. 6(1)(b) GDPR — performance of a contract**: when your organization installs the App and a space administrator configures it, processing is necessary to provide the agreed functionality.
- **Art. 6(1)(f) GDPR — legitimate interests**: improving accessibility of Confluence content for users who rely on assistive technology is a legitimate interest of both data controllers and data subjects.

If image content includes special categories of personal data (Art. 9 GDPR — e.g., images that reveal racial or ethnic origin, religious beliefs, or health data), the data controller (your organization) is responsible for ensuring an appropriate legal basis under Art. 9(2) GDPR before configuring the App for those spaces.

## 7. Data subject rights

If you are an individual whose personal data is processed via the App, your rights under GDPR — access (Art. 15), rectification (Art. 16), erasure (Art. 17), restriction (Art. 18), portability (Art. 20), objection (Art. 21), and complaint (Art. 77) — are exercisable against the **data controller**, that is, the organization operating the Confluence instance that has installed the App.

The App publisher acts only as a processor and will support the controller in fulfilling such requests where required by Art. 28 GDPR.

For privacy questions directed at the App publisher, contact: **Phalamar@googlemail.com**

## 8. Security

- API keys are stored in Atlassian-managed Forge app storage, which is encrypted at rest by Atlassian. After a key is saved, the App's configuration UI never returns it in plaintext — only a presence indicator is shown.
- All network traffic uses HTTPS.
- The App's external network access is restricted to the four AI provider hosts declared in its `manifest.yml`. No other outbound connections are possible from within the Forge runtime.
- The App publisher does not operate any infrastructure and has no direct access to processed data.

## 9. International transfers

Depending on the AI provider you select, image data may be transferred outside the European Economic Area (EEA), in particular to the United States. The legal basis for such transfers — for example, EU Standard Contractual Clauses or the EU-US Data Privacy Framework adequacy decision — is governed by the agreement between your organization and the AI provider.

If your organization requires data to remain within the EEA, choose an AI provider that offers EEA-resident inference, or refrain from configuring the App for affected spaces.

## 10. Children

The App is not directed at children under 16 and does not knowingly process children's data. The App is intended for use in business contexts (Confluence Cloud workspaces).

## 11. Changes to this policy

The publisher may update this Privacy Policy. Material changes will be reflected in the "Last updated" date at the top of the document. The current version is always available at the URL referenced in the App's Marketplace listing. Continued use of the App after an update constitutes acceptance of the revised policy.

## 12. Complaints

For complaints about the publisher's processing of your personal data, you may contact a competent supervisory authority. In Germany, this is the Federal Commissioner for Data Protection and Freedom of Information (Bundesbeauftragter für den Datenschutz und die Informationsfreiheit, BfDI), or your state's data protection authority.
