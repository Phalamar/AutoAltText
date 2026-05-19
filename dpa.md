# Data Processing Agreement / Auftragsverarbeitungsvertrag (AVV)

**Last updated / Stand:** 2026-05-19


## How to use this AVV — conclusion in electronic form / Nutzungsweise — Abschluss in elektronischer Form

**No physical signature required.** Art. 28 (9) GDPR expressly provides that a data processing agreement under Art. 28 GDPR "shall be in writing, including in electronic form." German law accepts text form (Textform, § 126b BGB) — a permanent declaration on a durable medium identifying the person making it (e.g. an email, a confirmation in a customer's account, or click-to-accept) — as sufficient. The parties expressly agree that this AVV is concluded in electronic form and that no qualified electronic signature (§ 126a BGB) and no handwritten signature (§ 126 BGB) is required for its validity or for any notice, amendment, or termination contemplated by it. Wherever this AVV refers to "text form" or "in writing", the requirement of § 126b BGB is to be applied.

This document is provided as a standing offer by the Publisher. It becomes binding between the parties when the Customer (controller) (a) installs the App "Auto Alt-Text for Confluence" via the Atlassian Marketplace, (b) configures the App via the space-settings UI by storing an AI provider API key, and (c) confirms acceptance of this AVV in text form — for example by an email to the contact address below identifying the Customer's Atlassian Cloud organization, by completing an electronic acceptance form provided by the Publisher, or by any other declaration on a durable medium clearly identifying the Customer. The Publisher confirms receipt of acceptance in text form; that confirmation, together with the acceptance, constitutes the documentary record required by Art. 28 (9) GDPR.

If a customer's internal procurement process nonetheless requires a counter-signed paper or qualified-electronic-signature version, contact the Publisher at the email address in the Parties section below.

---

**Keine physische Unterschrift erforderlich.** Art. 28 Abs. 9 DSGVO sieht ausdrücklich vor, dass ein Auftragsverarbeitungsvertrag nach Art. 28 DSGVO „schriftlich abzufassen [ist], was auch in einem elektronischen Format erfolgen kann". Das deutsche Recht erkennt die Textform (§ 126b BGB) — eine auf einem dauerhaften Datenträger abgegebene, dauerhaft lesbare Erklärung, die die Person des Erklärenden nennt (z. B. eine E-Mail, eine Bestätigung im Kundenkonto oder ein „Click-to-Accept") — als ausreichend an. Die Parteien vereinbaren ausdrücklich, dass dieser AVV in elektronischer Form geschlossen wird und für seine Wirksamkeit sowie für die in ihm vorgesehenen Mitteilungen, Änderungen oder Kündigungen weder eine qualifizierte elektronische Signatur (§ 126a BGB) noch eine eigenhändige Unterschrift (§ 126 BGB) erforderlich ist. Soweit in diesem AVV auf „Textform" oder „schriftlich" Bezug genommen wird, gilt das Erfordernis des § 126b BGB.

Dieses Dokument wird vom Anbieter als ständiges Angebot zur Verfügung gestellt. Es wird zwischen den Parteien verbindlich, wenn der Kunde (Verantwortlicher) (a) die App „Auto Alt-Text für Confluence" über den Atlassian Marketplace installiert, (b) die App über die Bereichseinstellungen durch Hinterlegung eines KI-Anbieter-API-Schlüssels konfiguriert und (c) die Annahme dieses AVV in Textform bestätigt — z. B. durch E-Mail an die unten genannte Kontaktadresse unter Angabe der Atlassian-Cloud-Organisation des Kunden, durch Ausfüllen eines vom Anbieter bereitgestellten elektronischen Annahmeformulars oder durch eine andere Erklärung auf einem dauerhaften Datenträger, die den Kunden eindeutig identifiziert. Der Anbieter bestätigt den Eingang der Annahme in Textform; diese Bestätigung bildet zusammen mit der Annahme die nach Art. 28 Abs. 9 DSGVO erforderliche Dokumentation.

Sollte ein interner Beschaffungsprozess eines Kunden gleichwohl eine papierhaft gegengezeichnete Fassung oder eine qualifiziert elektronisch signierte Fassung erfordern, ist der Anbieter unter der im Abschnitt „Parteien" genannten E-Mail-Adresse zu kontaktieren.

---

## English version

### Parties

**Controller** ("Customer"): The legal entity that installs the App "Auto Alt-Text for Confluence" in its Atlassian Confluence Cloud instance and configures it for one or more Confluence spaces.

**Processor** ("Publisher"):

> Rouven Hohlstein-Thiel
> [INSERT POSTAL ADDRESS]
> [Postal code, City], Germany
> Email: Phalamar@googlemail.com

### Preamble

The Customer has procured the Atlassian Marketplace app "Auto Alt-Text for Confluence" (the "App") from the Publisher. The App processes personal data on behalf of the Customer within the meaning of Art. 4 No. 8 and Art. 28 GDPR. This Data Processing Agreement ("AVV") specifies the parties' rights and obligations regarding such processing. It supplements the agreement governing use of the App (the Atlassian Standard EULA and the Publisher's Terms and Conditions) and the Atlassian Marketplace Terms.

### 1. Subject matter, nature, purpose, and duration of processing

#### 1.1 Subject matter and nature

