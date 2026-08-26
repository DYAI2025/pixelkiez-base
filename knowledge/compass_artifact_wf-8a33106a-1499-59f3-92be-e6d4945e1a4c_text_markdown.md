# Website-Audits 2025/2026: Best Practices für Report-Design, Struktur & Inhaltskategorien

## TL;DR
- **Der beste Website-Audit-Report folgt der „Arzt-Logik": zuerst die Diagnose (1-seitige Executive Summary mit Health-Score und 3 Kernbefunden in Business-Sprache), dann priorisierte Befunde nach Impact/Effort und Severity, zuletzt der technische Anhang** — nicht umgekehrt. Was Kunden lesen und umsetzen, ist kurz (8–15 Seiten), gescored, priorisiert und mit KPIs (Umsatz, Leads, Risiko) verknüpft.
- **Businesskunden priorisieren fünf Kategorien am höchsten**: (1) Auffindbarkeit/SEO & jetzt AI-Sichtbarkeit, (2) Performance/Core Web Vitals (Speed = Umsatz), (3) Conversion/UX, (4) Mobile, und — im deutschen/EU-Markt überdurchschnittlich hoch — (5) Rechtssicherheit (DSGVO/Consent + Barrierefreiheit/BFSG seit 28. Juni 2025).
- **Die immer gleichen Kundenfragen** lauten „Warum ranke ich nicht?", „Warum konvertiert die Seite nicht?", „Ist sie schnell genug?", „Was macht die Konkurrenz besser?", „Was kostet die Behebung und was bringt sie?", „Bin ich rechtlich sicher?" und neu „Werde ich von KI gefunden?". Der Report muss jedes technische Finding in diese Sprache übersetzen.

**Hinweis zu internen Quellen:** Ich habe die verbundenen Konnektoren (Google Drive, Slack, Confluence/Jira des Workspace „dyai2026") gezielt nach vorhandenem Material zu Website-Audits, Report-Vorlagen, Checklisten oder SEO-/UX-Kriterienkatalogen durchsucht. **Es liegt dort kein relevantes eigenes Material vor** — Google Drive enthält nur unverbundene Automatisierungs-/KI-Dokumente, Confluence nur Sprint-Planungsseiten („Usable Semantic Atlas"), Slack keine Treffer. Der Report stützt sich daher vollständig auf öffentliche Quellen (2024–2026).

---

## Key Findings

1. **Struktur-Konsens (belegt):** Erfolgreiche Audit-Reports folgen fast durchgängig der Reihenfolge Executive Summary → Scoring/Kategorien → priorisierte Befunde → Roadmap → technischer Anhang. Die Executive Summary ist oft „der einzige Teil, den ein Entscheider tatsächlich liest" und sollte 1 Seite und 3 Kernbefunde umfassen.

2. **Darstellungsmuster, die sich bewährt haben (Branchenkonsens):** Ampel-/Score-System (0–100 mit Grün/Gelb/Rot-Bändern), Severity-Level (Critical/High/Medium/Low), Impact-vs-Effort-Matrix bzw. „Quick Wins vs. strategische Maßnahmen", Priorisierungsframeworks (ICE/P0-P1-P2), Owner- und Aufwandsspalten, Vorher/Nachher-Beispiele und Wettbewerbs-Benchmark.

3. **Tool-Logik unterscheidet sich klar:** Lighthouse/PSI liefern harte 0–100-Scores mit Grün/Gelb/Rot; Sitebulb übersetzt Befunde in nach Severity sortierte „Hints" mit Klartext-Erklärung (agenturfreundlichste PDF-Reports); Screaming Frog liefert rohe Daten; Ahrefs/Semrush geben Health-Scores plus Business-Kontext.

4. **Format-Wirkung (schwache Studienlage, ehrlich gekennzeichnet):** Es gibt **keine belastbare Studie, die beweist, welches Reportformat nachweislich mehr Umsetzung erzeugt**. Branchenpraxis (Freelancer/Agenturen) favorisiert Loom-Video-Audits für Akquise/Kaltakquise und strukturierte PDF/Slides-Deliverables für Umsetzung.

