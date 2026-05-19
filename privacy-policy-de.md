# Datenschutzerklärung — Auto Alt-Text für Confluence

**Stand:** 17.05.2026

Diese Datenschutzerklärung erläutert, wie die Atlassian-Marketplace-App "Auto Alt-Text für Confluence" (die "App") personenbezogene Daten verarbeitet.

> **Checkliste vor Veröffentlichung (vor Veröffentlichung diesen Block entfernen):**
> - Postanschrift in Abschnitt 1 einsetzen (aktuell nur Platzhalter).
> - Volltext durch einen Anwalt mit Erfahrung in DSGVO / DDG-Durchsetzung in Deutschland prüfen lassen.
> - Stand-Datum auf das Datum der finalen, rechtlich geprüften Version aktualisieren.

---

## 1. Verantwortlicher und Kontakt

Die App wird angeboten von:

> Rouven Hohlstein-Thiel
> [POSTANSCHRIFT EINSETZEN — gemäß Art. 13 DSGVO und § 5 DDG erforderlich]
> [PLZ, Ort], Deutschland
> E-Mail: Phalamar@googlemail.com

Rouven Hohlstein-Thiel ist eine in Deutschland ansässige Privatperson und bietet diese App in privater Eigenschaft an.

**Hinweis zu den Rollen:** Wenn Ihre Organisation die App in Ihrer Confluence-Cloud-Instanz installiert, ist Ihre Organisation **Verantwortlicher** im Sinne der DSGVO für die Inhalte, die die App verarbeitet (Ihre Confluence-Seiten und die darin möglicherweise enthaltenen personenbezogenen Daten). Der App-Anbieter handelt in Ihrem Auftrag als **Auftragsverarbeiter** und verarbeitet Daten ausschließlich, soweit dies zur Bereitstellung der App-Funktionalität erforderlich ist.

Wenn Sie uns direkt per E-Mail kontaktieren (z. B. für Supportanfragen), verarbeiten wir Ihre E-Mail-Adresse und die übermittelten Nachrichteninhalte als Verantwortlicher ausschließlich zur Bearbeitung Ihrer Anfrage (Rechtsgrundlage: Art. 6 Abs. 1 lit. b bzw. f DSGVO). Diese Daten werden gelöscht, sobald Ihre Anfrage abschließend geklärt ist.

## 2. Welche Daten die App verarbeitet

Die App ist eine Forge-App, die auf der Infrastruktur von Atlassian läuft. Sie verarbeitet Daten ausschließlich dann, wenn ein Nutzer eine Confluence-Seite in einem Bereich aktualisiert, in dem die App konfiguriert ist.

Bei jedem Seiten-Update-Ereignis kann die App folgende Daten verarbeiten:

- **Seiteninhalt** im Atlas Document Format — um Bilder ohne Alt-Text zu identifizieren.
- **Bildanhänge** (Binärinhalte) — zur Übermittlung an den vom Bereichs-Administrator gewählten KI-Anbieter.
- **Generierter Alt-Text** — vom KI-Anbieter zurückgegeben und in die Seite zurückgeschrieben.
- **Seiten- und Bereichs-IDs** — zum Geltungsbereich der Einstellungen und zur Verhinderung selbst ausgelöster Re-Trigger.
- **API-Schlüssel der KI-Anbieter** — vom Bereichs-Administrator hinterlegt und in der von Atlassian verwalteten Forge-App-Storage gespeichert.

Die App verarbeitet oder speichert **nicht**:

- Identitäten, Namen, E-Mail-Adressen oder andere direkt identifizierende Nutzerdaten aus Confluence
- Nutzungsanalysen oder Telemetrie an den Anbieter
- Daten auf Servern des Anbieters (der Anbieter betreibt keine Server)

## 3. Wohin Daten übermittelt werden

Die App übermittelt Daten an folgende Empfänger:

| Empfänger | Daten | Wann |
|---|---|---|
| Atlassian (Forge-Runtime und App-Storage) | Einstellungen, Suppression-Marker und — vorübergehend während der Ausführung — Seiteninhalte und Bildbytes | Immer — Atlassian hostet die App |
| Vom Bereichs-Administrator konfigurierter KI-Anbieter (einer von: Google Gemini, OpenAI, Anthropic, xAI/Grok) | Bildbytes und ein kurzer sprachspezifischer Prompt, authentifiziert mit Ihrem hinterlegten API-Schlüssel | Bei jeder Verarbeitung eines Kandidatenbildes |

Daten werden **nicht** an den Anbieter (Rouven Hohlstein-Thiel) übermittelt. Der Anbieter betreibt keine eigene Infrastruktur und hat keinen Zugriff auf Ihre Confluence-Inhalte, Ihre API-Schlüssel oder generierten Alt-Text.

## 4. Unterauftragsverarbeiter

| Unterauftragsverarbeiter | Rolle | Übermittelte Daten |
|---|---|---|
| Atlassian | Cloud-Plattform und Runtime, die die App hostet | Sämtliche verarbeiteten Daten durchlaufen die Infrastruktur von Atlassian — geregelt durch Ihren bestehenden Atlassian-Cloud-Vertrag |
| Vom Kunden gewählter KI-Anbieter (pro Confluence-Bereich) | Generiert Alt-Texte aus Bildern | Bildbytes und kurzer Prompt |

Sie wählen den KI-Anbieter pro Bereich und können ihn jederzeit wechseln. Der Datenumgang jedes KI-Anbieters wird durch dessen eigene Geschäftsbedingungen geregelt:

- Google (Gemini): https://ai.google.dev/terms
- OpenAI: https://openai.com/policies/
- Anthropic: https://www.anthropic.com/legal
- xAI (Grok): https://x.ai/legal

Bitte prüfen Sie die Bedingungen des gewählten Anbieters, bevor Sie die App für Bereiche mit sensiblen Inhalten konfigurieren.

## 5. Speicherdauer

- **Einstellungen (Anbieterwahl, Ausgabesprache, API-Schlüssel) und Self-Update-Suppression-Marker** werden in der Forge-App-Storage so lange gespeichert, wie die App in Ihrer Confluence-Instanz installiert ist.
- **Bildbytes, Prompts und generierter Alt-Text** werden von der App nach Abschluss eines Seiten-Update-Ereignisses nicht aufbewahrt. Die Forge-Funktion hält sie ausschließlich während der Ausführung im Arbeitsspeicher.
- **Speicherdauer beim gewählten KI-Anbieter** wird durch dessen Bedingungen geregelt.

Bei Deinstallation der App löscht Atlassian Forge die App-Storage gemäß den Datenlöschungsrichtlinien von Atlassian.

## 6. Rechtsgrundlage (DSGVO)

Aus Sicht des Verantwortlichen (Ihre Organisation) basiert die Verarbeitung der Daten durch die App in der Regel auf folgenden Rechtsgrundlagen:

- **Art. 6 Abs. 1 lit. b DSGVO — Vertragserfüllung**: Sobald Ihre Organisation die App installiert und ein Bereichs-Administrator sie konfiguriert, ist die Verarbeitung zur Bereitstellung der vereinbarten Funktionalität erforderlich.
- **Art. 6 Abs. 1 lit. f DSGVO — berechtigtes Interesse**: Die Verbesserung der Barrierefreiheit von Confluence-Inhalten für Nutzer, die auf assistive Technologien angewiesen sind, stellt ein berechtigtes Interesse sowohl der Verantwortlichen als auch der betroffenen Personen dar.

Falls Bildinhalte besondere Kategorien personenbezogener Daten umfassen (Art. 9 DSGVO — z. B. Bilder, die rassische oder ethnische Herkunft, religiöse Überzeugungen oder Gesundheitsdaten offenbaren), ist der Verantwortliche (Ihre Organisation) dafür zuständig, eine geeignete Rechtsgrundlage nach Art. 9 Abs. 2 DSGVO sicherzustellen, bevor die App für diese Bereiche konfiguriert wird.