The Publisher processes personal data on behalf of the Customer exclusively to provide the functionality of the App as described in §3 of the Publisher's Terms and Conditions: detecting images on Confluence pages whose alt text is empty or contains only a filename, forwarding those images and a short prompt to the AI provider configured by the Customer's space administrator, and writing the AI provider's response back to the page as alt text (and, where enabled, as a visible caption).

The nature of processing comprises: reading page content via the Atlassian Confluence REST API upon page creation or update; reading image attachment binaries; transmitting image bytes and prompts to the customer-selected AI provider over HTTPS; writing alt text and (optionally) captions back to pages; reading and writing the App's configuration in Forge app storage.

#### 1.2 Purpose

The purpose of the processing is solely to support the Customer in providing alt text for images in Confluence pages, in order to improve accessibility of those pages for users of assistive technology.

#### 1.3 Duration

This AVV applies for as long as the App is installed in the Customer's Atlassian Cloud organization and at least one Confluence space is configured with an AI provider and a corresponding API key. It ends automatically upon uninstallation or upon removal of the configuration in all spaces.

### 2. Specification of the processing

#### 2.1 Categories of data subjects

Persons whose personal data may appear in image content uploaded to Confluence pages in spaces where the App is configured. This may include, depending on Customer content: employees, contractors, customers, business partners, attendees of events documented in Confluence, and any other natural person depicted in or identifiable from images.

#### 2.2 Categories of personal data

- Image content that depicts or identifies natural persons (e.g. photographs, screenshots of personal data, scans of documents).
- Free-text prompts derived solely from a fixed, language-specific template and not containing personal data from Confluence beyond the image itself.
- Confluence page IDs and space IDs (technical identifiers used for routing and suppression of self-triggered events).
- Generated alt text and (optionally) captions that may contain descriptions of natural persons inferred by the AI provider from the image.
- The Customer's AI provider API key (configuration data; not the personal data of a data subject in the GDPR sense, but treated as confidential).

#### 2.3 Special categories of personal data (Art. 9 GDPR)

If Customer image content includes special categories of personal data (e.g. images that reveal racial or ethnic origin, religious or philosophical beliefs, trade union membership, health data, sexual orientation, biometric data identifying a person), the Customer is responsible for ensuring an appropriate legal basis under Art. 9 (2) GDPR before configuring the App for the affected spaces. The Publisher does not solicit or knowingly facilitate processing of special categories.

### 3. Rights and obligations of the Controller

#### 3.1 Responsibility

The Customer remains the controller within the meaning of Art. 4 No. 7 GDPR for the personal data processed via the App. The Customer is solely responsible for assessing the lawfulness of the processing, for selecting an appropriate AI provider, and for informing data subjects.

#### 3.2 Instructions

The Customer instructs the Publisher to process personal data as documented in this AVV, the Privacy Policy, and the App's documentation. Additional or amending instructions shall be issued in text form (email is sufficient) to the contact address above. The Publisher shall confirm receipt of such instructions in text form. Where an instruction would, in the Publisher's reasonable assessment, infringe data protection law, the Publisher shall inform the Customer in text form without undue delay and may suspend execution of the instruction until clarified.

#### 3.3 Contact persons

The Customer's designated contact for processing-related matters is the person identified in the Customer's Atlassian Cloud organization as the administrator of the relevant Confluence space. The Publisher's contact is the email address in the Parties section above.

### 4. Obligations of the Processor

#### 4.1 Processing on instructions only

The Publisher processes personal data only on the documented instructions of the Customer, including with regard to transfers to third countries, unless required to do so by Union or Member State law to which the Publisher is subject. The Publisher shall inform the Customer of any such legal requirement before processing, unless that law prohibits such information on important grounds of public interest.

#### 4.2 Confidentiality

The Publisher ensures that any natural persons authorized to process personal data on behalf of the Publisher are bound to confidentiality (by contract or by statute). Currently, the Publisher operates as an individual and has no employees with access to personal data; should this change, confidentiality obligations in text form will be put in place before any access is granted.

#### 4.3 Technical and organizational measures

The Publisher implements appropriate technical and organizational measures (TOMs) within its sphere of control to ensure a level of security appropriate to the risk. The TOMs are described in **Annex 1**. The Customer acknowledges that a substantial portion of the security perimeter is provided by Atlassian's Forge platform; the Publisher inherits and relies upon Atlassian's platform controls and the customer-chosen AI provider's platform controls, in addition to its own measures.

#### 4.4 Support for the Controller

Taking into account the nature of the processing and the information available to the Publisher, the Publisher shall reasonably assist the Customer in fulfilling its obligations under Articles 32–36 GDPR (security, breach notification, data protection impact assessment, prior consultation) and Articles 12–22 GDPR (data subject requests). The Customer acknowledges that the Publisher's ability to assist is limited by the architecture of the App (no data is held on infrastructure operated by the Publisher).

#### 4.5 Sub-processors

The Customer hereby grants general authorization for the engagement of sub-processors. The current sub-processors are listed in **Annex 2**. The Publisher shall inform the Customer of any intended changes (addition or replacement of sub-processors) by an update of Annex 2 at the URL referenced in the App's Marketplace listing, with at least 30 days' prior notice for material changes where reasonably possible. The Customer may object in text form within 30 days of notice. If the parties cannot resolve the objection, the Customer may terminate its use of the App without cost; charges already incurred remain payable.

The Publisher imposes the same data protection obligations on sub-processors as those set out in this AVV, in particular sufficient guarantees that processing meets the requirements of the GDPR. Where a sub-processor's data protection obligations are governed by a separate agreement between that sub-processor and the Customer (as is the case for Atlassian under the Atlassian Cloud agreement and for the AI provider under the AI provider's own terms), those agreements apply.