5. **Deutscher/EU-Markt ist Sonderfall:** DSGVO/TDDDG-Consent und das Barrierefreiheitsstärkungsgesetz (BFSG, seit 28.6.2025) machen die Kategorien Datenschutz und Accessibility hier zu Pflichtbestandteilen mit Bußgeld-/Abmahnrisiko — international sind sie oft „nice to have".

6. **INP-Wechsel muss beachtet werden:** Seit 12. März 2024 hat INP (Interaction to Next Paint) FID als Core Web Vital ersetzt. Jeder Report, der noch FID nennt, ist veraltet.

---

## Details

### 1) Report-Best-Practices und Formate

#### Aufbau und Reihenfolge
Der übergreifende Konsens der 2025/26-Quellen (Reportr, Incremys, Aslan Agency, MendMySEO, Beetle Beetle) beschreibt eine „Arzt-Diagnose"-Logik: Erst das Fazit, dann die Testergebnisse, dann die Behandlungsoptionen. Die bewährte Sektionsfolge:

1. **Executive Summary (1 Seite):** Gesamt-Health-Score (0–100), die 3 umsatzrelevantesten Befunde in Klartext, plus ein Absatz „was bedeutet das fürs Business". Beispiel für gute Übersetzung: statt „Metadata-Optimierung erforderlich" besser „Title-Tags auf den 15 Seiten neu schreiben, die bereits Impressions, aber niedrige CTR haben".
2. **Kategorie-Scores (5–6 Kategorien):** je Kategorie eine Note/ein Score plus Trendlinie (Donut-/Balkendiagramm), beantwortet „wo sind die Probleme?".
3. **Priorisierte Befunde:** Tabelle mit Issue, Impact, Effort, Priorität, Owner.
4. **Roadmap:** Quick Wins (Woche 1) → 30-Tage → Quartal.
5. **Technischer Anhang:** URL-Level-Details für Entwickler.

**Länge:** Quick-Fix-Report 5–8 Seiten; vollständiger Audit-Report typisch 8–15 Seiten. Der breite Rat lautet, den Anhang nicht zur Hauptsache zu machen. Wichtige Unterscheidung: Ein **Audit-Report** (einmalig/quartalsweise, Diagnose) ist etwas anderes als ein **Monats-Report** (laufend, Fortschritts-/ROI-Tracking) — beide sollten nicht vermischt werden.

#### Bewährte Darstellungsmuster
- **Score 0–100:** Von HubSpot Website Grader, Lighthouse, Ahrefs, Semrush genutzt. Als Benchmark und Trend zu verstehen, nicht als Ziel: „Ein Score von 72, der um 5 Punkte pro Monat steigt, ist eine bessere Situation als ein flacher Score von 80."
- **Severity-Level:** Critical/High/Medium/Low — von Sitebulb, SE Ranking, Screaming-Frog-Auswertungen genutzt.
- **Impact-vs-Effort-Matrix / Quick Wins:** Der am häufigsten empfohlene Priorisierungsansatz. Ergänzt durch ICE-Scoring (Impact, Confidence, Ease) und P0/P1/P2-Zeitfenster.
- **Owner + Aufwand:** Jede Empfehlung braucht Verantwortlichen und realistische Aufwandsschätzung.
- **Benchmark/Wettbewerbsvergleich:** „Sie überholen jetzt drei Hauptwettbewerber für 'commercial HVAC repair'" — Wettbewerbsposition ist eine der Kernfragen der Businesskunden.
- **Revenue-Impact-Schätzung:** „200 zusätzliche Besucher = ~8.000 $ potenzieller Umsatz" — mit Vorsicht, klar als Schätzung kennzeichnen.

#### Vergleich der etablierten Tools (Report-Logik)