## 7. Betroffenenrechte

Wenn Sie eine Person sind, deren personenbezogene Daten über die App verarbeitet werden, stehen Ihnen unter der DSGVO folgende Rechte zu: Auskunft (Art. 15), Berichtigung (Art. 16), Löschung (Art. 17), Einschränkung (Art. 18), Datenübertragbarkeit (Art. 20), Widerspruch (Art. 21) und Beschwerde (Art. 77). Diese Rechte sind gegenüber dem **Verantwortlichen** geltend zu machen — also gegenüber der Organisation, die die Confluence-Instanz betreibt, in der die App installiert ist.

Der App-Anbieter handelt ausschließlich als Auftragsverarbeiter und unterstützt den Verantwortlichen bei der Erfüllung solcher Anfragen, soweit nach Art. 28 DSGVO erforderlich.

Anfragen zum Datenschutz an den App-Anbieter: **Phalamar@googlemail.com**

## 8. Sicherheit

- API-Schlüssel werden in der von Atlassian verwalteten Forge-App-Storage gespeichert, die von Atlassian verschlüsselt im Ruhezustand abgelegt wird. Nach dem Speichern eines Schlüssels gibt die Konfigurationsoberfläche der App ihn nicht mehr im Klartext zurück — angezeigt wird lediglich, dass ein Schlüssel hinterlegt ist.
- Sämtlicher Netzwerkverkehr erfolgt über HTTPS.
- Der externe Netzwerkzugriff der App ist auf die vier in der `manifest.yml` deklarierten KI-Anbieter-Hosts beschränkt. Andere ausgehende Verbindungen sind aus der Forge-Runtime nicht möglich.
- Der App-Anbieter betreibt keine eigene Infrastruktur und hat keinen direkten Zugriff auf verarbeitete Daten.

## 9. Internationale Datenübermittlungen

Je nach gewähltem KI-Anbieter können Bilddaten in Länder außerhalb des Europäischen Wirtschaftsraums (EWR) übermittelt werden, insbesondere in die USA. Die Rechtsgrundlage solcher Übermittlungen — etwa EU-Standardvertragsklauseln oder der Angemessenheitsbeschluss EU-US Data Privacy Framework — wird durch die Vereinbarung zwischen Ihrer Organisation und dem KI-Anbieter geregelt.

Wenn Ihre Organisation verlangt, dass Daten innerhalb des EWR verbleiben, wählen Sie einen KI-Anbieter, der EWR-residente Inferenz anbietet, oder konfigurieren Sie die App nicht für betroffene Bereiche.

## 10. Kinder

Die App richtet sich nicht an Kinder unter 16 Jahren und verarbeitet wissentlich keine Daten von Kindern. Die App ist für die Nutzung in geschäftlichen Kontexten (Confluence-Cloud-Arbeitsbereiche) gedacht.

## 11. Änderungen dieser Erklärung

Der Anbieter kann diese Datenschutzerklärung aktualisieren. Wesentliche Änderungen werden im "Stand"-Datum am Anfang des Dokuments kenntlich gemacht. Die jeweils aktuelle Fassung ist unter der im Marketplace-Listing der App verlinkten URL abrufbar. Die fortgesetzte Nutzung der App nach einer Aktualisierung gilt als Annahme der überarbeiteten Erklärung.

## 12. Beschwerden

Sie haben das Recht, sich bei einer zuständigen Aufsichtsbehörde zu beschweren. In Deutschland ist für private App-Anbieter die Landesdatenschutzbehörde Ihres Wohnsitzbundeslandes zuständig; für den Anbieter dieser App ist dies das Unabhängige Datenschutzzentrum Saarland (UDZ).