#### 4.6 Records of processing activities

The Publisher maintains a written (electronic) record of processing activities carried out on behalf of the Customer in accordance with Art. 30 (2) GDPR, to the extent applicable to the Publisher.

#### 4.7 Notification of breaches

The Publisher notifies the Customer in text form without undue delay, and where feasible within 72 hours of becoming aware, of any personal data breach affecting personal data processed on behalf of the Customer. The notification shall, to the extent known, include the information set out in Art. 33 (3) GDPR. The Publisher shall reasonably assist the Customer in fulfilling its notification obligations to the supervisory authority and to data subjects.

#### 4.8 Data subject requests

If a data subject contacts the Publisher directly to exercise rights under Articles 15–22 GDPR with respect to personal data processed on behalf of the Customer, the Publisher shall forward the request to the Customer without undue delay and shall not respond to the data subject directly on the merits of the request. The Publisher shall reasonably assist the Customer in handling such requests.

#### 4.9 Deletion and return

Upon termination of this AVV (uninstallation of the App or removal of configuration), the Publisher shall, at the Customer's choice, return or delete all personal data of the Customer held by the Publisher in connection with the processing, unless Union or Member State law requires storage. In practice, the Publisher does not hold any personal data on infrastructure operated by the Publisher; the only data that persists is held within Atlassian Forge app storage and is purged by Atlassian according to Atlassian's data deletion policies upon uninstallation.

#### 4.10 Audits

The Publisher provides the Customer with all information necessary to demonstrate compliance with Art. 28 GDPR. Audits and inspections may be carried out by the Customer or an auditor mandated by the Customer, subject to the following:

- audits shall be announced at least 30 days in advance in text form;
- audits shall be conducted during regular business hours, without unduly disrupting the Publisher's operations;
- audits shall, where reasonably possible, take the form of written self-assessments by the Publisher, supplemented by Atlassian and AI provider compliance documentation (e.g. SOC reports, ISO certifications, DPF participation) where available;
- on-site audits require a separate agreement in text form and reimbursement of the Publisher's reasonable costs;
- the Customer's auditor must be independent of the Publisher's competitors and bound to confidentiality.

#### 4.11 DPO

The Publisher has not appointed a Data Protection Officer; the Publisher operates as an individual below the thresholds in Art. 37 (1) GDPR and § 38 (1) BDSG. The contact for data protection matters is the Publisher's email address in the Parties section above.

### 5. International transfers

Depending on the AI provider chosen by the Customer's space administrator, personal data may be transferred to third countries outside the European Economic Area, in particular to the United States. The legal basis for such transfers (EU Standard Contractual Clauses, adequacy decision such as the EU-US Data Privacy Framework, or other safeguards under Art. 46 GDPR) is governed by the agreement between the Customer and the chosen AI provider. The Publisher does not transfer personal data to third countries on its own account.

### 6. Liability

The parties' liability under this AVV is governed by Art. 82 GDPR and by the liability provisions in the Publisher's Terms and Conditions, which apply mutatis mutandis. To the extent permitted by mandatory law, the liability cap set out in the Terms and Conditions applies cumulatively across the Terms and this AVV.

### 7. Term and termination

This AVV is effective for the duration set out in Section 1.3. Either party may terminate this AVV for cause where the other party materially breaches its obligations under this AVV or applicable data protection law and fails to remedy the breach within a reasonable period after notice in text form.

### 8. Miscellaneous

**Form.** This AVV, all notices, acceptances, instructions, breach notifications, sub-processor objections, audit announcements, amendments, supplements, and terminations contemplated by it are valid in text form (§ 126b BGB), as expressly permitted by Art. 28 (9) GDPR. Neither a qualified electronic signature (§ 126a BGB) nor a handwritten signature (§ 126 BGB) is required. A stricter form requirement can only be agreed expressly and in text form by both parties.

**Amendments.** The Publisher may update this AVV in line with changes in legal requirements or in the App's architecture; material changes will be notified to the Customer in accordance with Section 4.5 (sub-processor change procedure applied analogously). Should any provision of this AVV be invalid, the remaining provisions remain in force; the invalid provision shall be replaced with one that comes as close as possible to its economic purpose.

**Governing law and jurisdiction.** This AVV is governed by the laws of the Federal Republic of Germany; the place of jurisdiction is the seat of the Publisher to the extent permitted by law for B2B contracts.

---

## Deutsche Fassung

### Parteien