| Tool / Anbieter | Report-Logik | Scoring | Stärke / Zielgruppe |
|---|---|---|---|
| **Google Lighthouse / PageSpeed Insights** | 4 Kategorien (Performance, Accessibility, Best Practices, SEO), Lab- + Feld-Daten (CrUX); Opportunities mit ms-Einsparung | 0–100 pro Kategorie, Grün ≥90 / Gelb 50–89 / Rot <50; Performance = gewichteter Schnitt (v12: u. a. TBT, LCP am höchsten) | Kostenlos, Performance-Diagnose; verwechselt oft Lab- vs. Feld-Daten |
| **Google Search Console** | Diagnoseportal für Googlebot: Core Web Vitals, Indexierung, Coverage; 16 Monate Historie | keine Gesamtnote | Ground-Truth-Felddaten, kein proaktives Crawling |
| **Screaming Frog** | Rohe Crawl-Daten in Tabellen, Interpretation beim Nutzer | keine Note | Desktop-Crawler, Tiefe/Flexibilität, für Techniker |
| **Sitebulb** | „Hints"-System (>300 Checks), nach Severity sortiert, Klartext + Fix; Crawl-Maps | Severity (High/Medium/Low) + Scores | Beste client-ready PDF-Reports; für Nicht-Techniker/Agenturen |
| **Ahrefs Site Audit** | Health-Score + thematische Reports, Verknüpfung mit Backlink-/Keyword-Daten | Health-Score 0–100 | Monatliches Benchmark, JS-Rendering |
| **Semrush Site Audit** | Thematische Reports in All-in-one-Suite; jetzt AI-Visibility-Tracking | Health-Score | Integration/Automatisierung, Agenturen |
| **SE Ranking** | 115+ Checks nach Severity, seit 2026 GEO/AI-Tracking | Severity-basiert | Mid-Market, sauberere UI |
| **HubSpot Website Grader** | 4 Kategorien: Performance, SEO, Mobile, Security; instant Report | Score 0–100 (Ø ~60,9 = „D-" laut HubSpot-Auswertung von >1 Mio. Submissions) | Kostenloses Lead-Gen-Tool, laienverständlich |
| **WAVE / axe (Accessibility)** | WCAG-Verstöße mit Severity | keine Note | Barrierefreiheits-Prüfung |
| **Baymard Institute** | Forschungsbasierte UX-Guidelines (700+) + Benchmark 330+ Shops | UX-Scores je Guideline | E-Commerce-UX/Checkout, von 71 % der Fortune-500-E-Commerce genutzt |
| **Nielsen Norman Group** | 10 Usability-Heuristiken, Heuristic Evaluation mit Severity 0–4 | Severity-Rating pro Verstoß | Usability-Methodik-Standard |

#### Formate: Was Kunden lesen und umsetzen
**Ehrliche Einordnung:** Es existiert **keine belastbare, unabhängige Studie**, die quantifiziert, welches Deliverable-Format (Loom-Video vs. PDF vs. Notion vs. interaktives Dashboard) nachweislich zu mehr Umsetzung oder höherem Auftragsabschluss führt. Was existiert, ist verbreitete Branchenpraxis:
- **Loom-Video-Audits (5 Min.):** Von Freelancern/SMMA für Akquise und Kaltakquise favorisiert — persönlich, zeigt Kompetenz, niedrige Hemmschwelle. Typische Struktur: mit der Website starten, 3 konkrete Empfehlungen, klarer CTA.
- **PDF-Reports:** Standard-Deliverable; 24–48 h vor dem Präsentationscall versenden.
- **Interaktive Dashboards (Looker Studio, AgencyAnalytics, Swydo):** eher für laufendes Monats-Reporting als für Erst-Audits.
- **Google-Slides/Notion:** für kundenfreundliche, brandbare Deliverables.

Wiederkehrender Rat: Der Report ist auch ein Verkaufsdokument — er soll Vertrauen aufbauen und zur Umsetzung/Beauftragung führen.

#### Typische Fehler (Branchenkonsens)
Zu technisch/Jargon ohne Business-Übersetzung; zu lang (40-Seiten-PDF ohne Summary); rohe Screaming-Frog-CSV-Exporte; jedes Finding gleich gewichtet (keine Priorisierung); kein Business-Bezug; kein Owner/Aufwand; keine Messgrößen/Baseline. Kernsatz: „Man kann ein schlechtes Audit hübsch machen, aber man kann es nicht ergebniswirksam machen."

### 2) Kategorien, die Businesskunden wichtig sind

#### Marktüblich abgedeckte Analysekategorien
Technical SEO / Crawlability / Indexierung; Performance & Core Web Vitals; Mobile-Freundlichkeit; Content & Keyword-Abdeckung; UX & Conversion; Accessibility (WCAG/EAA/BFSG); Security (HTTPS, Header); Datenschutz/DSGVO & Consent; Analytics-/Tracking-Setup; Local SEO; Internationalisierung/hreflang; interne Verlinkung; Backlinks/Authority; Brand/Trust-Signale; AI-Sichtbarkeit (AEO/GEO).

#### Was Businesskunden tatsächlich am höchsten priorisieren (mit Belegen)

| Kategorie | Kundenrelevanz | Beleg / Quelle | Business-KPI |
|---|---|---|---|
| **Website als Umsatzkanal / SEO-Sichtbarkeit** | Sehr hoch | 91 % der Marketing-Leader nennen die Website den wichtigsten Umsatzkanal (Webflow 2025 State of the Website); Website/Blog/SEO = #1 ROI-Kanal (HubSpot State of Marketing, wobei HubSpot selbst anmerkt, dass der Abstand zu Platz 2 nur wenige Punkte beträgt) | Organischer Traffic, Leads, Umsatz |
| **Performance / Core Web Vitals** | Sehr hoch | Google/Deloitte „Milliseconds Make Millions" (2020, 37 Marken/30 Mio. Sessions): +0,1 s Speed → „Retail conversions increased by 8.4% and average order value increased by 9.2%" | Conversion Rate, Bounce, Umsatz |
| **Conversion / Checkout-UX** | Sehr hoch (E-Commerce) | Baymard Institute (akt. 22.09.2025): Ø Warenkorbabbruch **70,22 %** („an average calculated based on 50 different studies"); bis zu **35,26 %** Conversion-Uplift durch besseres Checkout-Design möglich | Conversion Rate, AOV |
| **AI-Sichtbarkeit (AEO/GEO)** | Schnell steigend | **52 %** der Marketing-Leader priorisieren 2026 AI-Search-Optimierung (Webflow 2026 State of the Website, Befragung von 1.000 Marketing-/Technologie-Leadern in USA/UK/Kanada) | Zukünftige Sichtbarkeit |
| **Rechtssicherheit DE/EU (DSGVO/BFSG)** | Sehr hoch (DE/EU) | Bitkom (09.09.2025, 603 Unternehmen ab 20 Beschäftigten): „praktisch alle Unternehmen (97 Prozent) [haben] hohen Aufwand mit dem Datenschutz … 44 Prozent einen sehr hohen Aufwand"; Aktion Mensch/Google (3. Testbericht, 17.06.2025): nur ~ein Drittel der 65 meistbesuchten Shops zumindest teilweise barrierefrei | Risiko/Bußgeld, Abmahnung |
| **Local SEO (lokale Dienstleister)** | Hoch (KMU/lokal) | BrightLocal Local Marketing Industry Survey 2024: „the most valuable local SEO services are 1) Google Business Profile management (76%), 2) Content creation (53%), 3) Citation building/cleanup (43%)" | Anrufe, Besuche, lokale Leads |