**Verantwortlicher** („Kunde"): Die juristische Person, die die App „Auto Alt-Text für Confluence" in ihrer Atlassian-Confluence-Cloud-Instanz installiert und für einen oder mehrere Confluence-Bereiche konfiguriert.

**Auftragsverarbeiter** („Anbieter"):

> Rouven Hohlstein-Thiel
> [POSTANSCHRIFT EINSETZEN]
> [PLZ, Ort], Deutschland
> E-Mail: Phalamar@googlemail.com

### Präambel

Der Kunde hat vom Anbieter die Atlassian-Marketplace-App „Auto Alt-Text für Confluence" (die „App") bezogen. Die App verarbeitet personenbezogene Daten im Auftrag des Kunden im Sinne von Art. 4 Nr. 8 und Art. 28 DSGVO. Dieser Auftragsverarbeitungsvertrag („AVV") konkretisiert die Rechte und Pflichten der Parteien hinsichtlich dieser Verarbeitung. Er ergänzt die Vereinbarung über die Nutzung der App (Atlassian Standard EULA und AGB des Anbieters) sowie die Atlassian Marketplace Terms.

### 1. Gegenstand, Art, Zweck und Dauer der Verarbeitung

#### 1.1 Gegenstand und Art

Der Anbieter verarbeitet personenbezogene Daten im Auftrag des Kunden ausschließlich zur Bereitstellung der Funktionalität der App, wie in § 3 der AGB des Anbieters beschrieben: Erkennen von Bildern auf Confluence-Seiten, deren Alt-Text leer ist oder lediglich einen Dateinamen enthält; Übermittlung dieser Bilder und eines kurzen Prompts an den vom Bereichs-Administrator des Kunden konfigurierten KI-Anbieter; Zurückschreiben der Antwort des KI-Anbieters in die Seite als Alt-Text (und, sofern aktiviert, als sichtbare Bildunterschrift).

Die Art der Verarbeitung umfasst: Lesen von Seiteninhalten über die Atlassian-Confluence-REST-API beim Erstellen oder Aktualisieren von Seiten; Lesen von Bildanhang-Binärinhalten; Übertragung von Bildbytes und Prompts an den vom Kunden gewählten KI-Anbieter über HTTPS; Schreiben von Alt-Texten und (optional) Bildunterschriften zurück in Seiten; Lesen und Schreiben der App-Konfiguration in der Forge-App-Storage.

#### 1.2 Zweck

Zweck der Verarbeitung ist ausschließlich, den Kunden bei der Bereitstellung von Alt-Texten für Bilder in Confluence-Seiten zu unterstützen, um die Barrierefreiheit dieser Seiten für Nutzer assistiver Technologien zu verbessern.

#### 1.3 Dauer

Dieser AVV gilt, solange die App in der Atlassian-Cloud-Organisation des Kunden installiert ist und mindestens ein Confluence-Bereich mit einem KI-Anbieter und einem entsprechenden API-Schlüssel konfiguriert ist. Er endet automatisch mit der Deinstallation oder mit Entfernung der Konfiguration in allen Bereichen.

### 2. Konkretisierung der Verarbeitung

#### 2.1 Kategorien betroffener Personen

Personen, deren personenbezogene Daten in Bildinhalten erscheinen können, die in Confluence-Seiten in Bereichen hochgeladen werden, in denen die App konfiguriert ist. Dies kann je nach Kundeninhalt umfassen: Mitarbeiter, freie Mitarbeiter, Kunden, Geschäftspartner, Teilnehmer von in Confluence dokumentierten Veranstaltungen sowie alle anderen natürlichen Personen, die in Bildern abgebildet oder anhand dieser identifizierbar sind.

#### 2.2 Kategorien personenbezogener Daten

- Bildinhalte, die natürliche Personen abbilden oder identifizieren (z. B. Fotografien, Screenshots mit personenbezogenen Daten, Scans von Dokumenten).
- Freitext-Prompts, die ausschließlich aus einer fest hinterlegten, sprachspezifischen Vorlage abgeleitet sind und über das Bild selbst hinaus keine personenbezogenen Daten aus Confluence enthalten.
- Confluence-Seiten- und Bereichs-IDs (technische Identifier zur Steuerung und zur Unterdrückung selbst ausgelöster Trigger).
- Generierte Alt-Texte und (optional) Bildunterschriften, die Beschreibungen natürlicher Personen enthalten können, die der KI-Anbieter aus dem Bild abgeleitet hat.
- Der API-Schlüssel des Kunden zum KI-Anbieter (Konfigurationsdatum; im DSGVO-Sinn keine personenbezogenen Daten einer betroffenen Person, gleichwohl als vertraulich behandelt).

#### 2.3 Besondere Kategorien personenbezogener Daten (Art. 9 DSGVO)

Sofern Bildinhalte des Kunden besondere Kategorien personenbezogener Daten umfassen (z. B. Bilder, die rassische oder ethnische Herkunft, religiöse oder weltanschauliche Überzeugungen, Gewerkschaftszugehörigkeit, Gesundheitsdaten, sexuelle Orientierung oder biometrische Daten zur eindeutigen Identifizierung offenbaren), ist der Kunde dafür verantwortlich, vor Konfiguration der App für die betroffenen Bereiche eine geeignete Rechtsgrundlage nach Art. 9 Abs. 2 DSGVO sicherzustellen. Der Anbieter fordert keine besonderen Kategorien an und fördert deren Verarbeitung nicht wissentlich.

### 3. Rechte und Pflichten des Verantwortlichen

#### 3.1 Verantwortung

Der Kunde bleibt Verantwortlicher im Sinne von Art. 4 Nr. 7 DSGVO für die über die App verarbeiteten personenbezogenen Daten. Der Kunde ist allein verantwortlich für die Bewertung der Zulässigkeit der Verarbeitung, für die Auswahl eines geeigneten KI-Anbieters und für die Information der betroffenen Personen.

#### 3.2 Weisungen

Der Kunde weist den Anbieter an, personenbezogene Daten gemäß diesem AVV, der Datenschutzerklärung und der App-Dokumentation zu verarbeiten. Zusätzliche oder ändernde Weisungen sind in Textform (E-Mail genügt) an die oben genannte Kontaktadresse zu richten. Der Anbieter bestätigt den Eingang solcher Weisungen in Textform. Sollte eine Weisung nach pflichtgemäßer Einschätzung des Anbieters gegen Datenschutzrecht verstoßen, teilt der Anbieter dies dem Kunden unverzüglich in Textform mit und kann die Ausführung der Weisung bis zur Klärung aussetzen.

#### 3.3 Ansprechpartner

Ansprechpartner des Kunden für verarbeitungsbezogene Angelegenheiten ist die in der Atlassian-Cloud-Organisation des Kunden als Administrator des betreffenden Confluence-Bereichs ausgewiesene Person. Ansprechpartner des Anbieters ist die im Abschnitt „Parteien" genannte E-Mail-Adresse.

### 4. Pflichten des Auftragsverarbeiters

#### 4.1 Verarbeitung nur auf Weisung

Der Anbieter verarbeitet personenbezogene Daten ausschließlich auf dokumentierte Weisung des Kunden, auch in Bezug auf Übermittlungen in Drittländer, es sei denn, er ist hierzu nach dem Recht der Union oder eines Mitgliedstaates, dem er unterliegt, verpflichtet. In einem solchen Fall teilt der Anbieter dem Kunden diese rechtlichen Anforderungen vor der Verarbeitung mit, sofern das betreffende Recht eine solche Mitteilung nicht wegen eines wichtigen öffentlichen Interesses verbietet.

#### 4.2 Vertraulichkeit

Der Anbieter stellt sicher, dass alle zur Verarbeitung personenbezogener Daten in seinem Namen befugten natürlichen Personen zur Vertraulichkeit verpflichtet sind (vertraglich oder gesetzlich). Der Anbieter stellt sicher, dass die zur Verarbeitung befugten Personen zur Vertraulichkeit verpflichtet sind. Dies gilt auch für den Fall, dass der Anbieter zur Erfüllung seiner Pflichten Erfüllungsgehilfen oder Mitarbeiter heranzieht.

#### 4.3 Technisch-organisatorische Maßnahmen

Der Anbieter trifft in seinem Verantwortungsbereich angemessene technische und organisatorische Maßnahmen (TOM), um ein dem Risiko angemessenes Schutzniveau zu gewährleisten. Die TOM sind in **Anlage 1** beschrieben. Der Kunde nimmt zur Kenntnis, dass ein wesentlicher Teil des Sicherheits-Perimeters durch die Forge-Plattform von Atlassian bereitgestellt wird; der Anbieter stützt sich neben seinen eigenen Maßnahmen auf die Plattform-Kontrollen von Atlassian sowie des vom Kunden gewählten KI-Anbieters.

#### 4.4 Unterstützung des Verantwortlichen

Unter Berücksichtigung der Art der Verarbeitung und der dem Anbieter zur Verfügung stehenden Informationen unterstützt der Anbieter den Kunden im Rahmen des Zumutbaren bei der Erfüllung seiner Pflichten nach Art. 32 bis 36 DSGVO (Sicherheit, Meldung von Verletzungen, Datenschutz-Folgenabschätzung, vorherige Konsultation) und Art. 12 bis 22 DSGVO (Anfragen betroffener Personen). Der Kunde nimmt zur Kenntnis, dass die Möglichkeiten des Anbieters zur Unterstützung durch die Architektur der App begrenzt sind (keine Daten werden auf vom Anbieter betriebener Infrastruktur vorgehalten).

#### 4.5 Unterauftragsverarbeiter

Der Kunde erteilt hiermit eine allgemeine Genehmigung zur Beauftragung von Unterauftragsverarbeitern. Die aktuellen Unterauftragsverarbeiter sind in **Anlage 2** aufgeführt. Der Anbieter informiert den Kunden über beabsichtigte Änderungen (Hinzufügung oder Ersetzung von Unterauftragsverarbeitern) durch Aktualisierung der Anlage 2 unter der im Marketplace-Listing der App verlinkten URL, bei wesentlichen Änderungen mit einer Vorlauffrist von mindestens 30 Tagen, soweit zumutbar. Der Kunde kann innerhalb von 30 Tagen nach Mitteilung in Textform widersprechen. Können die Parteien den Widerspruch nicht ausräumen, kann der Kunde die Nutzung der App ohne Kosten beenden; bereits angefallene Entgelte bleiben fällig.

Der Anbieter erlegt Unterauftragsverarbeitern dieselben Datenschutzpflichten auf, wie sie in diesem AVV festgelegt sind, insbesondere hinreichende Garantien, dass die Verarbeitung den Anforderungen der DSGVO genügt. Soweit die datenschutzrechtlichen Pflichten eines Unterauftragsverarbeiters durch eine separate Vereinbarung zwischen diesem Unterauftragsverarbeiter und dem Kunden geregelt sind (wie es für Atlassian unter dem Atlassian-Cloud-Vertrag und für den KI-Anbieter unter dessen eigenen Bedingungen der Fall ist), gelten diese Vereinbarungen.

#### 4.6 Verzeichnis der Verarbeitungstätigkeiten

Der Anbieter führt — soweit auf ihn anwendbar — ein elektronisches Verzeichnis der im Auftrag des Kunden ausgeführten Verarbeitungstätigkeiten gemäß Art. 30 Abs. 2 DSGVO.

#### 4.7 Meldung von Verletzungen

Der Anbieter meldet dem Kunden unverzüglich, nach Möglichkeit innerhalb von 72 Stunden nach Kenntniserlangung, in Textform jede Verletzung des Schutzes personenbezogener Daten, die im Auftrag des Kunden verarbeitete Daten betrifft. Die Meldung enthält, soweit bekannt, die in Art. 33 Abs. 3 DSGVO genannten Angaben. Der Anbieter unterstützt den Kunden im Rahmen des Zumutbaren bei der Erfüllung seiner Meldepflichten gegenüber der Aufsichtsbehörde und den betroffenen Personen.

#### 4.8 Anfragen betroffener Personen

Wendet sich eine betroffene Person zur Ausübung von Rechten nach Art. 15 bis 22 DSGVO bezüglich im Auftrag des Kunden verarbeiteter personenbezogener Daten direkt an den Anbieter, leitet der Anbieter die Anfrage unverzüglich an den Kunden weiter und antwortet der betroffenen Person nicht inhaltlich. Der Anbieter unterstützt den Kunden im Rahmen des Zumutbaren bei der Bearbeitung solcher Anfragen.

#### 4.9 Löschung und Rückgabe

Mit Beendigung dieses AVV (Deinstallation der App oder Entfernung der Konfiguration) gibt der Anbieter sämtliche im Zusammenhang mit der Verarbeitung beim Anbieter vorhandenen personenbezogenen Daten des Kunden nach Wahl des Kunden zurück oder löscht sie, sofern nicht das Recht der Union oder eines Mitgliedstaates eine Speicherung vorschreibt. In der Praxis hält der Anbieter keine personenbezogenen Daten auf eigener Infrastruktur; die einzigen verbleibenden Daten liegen in der Atlassian-Forge-App-Storage und werden mit Deinstallation gemäß den Datenlöschungsrichtlinien von Atlassian gelöscht.

#### 4.10 Kontrollen

Der Anbieter stellt dem Kunden alle erforderlichen Informationen zum Nachweis der Einhaltung von Art. 28 DSGVO zur Verfügung. Kontrollen und Inspektionen können durch den Kunden oder einen vom Kunden beauftragten Prüfer durchgeführt werden, vorbehaltlich der folgenden Maßgaben:

- Kontrollen sind mindestens 30 Tage im Voraus in Textform anzukündigen;
- Kontrollen finden während der üblichen Geschäftszeiten und ohne unzumutbare Störung des Geschäftsbetriebs des Anbieters statt;
- Kontrollen erfolgen, soweit zumutbar möglich, in Form schriftlicher Selbstauskünfte des Anbieters, ergänzt durch Compliance-Dokumentation von Atlassian und der KI-Anbieter (z. B. SOC-Berichte, ISO-Zertifizierungen, DPF-Teilnahme), soweit verfügbar;
- Vor-Ort-Kontrollen bedürfen einer separaten Vereinbarung in Textform und der Erstattung der angemessenen Kosten des Anbieters;
- Der Prüfer des Kunden muss unabhängig von Wettbewerbern des Anbieters und zur Vertraulichkeit verpflichtet sein.

#### 4.11 Datenschutzbeauftragter

Der Anbieter hat keinen Datenschutzbeauftragten benannt; der Anbieter handelt als Einzelperson unterhalb der Schwellen in Art. 37 Abs. 1 DSGVO und § 38 Abs. 1 BDSG. Ansprechpartner für datenschutzrechtliche Belange ist die im Abschnitt „Parteien" genannte E-Mail-Adresse des Anbieters.

### 5. Internationale Übermittlungen

Je nach dem vom Bereichs-Administrator des Kunden gewählten KI-Anbieter können personenbezogene Daten in Drittländer außerhalb des Europäischen Wirtschaftsraums übermittelt werden, insbesondere in die USA. Die Rechtsgrundlage solcher Übermittlungen (EU-Standardvertragsklauseln, Angemessenheitsbeschluss wie EU-US Data Privacy Framework oder andere Garantien nach Art. 46 DSGVO) wird durch die Vereinbarung zwischen dem Kunden und dem gewählten KI-Anbieter geregelt. Der Anbieter selbst übermittelt keine personenbezogenen Daten in Drittländer.

### 6. Haftung

Die Haftung der Parteien unter diesem AVV richtet sich nach Art. 82 DSGVO und nach den Haftungsregelungen in den AGB des Anbieters, die entsprechend gelten. Soweit gesetzlich zulässig, gilt die in den AGB festgelegte Haftungsgrenze kumulativ über die AGB und diesen AVV.

### 7. Laufzeit und Beendigung

Dieser AVV gilt für die in Abschnitt 1.3 festgelegte Dauer. Jede Partei kann diesen AVV aus wichtigem Grund kündigen, wenn die andere Partei wesentliche Pflichten aus diesem AVV oder dem anwendbaren Datenschutzrecht verletzt und die Verletzung nicht innerhalb einer angemessenen Frist nach Aufforderung in Textform abstellt.

### 8. Schlussbestimmungen

**Form.** Dieser AVV sowie sämtliche in ihm vorgesehenen Mitteilungen, Annahmen, Weisungen, Verletzungsmeldungen, Widersprüche gegen Unterauftragsverarbeiter, Kontrollankündigungen, Änderungen, Ergänzungen und Kündigungen sind in Textform (§ 126b BGB) wirksam, wie von Art. 28 Abs. 9 DSGVO ausdrücklich gestattet. Weder eine qualifizierte elektronische Signatur (§ 126a BGB) noch eine eigenhändige Unterschrift (§ 126 BGB) ist erforderlich. Ein strengeres Formerfordernis kann nur ausdrücklich und in Textform durch beide Parteien vereinbart werden.

**Änderungen.** Der Anbieter kann diesen AVV an geänderte rechtliche Anforderungen oder an Änderungen der App-Architektur anpassen; wesentliche Änderungen werden dem Kunden entsprechend Abschnitt 4.5 (analog zum Verfahren für Unterauftragsverarbeiter) mitgeteilt. Sollte eine Bestimmung dieses AVV unwirksam sein, bleiben die übrigen Bestimmungen in Kraft; die unwirksame Bestimmung wird durch eine Bestimmung ersetzt, die ihrem wirtschaftlichen Zweck möglichst nahekommt.

**Anwendbares Recht und Gerichtsstand.** Es gilt das Recht der Bundesrepublik Deutschland; Gerichtsstand ist der Sitz des Anbieters, soweit dies bei B2B-Verträgen gesetzlich zulässig ist.

---

## Annex 1 / Anlage 1 — Technical and Organizational Measures (TOMs) / Technisch-organisatorische Maßnahmen

> **Note / Hinweis:** A substantial portion of the TOMs is provided by Atlassian as platform operator of the Forge runtime where the App executes. The Customer should review Atlassian's *Cloud Security Practices*, *Cloud SOC 2 reports*, and *Cloud Subprocessor list* for the full platform picture. The measures below describe the App-specific layer.
>
> Ein wesentlicher Teil der TOM wird durch Atlassian als Plattformbetreiber der Forge-Runtime bereitgestellt, in der die App ausgeführt wird. Der Kunde sollte die *Cloud Security Practices*, *Cloud-SOC-2-Berichte* und *Cloud-Subprocessor-Liste* von Atlassian für das vollständige Bild auf Plattformebene heranziehen. Die nachstehenden Maßnahmen beschreiben die App-spezifische Ebene.

### A. Confidentiality (Art. 32 (1) (b) GDPR) / Vertraulichkeit

- **Access control / Zutrittskontrolle:** The Publisher operates no physical infrastructure. All processing infrastructure is operated by Atlassian (Forge) and by the customer-selected AI provider, each with their own physical access controls. — Der Anbieter betreibt keine physische Infrastruktur; sämtliche Verarbeitungs-Infrastruktur wird von Atlassian (Forge) und vom Kunden gewählten KI-Anbieter mit jeweils eigenen Zutrittskontrollen betrieben.
- **System access / Zugangskontrolle:** Source code repositories use multi-factor authentication. Deployment to Atlassian Forge uses authenticated CLI tokens. The Publisher has no production database or production server requiring access controls. — Quellcode-Repositories sind durch Mehr-Faktor-Authentifizierung geschützt. Deployments in Atlassian Forge erfolgen über authentifizierte CLI-Tokens. Es gibt keine produktive Datenbank oder Server-Infrastruktur des Anbieters, die einer Zugangskontrolle bedarf.
- **Data access / Zugriffskontrolle:** The App runs in Atlassian's Forge sandbox and accesses customer data only via the scopes declared in `manifest.yml`, granted explicitly during installation. The Publisher has no production access to customer data outside the Forge runtime. — Die App läuft in der Forge-Sandbox von Atlassian und greift auf Kundendaten ausschließlich über die im `manifest.yml` deklarierten und während der Installation ausdrücklich gewährten Scopes zu. Außerhalb der Forge-Runtime hat der Anbieter keinen produktiven Zugriff auf Kundendaten.
- **Pseudonymization / Pseudonymisierung:** Image content is not pseudonymized prior to forwarding to the AI provider, since the App's purpose requires the AI provider to interpret the original image. The AI provider's own data handling applies. — Bildinhalte werden vor der Weiterleitung an den KI-Anbieter nicht pseudonymisiert, da der Zweck der App erfordert, dass der KI-Anbieter das Originalbild interpretiert. Es gilt der Datenumgang des KI-Anbieters.

### B. Integrity (Art. 32 (1) (b) GDPR) / Integrität

- **Transmission control / Weitergabekontrolle:** All network connections from the App to external services use HTTPS/TLS. External egress is restricted to the four AI provider hosts declared in `manifest.yml` (`api.openai.com`, `generativelanguage.googleapis.com`, `api.anthropic.com`, `api.x.ai`); no other outbound connections are possible from within the Forge runtime. — Sämtliche Netzwerkverbindungen der App zu externen Diensten erfolgen über HTTPS/TLS. Ausgehender Verkehr ist auf die vier im `manifest.yml` deklarierten KI-Anbieter-Hosts beschränkt; andere ausgehende Verbindungen sind aus der Forge-Runtime nicht möglich.
- **Input control / Eingabekontrolle:** Page-update events that trigger the App are recorded by Atlassian Confluence as part of the page version history. The App's own write operations are visible in the page version history as edits attributed to the App. — Seiten-Update-Ereignisse, die die App auslösen, werden von Atlassian Confluence als Teil der Versionshistorie der Seite protokolliert. Schreibvorgänge der App sind in der Versionshistorie als Bearbeitungen der App sichtbar.

### C. Availability and resilience (Art. 32 (1) (b) GDPR) / Verfügbarkeit und Belastbarkeit

- The App's availability is governed by Atlassian Forge's platform availability and by the chosen AI provider's availability. The Publisher does not commit to a service level. — Die Verfügbarkeit der App wird durch die Plattform-Verfügbarkeit von Atlassian Forge sowie die Verfügbarkeit des gewählten KI-Anbieters bestimmt. Der Anbieter sichert kein Service Level zu.
- The App's configuration is held in Atlassian-managed Forge app storage, which Atlassian persists according to its own data durability practices. — Die Konfiguration der App liegt in der von Atlassian verwalteten Forge-App-Storage, die Atlassian gemäß seinen eigenen Datenhaltungspraktiken vorhält.

### D. Procedures for regular review (Art. 32 (1) (d) GDPR) / Verfahren zur regelmäßigen Überprüfung

- **Data protection management / Datenschutzmanagement:** This AVV, the Privacy Policy, and the App's TOMs are reviewed at least annually, on material changes to the App's architecture, and on material changes to the legal framework. — Dieser AVV, die Datenschutzerklärung und die TOMs der App werden mindestens einmal jährlich, bei wesentlichen Änderungen der App-Architektur und bei wesentlichen Änderungen des rechtlichen Rahmens überprüft.
- **Incident response / Vorfallmanagement:** Notification process per Section 4.7 of this AVV. The Publisher monitors security advisories for the Forge platform and the AI providers. — Meldeprozess gemäß Abschnitt 4.7 dieses AVV. Der Anbieter beobachtet Sicherheitsmeldungen für die Forge-Plattform und die KI-Anbieter.
- **Order control / Auftragskontrolle:** This AVV documents the order; sub-processor changes follow the procedure in Section 4.5. — Dieser AVV dokumentiert den Auftrag; Änderungen bei Unterauftragsverarbeitern folgen dem Verfahren in Abschnitt 4.5.

### E. Storage and segregation / Trennungskontrolle

- App configuration is segregated per Confluence space using a per-space storage key (`settings:${spaceId}`), so that configuration of one space cannot be read or written via the App's logic for another space. — Die App-Konfiguration ist je Confluence-Bereich durch einen bereichsspezifischen Storage-Key (`settings:${spaceId}`) getrennt; eine Bereichs-Konfiguration ist über die Logik der App nicht aus oder in einen anderen Bereich lesbar oder schreibbar.
- Different customers' data is segregated at the Atlassian Forge level (each installation is a separate Forge app instance scoped to one Atlassian Cloud organization). — Daten unterschiedlicher Kunden sind auf Atlassian-Forge-Ebene getrennt (jede Installation ist eine eigenständige, auf eine Atlassian-Cloud-Organisation begrenzte Forge-App-Instanz). Zusätzlich wird durch die Atlassian Forge Mandantentrennung sichergestellt, dass die App-Instanzen und Daten verschiedener Kunden (Atlassian Cloud Organisationen) strikt voneinander isoliert sind.

### F. Key handling / Schlüsselverwaltung

- The AI provider API key supplied by the Customer is stored in Atlassian-managed Forge app storage, which Atlassian encrypts at rest. After saving, the App's configuration UI never returns the key in plaintext; a presence indicator is shown instead. — Der vom Kunden hinterlegte KI-Anbieter-API-Schlüssel wird in der von Atlassian verwalteten Forge-App-Storage gespeichert, die Atlassian im Ruhezustand verschlüsselt. Nach dem Speichern gibt die Konfigurationsoberfläche den Schlüssel nicht mehr im Klartext zurück; angezeigt wird lediglich, dass ein Schlüssel hinterlegt ist.

---

## Annex 2 / Anlage 2 — Sub-processors / Unterauftragsverarbeiter

**Last reviewed / Zuletzt geprüft:** 2026-05-19

| Sub-processor / Unterauftragsverarbeiter | Role / Rolle | Location / Standort | Data / Daten |
|---|---|---|---|
| Atlassian Pty Ltd / Atlassian, Inc. | Forge platform host — runs the App and stores its configuration / Forge-Plattform-Betreiber — führt die App aus und speichert deren Konfiguration | Global (Atlassian Cloud regions per Customer setup) / Global (Atlassian-Cloud-Regionen gemäß Kundenkonfiguration) | All data processed by the App passes through Atlassian / Sämtliche von der App verarbeiteten Daten durchlaufen Atlassian |
| AI provider chosen by the Customer's space administrator / Vom Bereichs-Administrator des Kunden gewählter KI-Anbieter — currently one of / aktuell einer von: Google LLC (Gemini), OpenAI Ireland Ltd / OpenAI LLC, Anthropic PBC, xAI Corp. | Generates alt text from images / Generiert Alt-Texte aus Bildern | Per provider — typically US, with some EU residency options / Je Anbieter — überwiegend USA, teils mit EU-Residency-Optionen | Image bytes and short prompt; authenticated with the Customer's API key / Bildbytes und kurzer Prompt; authentifiziert mit dem API-Schlüssel des Kunden |

The Customer accepts that the AI provider is selected by the Customer's space administrator and is, from a data protection standpoint, a sub-processor engaged at the Customer's instruction. The Customer is responsible for entering into any required additional agreements (DPA, SCCs) directly with the AI provider; the Publisher does not act as an intermediary for such agreements.

Der Kunde akzeptiert, dass der KI-Anbieter durch seinen Bereichs-Administrator ausgewählt wird und datenschutzrechtlich ein auf Weisung des Kunden eingebundener Unterauftragsverarbeiter ist. Der Kunde ist verantwortlich für den Abschluss erforderlicher Zusatzvereinbarungen (DPA, SCC) direkt mit dem KI-Anbieter; der Anbieter tritt insoweit nicht als Vermittler auf.