#### Segment-Unterschiede
- **KMU / lokale Dienstleister:** Wollen Nachweis, dass SEO zu Anfragen führt; Fokus auf Google Business Profile, lokale Sichtbarkeit, Reviews. Einfache Reports, technische Details nur wenn sie eine sichtbare Änderung erklären.
- **E-Commerce:** Checkout-UX, Page Speed, Mobile, Zahlungsmethoden — direkter Umsatzhebel (Baymard). Extra-Kosten-Transparenz und Guest-Checkout sind Top-Abbruchtreiber (40 % der Abbrecher nennen zu hohe Zusatzkosten als Grund; 62 % der Shops machen Guest-Checkout nicht zur prominentesten Option).
- **B2B/SaaS:** Conversion entlang der Buyer Journey, Content-Gaps vs. Wettbewerb, Lead-Qualität; „jeder Reibungspunkt kostet qualifizierte Leads und Enterprise-Deals".
- **Enterprise:** Skalierbare technische Audits (Crawl-Budget, Log-Files, Internationalisierung/hreflang), Governance.

#### Deutscher/europäischer Markt gesondert
- **DSGVO + TDDDG (früher TTDSG, umbenannt 14.5.2024):** § 25 TDDDG verlangt aktive Einwilligung vor dem Setzen nicht-essenzieller Cookies; Accept/Reject müssen gleich prominent sein (DSK-Orientierungshilfe); granulare Einwilligung; Consent-Logs (Empfehlung: mind. 3 Jahre auf EU-Servern). Cookie-Walls generell unzulässig. Einwilligungsverwaltungsverordnung (EinwV) seit 1. April 2025 (freiwillige PIMS/Consent-Management-Dienste). Zur Einordnung des Aufwands: laut Bitkom sagen 81 % der Unternehmen, die DSGVO erschwere Geschäftsprozesse.
- **BFSG (Barrierefreiheitsstärkungsgesetz), seit 28. Juni 2025:** setzt EU-Richtlinie 2019/882 (EAA) um; verlangt WCAG 2.1 AA / EN 301 549 für E-Commerce und consumer-facing Dienste; Accessibility-Statement Pflicht; Bußgelder bis 100.000 €; Kleinstunternehmen (<10 MA und <2 Mio. € Umsatz) bei Dienstleistungen ausgenommen. Aktualisiertes EN 301 549 wird auf WCAG 2.2 verweisen (Veröffentlichung im EU-Amtsblatt für Mai 2026 geplant). Marktrealität: Der 3. Aktion-Mensch/Google-Testbericht (17.06.2025) fand nur ~ein Drittel der 65 meistbesuchten Shops zumindest teilweise barrierefrei; der vorherige Bericht 2024 hatte „vier von fünf" (56 von 71 getesteten Shops) als nicht barrierefrei eingestuft.

#### AI-Sichtbarkeit (AEO/GEO) — wichtige Einordnung
AEO/GEO-Audits prüfen Crawlability für AI-Bots, answer-first Content, strukturierte Daten, Entity-Klarheit und llms.txt. **Wichtiger Vorbehalt (belegt):** Google hat am 15. Mai 2026 offiziell klargestellt, dass strukturierte Daten für AI Overviews nicht erforderlich sind und llms.txt sowie Content-Chunking von Google-Systemen nicht genutzt werden; llms.txt hat „keine breit validierte Evidenz" für bessere AI-Sichtbarkeit. Der praktische Rat: klassische SEO-Fundamente (einzigartiger Content, saubere Indexierbarkeit, Page Experience) + externes AI-Visibility-Monitoring (Profound, Peec AI, Semrush) statt spekulativer llms.txt-Optimierung.

### 3) Was Kunden immer wissen wollen

Die wiederkehrenden Kundenfragen (Branchenkonsens) und ihre KPI-Übersetzung:

| Kundenfrage | Technisches Finding | Business-KPI-Übersetzung |
|---|---|---|
| „Warum ranke ich nicht?" | Indexierung, Technical SEO, Content-Gaps | Sichtbarkeit, organischer Traffic |
| „Warum konvertiert die Seite nicht?" | UX-Friction, Checkout-Barrieren, langsame Seiten | Conversion Rate, Umsatz |
| „Ist meine Seite schnell genug?" | Core Web Vitals (LCP/INP/CLS) | Conversion, Bounce, Umsatz (+0,1 s → +8,4 % Conv.) |
| „Was macht die Konkurrenz besser?" | Benchmark, Backlink-/Content-Gap | Wettbewerbsposition, Marktanteil |
| „Was kostet die Behebung?" | Effort-Schätzung je Finding | Investition, Aufwand |
| „Was bringt mir das an Umsatz/Leads?" | Impact-Schätzung, Traffic→Conversion | Leads, Umsatz, ROI |
| „Bin ich rechtlich sicher?" | DSGVO/Consent, BFSG/WCAG | Risiko, Bußgeld/Abmahnung |
| „Werde ich von KI gefunden?" | AEO/GEO, Citations in ChatGPT/Perplexity/AI Overviews | Zukünftige Sichtbarkeit |

**Übersetzungsprinzip:** Businessowner denken in ROI, Wettbewerbsposition, Erfolgsgeschichten, konkreten nächsten Schritten und Quick Wins — nicht in Canonicals und Schema. Jede Empfehlung sollte Grund + erwarteten Impact + Owner enthalten. Rankings sind für Kunden am leichtesten verständlich, aber „nützlich und gefährlich zugleich", weil eine einzelne Rankingbewegung ein Gespräch dominieren kann, obwohl die kommerziellen Daten anders laufen — deshalb Rankings in Business/Intent/Funnel gruppieren.

---

## Recommendations

### Empfohlene Kategorien-Struktur für einen Website-Audit-Report (direkt als Vorlage nutzbar)

**Teil A — Executive Summary (1 Seite, immer zuerst)**
- Gesamt-Health-Score 0–100 mit Ampel
- 3 wichtigste Befunde in Business-Sprache (Umsatz/Leads/Risiko)
- Ein Satz je Befund: Problem → Business-Impact → empfohlene Aktion
- „Erste 30 Tage"-Ausblick

**Teil B — Kategorie-Scores (Dashboard, 1 Seite)** — mit Gewichtungsvorschlag:
1. **Auffindbarkeit / Technical SEO & Indexierung** (Gewicht ~20 %) — Crawlability, robots.txt, Sitemap, Statuscodes, interne Verlinkung
2. **Performance & Core Web Vitals** (~15 %) — LCP <2,5 s, INP <200 ms, CLS <0,1; Felddaten (CrUX) 75. Perzentil
3. **Mobile-Freundlichkeit** (~10 %)
4. **UX & Conversion** (~15 %) — NNG-Heuristiken, Checkout/Formulare (Baymard bei E-Commerce)
5. **Content & Keyword-/AI-Abdeckung** (~15 %) — inkl. AEO/GEO als Unterpunkt
6. **Rechtssicherheit DE/EU** (~15 %) — DSGVO/TDDDG-Consent + Barrierefreiheit BFSG/WCAG 2.1 AA
7. **Security & Trust** (~5 %) — HTTPS, Header, Trust-Signale
8. **Analytics-/Tracking-Setup** (~5 %) — GA4, Conversion-Tracking

*Gewichtung ist eine begründete Einschätzung, kein Standard — für lokale Dienstleister Local SEO hochgewichten, für E-Commerce UX/Conversion und Performance, für B2B/SaaS Content/Conversion, für DE/EU-consumer-facing Rechtssicherheit deutlich höher.*

**Teil C — Priorisierte Befunde (Kern, Tabelle)**
Spalten: Issue | Kategorie | Severity (Critical/High/Medium/Low) | Impact (H/M/L) | Effort (H/M/L) | Priorität (P0/P1/P2) | Owner | erwarteter KPI-Effekt

**Teil D — Roadmap:** Quick Wins (P0, diese Woche) → P1 (dieser Monat) → P2 (nächstes Quartal), als Impact-vs-Effort-Matrix visualisiert.

**Teil E — Technischer Anhang:** URL-Level-Details, Screenshots, Crawl-Daten.

### Bewährte Darstellungselemente (Baukasten)
- 0–100-Score + Ampel je Kategorie, plus Trendlinie bei Folge-Audits
- Severity-Tags + Impact/Effort-Matrix
- Quick-Wins-Block ganz vorne
- Owner- und Aufwandsspalte in jeder Empfehlungstabelle
- Vorher/Nachher-Screenshots bei UX/Content
- 1 Wettbewerbs-Benchmark je Kernkategorie
- Revenue-/Lead-Impact als klar gekennzeichnete Schätzung

### Staged Next Steps
1. **Sofort:** Report-Template mit den 8 Kategorien + Executive-Summary-Seite + Priorisierungstabelle bauen (z. B. in Slides/Notion für Deliverable, Lighthouse+GSC+Crawler als Datengrundlage).
2. **Kurzfristig:** Für DE/EU-Kunden DSGVO/BFSG als fixe Pflicht-Sektion mit Bußgeld-Kontext etablieren — starker Auftrags-Trigger (Bitkom: 97 % der Unternehmen mit hohem Datenschutz-Aufwand; ~zwei Drittel der Shops noch nicht barrierefrei).
3. **Mittelfristig:** AEO/GEO als eigene Score-Kategorie ergänzen, aber konservativ (SEO-Fundamente betonen, llms.txt als „experimentell/low-confidence" kennzeichnen).
4. **Format:** Für Akquise 5-Min-Loom-Video testen; für Umsetzung PDF/Slides 24–48 h vor Call versenden; Fortschritt über Dashboard.

**Benchmarks, die die Empfehlung ändern würden:** Wenn eine belastbare Studie erscheint, die ein Deliverable-Format quantifiziert mit Umsetzung verknüpft, Format-Priorisierung anpassen. Wenn Google/CrUX-Thresholds oder EN 301 549 (→ WCAG 2.2, geplant Mai 2026) sich ändern, Score-Kriterien aktualisieren.

---

## Caveats
- **Format-Wirksamkeit ist nicht studienbelegt:** Aussagen dazu, welches Reportformat „nachweislich" zu mehr Umsetzung/Abschluss führt, sind Branchenpraxis, keine harte Studienlage. Explizit gekennzeichnet.
- **Gewichtungen sind eigene Einschätzung:** Die Prozent-Gewichte der Kategorien-Struktur sind eine begründete Inferenz, kein Marktstandard.
- **Aktualität von Standards:** INP hat FID im März 2024 ersetzt (FID seit 9.9.2024 endgültig deprecated). Reports mit FID sind veraltet.
- **AI-Sichtbarkeit ist in Bewegung:** Googles Aussagen vom Mai 2026 widersprechen Teilen des GEO/AEO-Beratungsmarktes (llms.txt, Schema für AI). Hier bewusst konservativ.
- **Einige Statistiken mit Vorsicht:** „+0,1 s → +8,4 % Conversion" stammt aus Google/Deloitte „Milliseconds Make Millions" (Daten Ende 2019, vor Core Web Vitals) — weiterhin die kanonische Quelle, aber älter. Warenkorbabbruch 70,22 % ist Baymard-Durchschnitt über 50 Studien. Der Barrierefreiheits-Wert ist ein Test von 65–71 Shops (kein repräsentativer Survey); „vier von fünf" stammt aus dem 2024er-Bericht, der aktuellere 2025er-Bericht spricht von „~ein Drittel teilweise barrierefrei". Die Webflow-Zahlen (91 %, 52 %) stammen aus dem State-of-the-Website-Report; die 91 % kamen über eine Agentur-Zusammenfassung und sollten idealerweise am Original-PDF verifiziert werden. Round-Number-Stats ohne rückverfolgbare Primärquelle (z. B. „Amazon 100 ms = 1 % Umsatz", „$4 Bio. Warenkorbverlust") wurden bewusst nicht als Fakt verwendet.
- **Interne Quellen:** In den verbundenen Konnektoren (Drive/Slack/Confluence/Jira) lag kein eigenes Audit-Material vor; falls an anderer Stelle (Notion, andere Drives) doch Vorlagen existieren, wurden sie nicht erfasst.