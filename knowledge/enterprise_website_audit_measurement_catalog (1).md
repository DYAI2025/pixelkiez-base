# Enterprise Website Audit Measurement Catalog
Research date: 2026-08-26  |  Scope: measurement architecture, not a specific website audit.

> Truth discipline: standards/platform metrics, research evidence, industry metrics, vendor scores, proxies and heuristics are kept separate. `WEIGHTING_REQUIRES_PRODUCT_DECISION` is retained wherever no evidence-based universal weighting exists.

## 1. EXECUTIVE RESEARCH SUMMARY
- **Audit dimensions:** 54 (C01-C50 baseline + C51-C54 gap findings).
- **Unique normalized measurement concepts:** 138.
- **Analysis methods:** 30.
- **Source ledger:** 44 central sources; primary/platform/standards sources prioritized.
- **Coverage status:** `COVERAGE_SATURATION_REACHED` relative to the documented discovery strategy, not global completeness.
- **Most mature areas:** Core Web Vitals/field-vs-lab performance, HTTP/robots/canonical/index directives, Search Console definitions, HTML semantics, WCAG-oriented accessibility, HTTP status/reliability measurement.
- **Least mature areas:** cross-platform GEO/AI visibility, passage retrievability, AI entity representation, web sustainability scoring, browser-agent operability.
- **Central decision:** there is no evidence-backed universal website score. A client-facing composite may be a product decision, but weights must remain transparent and category blockers cannot be hidden by averages.

### Evidence distribution
| Evidence class | Count |
|---|---:|
| E1_STANDARDIZED | 15 |
| E2_PLATFORM_OFFICIAL | 43 |
| E3_RESEARCH_VALIDATED | 4 |
| E4_REPRODUCIBLE_INDUSTRY_METRIC | 34 |
| E5_VENDOR_SPECIFIC | 5 |
| E6_PLAUSIBLE_PROXY | 32 |
| E7_PRACTITIONER_HEURISTIC | 2 |
| E8_UNCLEAR_OR_UNVALIDATED | 3 |

## 2. ENTERPRISE WEBSITE AUDIT TAXONOMY
| ID | Kategorie | Zweck | Was wird beurteilt? | Datenquellen | Reifegrad | Skill-Relevanz |
|---|---|---|---|---|---|---|
| C01 | Measurement Architecture & Audit Governance | Reproduzierbare Evidenz und Diagnose für Measurement Architecture & Audit Governance | 3 normalisierte Konzepte | HYBRID, MANUAL | MEDIUM | P0 |
| C02 | Web Performance & Core User Experience Metrics | Reproduzierbare Evidenz und Diagnose für Web Performance & Core User Experience Metrics | 5 normalisierte Konzepte | FIELD | HIGH | P0 |
| C03 | Field Data / RUM / CrUX | Reproduzierbare Evidenz und Diagnose für Field Data / RUM / CrUX | 5 normalisierte Konzepte | FIELD, HYBRID | HIGH | P0 |
| C04 | Synthetic / Lab Performance Testing | Reproduzierbare Evidenz und Diagnose für Synthetic / Lab Performance Testing | 5 normalisierte Konzepte | LAB, SYNTHETIC | HIGH | P0 |
| C05 | Server Performance, TTFB, Backend & Hosting | Reproduzierbare Evidenz und Diagnose für Server Performance, TTFB, Backend & Hosting | 3 normalisierte Konzepte | FIELD, SERVER | MEDIUM | P0 |
| C06 | Network, HTTP, TLS, DNS, CDN, Caching & Compression | Reproduzierbare Evidenz und Diagnose für Network, HTTP, TLS, DNS, CDN, Caching & Compression | 5 normalisierte Konzepte | CRAWL, SERVER, SYNTHETIC | HIGH | P0 |
| C07 | JavaScript Runtime, Main Thread & Rendering | Reproduzierbare Evidenz und Diagnose für JavaScript Runtime, Main Thread & Rendering | 3 normalisierte Konzepte | LAB | MEDIUM | P1 |
| C08 | CSS, Fonts, Images, Video & Resource Optimization | Reproduzierbare Evidenz und Diagnose für CSS, Fonts, Images, Video & Resource Optimization | 4 normalisierte Konzepte | CRAWL, LAB | MEDIUM | P1 |
| C09 | Mobile, Responsive Design & Device Experience | Reproduzierbare Evidenz und Diagnose für Mobile, Responsive Design & Device Experience | 2 normalisierte Konzepte | CRAWL, LAB | MEDIUM | P1 |
| C10 | Crawlability | Reproduzierbare Evidenz und Diagnose für Crawlability | 3 normalisierte Konzepte | CRAWL, HYBRID | HIGH | P0 |
| C11 | Indexability | Reproduzierbare Evidenz und Diagnose für Indexability | 2 normalisierte Konzepte | HYBRID, SEARCH_PLATFORM | HIGH | P0 |
| C12 | Robots Directives, Sitemaps, Canonicals & URL Management | Reproduzierbare Evidenz und Diagnose für Robots Directives, Sitemaps, Canonicals & URL Management | 3 normalisierte Konzepte | CRAWL, HYBRID | HIGH | P0 |
| C13 | Technical SEO | Reproduzierbare Evidenz und Diagnose für Technical SEO | 2 normalisierte Konzepte | CRAWL | MEDIUM | P0 |
| C14 | On-Page SEO | Reproduzierbare Evidenz und Diagnose für On-Page SEO | 2 normalisierte Konzepte | CRAWL | MEDIUM | P1 |
| C15 | HTML Semantics & Document Structure | Reproduzierbare Evidenz und Diagnose für HTML Semantics & Document Structure | 2 normalisierte Konzepte | CRAWL, HYBRID | HIGH | P0 |
| C16 | Metadata Analysis | Reproduzierbare Evidenz und Diagnose für Metadata Analysis | 3 normalisierte Konzepte | CRAWL, HYBRID | MEDIUM | P0 |
| C17 | Titles, Meta Descriptions & SERP Representation | Reproduzierbare Evidenz und Diagnose für Titles, Meta Descriptions & SERP Representation | 2 normalisierte Konzepte | HYBRID, SEARCH_PLATFORM | MEDIUM | P1 |
| C18 | Structured Data / Schema / Rich Result Eligibility | Reproduzierbare Evidenz und Diagnose für Structured Data / Schema / Rich Result Eligibility | 2 normalisierte Konzepte | CRAWL, HYBRID | HIGH | P0 |
| C19 | Entity Representation & Semantic Machine Readability | Reproduzierbare Evidenz und Diagnose für Entity Representation & Semantic Machine Readability | 2 normalisierte Konzepte | CRAWL, HYBRID | LOW_TO_MEDIUM | P2 |
| C20 | Content Quality | Reproduzierbare Evidenz und Diagnose für Content Quality | 2 normalisierte Konzepte | HYBRID, MANUAL | MEDIUM | P1 |
| C21 | Search Intent & Query-Content Alignment | Reproduzierbare Evidenz und Diagnose für Search Intent & Query-Content Alignment | 1 normalisierte Konzepte | HYBRID | LOW_TO_MEDIUM | P1 |
| C22 | Content Coverage, Information Gain & Topical Structure | Reproduzierbare Evidenz und Diagnose für Content Coverage, Information Gain & Topical Structure | 1 normalisierte Konzepte | HYBRID | LOW_TO_MEDIUM | P2 |
| C23 | Duplicate / Near-Duplicate / Thin Content | Reproduzierbare Evidenz und Diagnose für Duplicate / Near-Duplicate / Thin Content | 2 normalisierte Konzepte | CRAWL | MEDIUM | P1 |
| C24 | Information Architecture | Reproduzierbare Evidenz und Diagnose für Information Architecture | 1 normalisierte Konzepte | CRAWL | MEDIUM | P1 |
| C25 | Internal Linking | Reproduzierbare Evidenz und Diagnose für Internal Linking | 2 normalisierte Konzepte | CRAWL | MEDIUM | P0 |
| C26 | Navigation, Hierarchy & Click Depth | Reproduzierbare Evidenz und Diagnose für Navigation, Hierarchy & Click Depth | 1 normalisierte Konzepte | MANUAL | MEDIUM | P1 |
| C27 | External Links, Backlinks & Off-Page Signals | Reproduzierbare Evidenz und Diagnose für External Links, Backlinks & Off-Page Signals | 2 normalisierte Konzepte | THIRD_PARTY | MEDIUM | P2 |
| C28 | Search Visibility, Impressions, Clicks, CTR & Query Performance | Reproduzierbare Evidenz und Diagnose für Search Visibility, Impressions, Clicks, CTR & Query Performance | 4 normalisierte Konzepte | SEARCH_PLATFORM | HIGH | P0 |
| C29 | International SEO, Hreflang & Localization | Reproduzierbare Evidenz und Diagnose für International SEO, Hreflang & Localization | 2 normalisierte Konzepte | CRAWL, MANUAL | MEDIUM | P1 |
| C30 | Local Search / Local SEO | Reproduzierbare Evidenz und Diagnose für Local Search / Local SEO | 2 normalisierte Konzepte | HYBRID, THIRD_PARTY | MEDIUM | P2 |
| C31 | Image SEO | Reproduzierbare Evidenz und Diagnose für Image SEO | 2 normalisierte Konzepte | HYBRID | MEDIUM | P1 |
| C32 | Video SEO | Reproduzierbare Evidenz und Diagnose für Video SEO | 2 normalisierte Konzepte | HYBRID | MEDIUM | P1 |
| C33 | GEO / Generative Engine Optimization | Reproduzierbare Evidenz und Diagnose für GEO / Generative Engine Optimization | 2 normalisierte Konzepte | THIRD_PARTY | LOW_TO_MEDIUM | P3 |
| C34 | AI Search Visibility | Reproduzierbare Evidenz und Diagnose für AI Search Visibility | 4 normalisierte Konzepte | SEARCH_PLATFORM, THIRD_PARTY | LOW_TO_MEDIUM | P3 |
| C35 | AI Citation / Mention / Source Visibility | Reproduzierbare Evidenz und Diagnose für AI Citation / Mention / Source Visibility | 3 normalisierte Konzepte | ANALYTICS, THIRD_PARTY | LOW_TO_MEDIUM | P3 |
| C36 | AI Crawler Accessibility & Machine Retrieval | Reproduzierbare Evidenz und Diagnose für AI Crawler Accessibility & Machine Retrieval | 3 normalisierte Konzepte | CRAWL | LOW_TO_MEDIUM | P2 |
| C37 | Passage-Level Retrievability & Answerability | Reproduzierbare Evidenz und Diagnose für Passage-Level Retrievability & Answerability | 2 normalisierte Konzepte | HYBRID, MANUAL | LOW_TO_MEDIUM | P2 |
| C38 | Brand / Entity Representation in AI Answer Systems | Reproduzierbare Evidenz und Diagnose für Brand / Entity Representation in AI Answer Systems | 2 normalisierte Konzepte | HYBRID, THIRD_PARTY | LOW_TO_MEDIUM | P3 |
| C39 | Accessibility & WCAG-Oriented Measurements | Reproduzierbare Evidenz und Diagnose für Accessibility & WCAG-Oriented Measurements | 3 normalisierte Konzepte | HYBRID, LAB | HIGH | P0 |
| C40 | UX Diagnostics & Usability Signals | Reproduzierbare Evidenz und Diagnose für UX Diagnostics & Usability Signals | 3 normalisierte Konzepte | MANUAL | MEDIUM | P1 |
| C41 | Security, HTTPS & Browser Trust Signals | Reproduzierbare Evidenz und Diagnose für Security, HTTPS & Browser Trust Signals | 3 normalisierte Konzepte | CRAWL, LAB, SYNTHETIC | HIGH | P0 |
| C42 | Privacy, Consent & Tracking Architecture | Reproduzierbare Evidenz und Diagnose für Privacy, Consent & Tracking Architecture | 3 normalisierte Konzepte | LAB | MEDIUM | P1 |
| C43 | Analytics Data Quality & Measurement Integrity | Reproduzierbare Evidenz und Diagnose für Analytics Data Quality & Measurement Integrity | 3 normalisierte Konzepte | ANALYTICS, HYBRID | MEDIUM | P1 |
| C44 | Conversion / Engagement Metrics | Reproduzierbare Evidenz und Diagnose für Conversion / Engagement Metrics | 3 normalisierte Konzepte | ANALYTICS | MEDIUM | P1 |
| C45 | Log-File Analysis & Search-Bot Behaviour | Reproduzierbare Evidenz und Diagnose für Log-File Analysis & Search-Bot Behaviour | 3 normalisierte Konzepte | SERVER | MEDIUM | P1 |
| C46 | Availability, Reliability & Error Monitoring | Reproduzierbare Evidenz und Diagnose für Availability, Reliability & Error Monitoring | 2 normalisierte Konzepte | SERVER | HIGH | P0 |
| C47 | Redirects, HTTP Status Codes & Error Architecture | Reproduzierbare Evidenz und Diagnose für Redirects, HTTP Status Codes & Error Architecture | 2 normalisierte Konzepte | CRAWL | HIGH | P0 |
| C48 | Web Technology / Architecture Diagnostics | Reproduzierbare Evidenz und Diagnose für Web Technology / Architecture Diagnostics | 2 normalisierte Konzepte | HYBRID | MEDIUM | P2 |
| C49 | Performance Budgets & Regression Monitoring | Reproduzierbare Evidenz und Diagnose für Performance Budgets & Regression Monitoring | 2 normalisierte Konzepte | HYBRID, LAB | MEDIUM | P1 |
| C50 | Competitive / Benchmark Analysis | Reproduzierbare Evidenz und Diagnose für Competitive / Benchmark Analysis | 2 normalisierte Konzepte | HYBRID, THIRD_PARTY | MEDIUM | P2 |
| C51 | Browser Compatibility & Web Platform Interoperability | Reproduzierbare Evidenz und Diagnose für Browser Compatibility & Web Platform Interoperability | 2 normalisierte Konzepte | LAB, THIRD_PARTY | MEDIUM | P1 |
| C52 | Third-Party Dependencies & Supply-Chain Footprint | Reproduzierbare Evidenz und Diagnose für Third-Party Dependencies & Supply-Chain Footprint | 3 normalisierte Konzepte | HYBRID, LAB | MEDIUM | P1 |
| C53 | Web Sustainability & Digital Resource Efficiency | Reproduzierbare Evidenz und Diagnose für Web Sustainability & Digital Resource Efficiency | 2 normalisierte Konzepte | LAB, MANUAL | EMERGING | P3 |
| C54 | Agentic Web / Browser-Agent Operability | Reproduzierbare Evidenz und Diagnose für Agentic Web / Browser-Agent Operability | 2 normalisierte Konzepte | HYBRID, LAB | EMERGING | P3 |

## 3. CATEGORY EXPLANATIONS
### C01 — Measurement Architecture & Audit Governance
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Measurement Architecture & Audit Governance. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Audit evidence coverage, Measurement reproducibility status, Source freshness age.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, RELIABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Audit evidence coverage, Measurement reproducibility status, Source freshness age.
**Wichtigste Analyseverfahren:** Evidence-ledger audit governance
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C02 — Web Performance & Core User Experience Metrics
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Web Performance & Core User Experience Metrics. Der Katalog enthält hier 5 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Largest Contentful Paint (LCP), Interaction to Next Paint (INP), Cumulative Layout Shift (CLS), Core Web Vitals pass status, First Input Delay (FID).
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Largest Contentful Paint (LCP), Interaction to Next Paint (INP), Cumulative Layout Shift (CLS), Core Web Vitals pass status, First Input Delay (FID).
**Wichtigste Analyseverfahren:** CrUX field-data analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C03 — Field Data / RUM / CrUX
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Field Data / RUM / CrUX. Der Katalog enthält hier 5 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: CrUX p75 LCP, CrUX p75 INP, CrUX p75 CLS, RUM sample size, Field-lab delta.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, RELIABILITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** CrUX p75 LCP, CrUX p75 INP, CrUX p75 CLS, RUM sample size, Field-lab delta.
**Wichtigste Analyseverfahren:** CrUX field-data analysis, RUM instrumentation review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API, FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C04 — Synthetic / Lab Performance Testing
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Synthetic / Lab Performance Testing. Der Katalog enthält hier 5 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Lighthouse Performance score, Total Blocking Time (TBT), First Contentful Paint (FCP), Speed Index, Lab run variance.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, RELIABILITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Lighthouse Performance score, Total Blocking Time (TBT), First Contentful Paint (FCP), Speed Index, Lab run variance.
**Wichtigste Analyseverfahren:** Synthetic performance profiling
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C05 — Server Performance, TTFB, Backend & Hosting
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Server Performance, TTFB, Backend & Hosting. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Time to First Byte (TTFB), Server request duration, Backend error rate.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, RELIABILITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Time to First Byte (TTFB), Server request duration, Backend error rate.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C06 — Network, HTTP, TLS, DNS, CDN, Caching & Compression
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Network, HTTP, TLS, DNS, CDN, Caching & Compression. Der Katalog enthält hier 5 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: HTTP protocol version, Cache-Control policy, Compression encoding, TLS protocol version, DNS lookup latency.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, RELIABILITY, SECURITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** HTTP protocol version, Cache-Control policy, Compression encoding, TLS protocol version, DNS lookup latency.
**Wichtigste Analyseverfahren:** HTTP/TLS/DNS protocol inspection
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C07 — JavaScript Runtime, Main Thread & Rendering
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um JavaScript Runtime, Main Thread & Rendering. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Long task count, Main-thread time, JavaScript execution time.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Long task count, Main-thread time, JavaScript execution time.
**Wichtigste Analyseverfahren:** Synthetic performance profiling
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C08 — CSS, Fonts, Images, Video & Resource Optimization
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um CSS, Fonts, Images, Video & Resource Optimization. Der Katalog enthält hier 4 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Transferred page weight, Image transfer bytes, Font transfer bytes, Modern image format coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, SUSTAINABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Transferred page weight, Image transfer bytes, Font transfer bytes, Modern image format coverage.
**Wichtigste Analyseverfahren:** Synthetic performance profiling
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C09 — Mobile, Responsive Design & Device Experience
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Mobile, Responsive Design & Device Experience. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Responsive viewport configuration, Horizontal overflow incidence.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Responsive viewport configuration, Horizontal overflow incidence.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C10 — Crawlability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Crawlability. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: robots.txt fetch status, Crawl-allowed URL share, Orphan URL count.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, CRAWLING, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** robots.txt fetch status, Crawl-allowed URL share, Orphan URL count.
**Wichtigste Analyseverfahren:** Rendered technical crawl, URL indexation inspection
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C11 — Indexability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Indexability. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Indexable URL status, Indexed URL status in Google.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** INDEXING, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Indexable URL status, Indexed URL status in Google.
**Wichtigste Analyseverfahren:** Rendered technical crawl, URL indexation inspection
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C12 — Robots Directives, Sitemaps, Canonicals & URL Management
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Robots Directives, Sitemaps, Canonicals & URL Management. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Canonical declaration status, Sitemap capacity validity, Robots meta / X-Robots directive status.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, INDEXING, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Canonical declaration status, Sitemap capacity validity, Robots meta / X-Robots directive status.
**Wichtigste Analyseverfahren:** Rendered technical crawl
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C13 — Technical SEO
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Technical SEO. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: HTTP success/error distribution, HTTPS canonical coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, RELIABILITY, SECURITY, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** HTTP success/error distribution, HTTPS canonical coverage.
**Wichtigste Analyseverfahren:** Rendered technical crawl
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C14 — On-Page SEO
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um On-Page SEO. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Primary heading presence, Descriptive link text coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Primary heading presence, Descriptive link text coverage.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C15 — HTML Semantics & Document Structure
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um HTML Semantics & Document Structure. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: HTML validity / parse anomalies, Landmark/semantic element coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, AI_VISIBILITY, RELIABILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** HTML validity / parse anomalies, Landmark/semantic element coverage.
**Wichtigste Analyseverfahren:** Rendered technical crawl
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C16 — Metadata Analysis
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Metadata Analysis. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Document title presence, Meta description presence, Language metadata consistency.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Document title presence, Meta description presence, Language metadata consistency.
**Wichtigste Analyseverfahren:** Rendered technical crawl, Metadata conflict analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C17 — Titles, Meta Descriptions & SERP Representation
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Titles, Meta Descriptions & SERP Representation. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Title-link source consistency, SERP snippet representation review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Title-link source consistency, SERP snippet representation review.
**Wichtigste Analyseverfahren:** Metadata conflict analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C18 — Structured Data / Schema / Rich Result Eligibility
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Structured Data / Schema / Rich Result Eligibility. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Structured data syntax validity, Rich-result eligibility diagnostics.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Structured data syntax validity, Rich-result eligibility diagnostics.
**Wichtigste Analyseverfahren:** Rendered technical crawl, Structured-data validation
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C19 — Entity Representation & Semantic Machine Readability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Entity Representation & Semantic Machine Readability. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Machine-readable entity identifier coverage, Entity consistency across page signals.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Machine-readable entity identifier coverage, Entity consistency across page signals.
**Wichtigste Analyseverfahren:** Structured-data validation
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C20 — Content Quality
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Content Quality. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Content helpfulness evidence review, Content freshness status.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Content helpfulness evidence review, Content freshness status.
**Wichtigste Analyseverfahren:** Intent and content-fit review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** MANUAL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C21 — Search Intent & Query-Content Alignment
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Search Intent & Query-Content Alignment. Der Katalog enthält hier 1 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Query-content alignment.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CONVERSION, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Query-content alignment.
**Wichtigste Analyseverfahren:** Search Console query-performance analysis, Intent and content-fit review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C22 — Content Coverage, Information Gain & Topical Structure
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Content Coverage, Information Gain & Topical Structure. Der Katalog enthält hier 1 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Topic coverage gap.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Topic coverage gap.
**Wichtigste Analyseverfahren:** Intent and content-fit review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C23 — Duplicate / Near-Duplicate / Thin Content
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Duplicate / Near-Duplicate / Thin Content. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Exact duplicate content cluster count, Near-duplicate similarity.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, INDEXING, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Exact duplicate content cluster count, Near-duplicate similarity.
**Wichtigste Analyseverfahren:** Content duplicate clustering
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C24 — Information Architecture
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Information Architecture. Der Katalog enthält hier 1 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Information architecture depth distribution.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Information architecture depth distribution.
**Wichtigste Analyseverfahren:** Internal link-graph analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C25 — Internal Linking
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Internal Linking. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Internal inlink count, Broken internal link count.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, RELIABILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Internal inlink count, Broken internal link count.
**Wichtigste Analyseverfahren:** Internal link-graph analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C26 — Navigation, Hierarchy & Click Depth
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Navigation, Hierarchy & Click Depth. Der Katalog enthält hier 1 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Navigation task path length.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CONVERSION, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Navigation task path length.
**Wichtigste Analyseverfahren:** Internal link-graph analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** MANUAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C27 — External Links, Backlinks & Off-Page Signals
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um External Links, Backlinks & Off-Page Signals. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Referring domain count, Domain Rating / Authority Score.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Referring domain count, Domain Rating / Authority Score.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C28 — Search Visibility, Impressions, Clicks, CTR & Query Performance
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Search Visibility, Impressions, Clicks, CTR & Query Performance. Der Katalog enthält hier 4 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Google Search impressions, Google Search clicks, Google Search CTR, Google average position.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Google Search impressions, Google Search clicks, Google Search CTR, Google average position.
**Wichtigste Analyseverfahren:** Search Console query-performance analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C29 — International SEO, Hreflang & Localization
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um International SEO, Hreflang & Localization. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: hreflang cluster validity, Localization content parity review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** hreflang cluster validity, Localization content parity review.
**Wichtigste Analyseverfahren:** International annotation audit
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, MANUAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C30 — Local Search / Local SEO
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Local Search / Local SEO. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Local relevance completeness, NAP consistency.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Local relevance completeness, NAP consistency.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C31 — Image SEO
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Image SEO. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Image alt-text coverage, Image discoverability status.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, CRAWLING, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Image alt-text coverage, Image discoverability status.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C32 — Video SEO
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Video SEO. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Video page eligibility signals, Video transcript/caption availability.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, AI_VISIBILITY, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Video page eligibility signals, Video transcript/caption availability.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C33 — GEO / Generative Engine Optimization
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um GEO / Generative Engine Optimization. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: GEO experimental visibility score, AI-query coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, GEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** GEO experimental visibility score, AI-query coverage.
**Wichtigste Analyseverfahren:** AI visibility repeated-sampling experiment
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C34 — AI Search Visibility
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um AI Search Visibility. Der Katalog enthält hier 4 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Google generative-AI impressions, Google generative-AI clicks, Vendor AI Share of Voice, AI answer inclusion rate.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, BUSINESS, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Google generative-AI impressions, Google generative-AI clicks, Vendor AI Share of Voice, AI answer inclusion rate.
**Wichtigste Analyseverfahren:** AI visibility repeated-sampling experiment
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C35 — AI Citation / Mention / Source Visibility
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um AI Citation / Mention / Source Visibility. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: AI citation rate, AI mention rate, ChatGPT referral sessions.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, BUSINESS, GEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** AI citation rate, AI mention rate, ChatGPT referral sessions.
**Wichtigste Analyseverfahren:** AI visibility repeated-sampling experiment
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C36 — AI Crawler Accessibility & Machine Retrieval
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um AI Crawler Accessibility & Machine Retrieval. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: OAI-SearchBot crawl permission, Googlebot crawl permission, AI crawler policy matrix.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, CRAWLING, INDEXING. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** OAI-SearchBot crawl permission, Googlebot crawl permission, AI crawler policy matrix.
**Wichtigste Analyseverfahren:** AI crawler accessibility audit
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C37 — Passage-Level Retrievability & Answerability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Passage-Level Retrievability & Answerability. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Passage answerability review, Heading-to-passage structure.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, AI_VISIBILITY, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Passage answerability review, Heading-to-passage structure.
**Wichtigste Analyseverfahren:** Passage answerability audit
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** MANUAL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C38 — Brand / Entity Representation in AI Answer Systems
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Brand / Entity Representation in AI Answer Systems. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: AI entity representation consistency, AI attribution accuracy.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, BUSINESS. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** AI entity representation consistency, AI attribution accuracy.
**Wichtigste Analyseverfahren:** AI visibility repeated-sampling experiment
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C39 — Accessibility & WCAG-Oriented Measurements
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Accessibility & WCAG-Oriented Measurements. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: WCAG 2.2 success-criterion conformance, Target Size (Minimum) compliance, Automated accessibility issue count.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, BUSINESS, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** WCAG 2.2 success-criterion conformance, Target Size (Minimum) compliance, Automated accessibility issue count.
**Wichtigste Analyseverfahren:** WCAG-EM-oriented accessibility evaluation
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C40 — UX Diagnostics & Usability Signals
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um UX Diagnostics & Usability Signals. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Task completion rate, Time on task, Usability heuristic review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, CONVERSION, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Task completion rate, Time on task, Usability heuristic review.
**Wichtigste Analyseverfahren:** Task-based usability testing, Heuristic usability review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** MANUAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C41 — Security, HTTPS & Browser Trust Signals
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Security, HTTPS & Browser Trust Signals. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: HTTPS availability, Mixed content incidence, Security-header configuration review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** RELIABILITY, SECURITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** HTTPS availability, Mixed content incidence, Security-header configuration review.
**Wichtigste Analyseverfahren:** HTTP/TLS/DNS protocol inspection
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C42 — Privacy, Consent & Tracking Architecture
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Privacy, Consent & Tracking Architecture. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Consent prior to non-essential storage/tracking, GPC signal handling, Tracker/cookie inventory.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, PRIVACY, SECURITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Consent prior to non-essential storage/tracking, GPC signal handling, Tracker/cookie inventory.
**Wichtigste Analyseverfahren:** Consent-state browser audit
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C43 — Analytics Data Quality & Measurement Integrity
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Analytics Data Quality & Measurement Integrity. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Analytics event schema validity, Analytics thresholding status, Measurement-plan coverage.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, CONVERSION, RELIABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Analytics event schema validity, Analytics thresholding status, Measurement-plan coverage.
**Wichtigste Analyseverfahren:** RUM instrumentation review, Analytics implementation QA
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C44 — Conversion / Engagement Metrics
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Conversion / Engagement Metrics. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: GA4 engagement rate, GA4 bounce rate, Key-event conversion rate.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, CONVERSION, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** GA4 engagement rate, GA4 bounce rate, Key-event conversion rate.
**Wichtigste Analyseverfahren:** Analytics implementation QA
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** EXTERNAL_API. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C45 — Log-File Analysis & Search-Bot Behaviour
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Log-File Analysis & Search-Bot Behaviour. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Verified search-bot request share, Bot status-code distribution, Bot crawl waste proxy.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, RELIABILITY, SEO. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Verified search-bot request share, Bot status-code distribution, Bot crawl waste proxy.
**Wichtigste Analyseverfahren:** Search-bot log analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C46 — Availability, Reliability & Error Monitoring
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Availability, Reliability & Error Monitoring. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Availability SLI, Latency percentile SLI.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, RELIABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Availability SLI, Latency percentile SLI.
**Wichtigste Analyseverfahren:** Reliability SLI/SLO review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C47 — Redirects, HTTP Status Codes & Error Architecture
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Redirects, HTTP Status Codes & Error Architecture. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Redirect chain length, 4xx/5xx URL incidence.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** CRAWLING, PERFORMANCE, RELIABILITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Redirect chain length, 4xx/5xx URL incidence.
**Wichtigste Analyseverfahren:** HTTP/TLS/DNS protocol inspection
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C48 — Web Technology / Architecture Diagnostics
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Web Technology / Architecture Diagnostics. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Technology inventory, Client-side rendering dependency.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** AI_VISIBILITY, BUSINESS, CRAWLING, PERFORMANCE, RELIABILITY, SECURITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Technology inventory, Client-side rendering dependency.
**Wichtigste Analyseverfahren:** Kategorieübergreifender Crawl/Review gemäß Metric Record.
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C49 — Performance Budgets & Regression Monitoring
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Performance Budgets & Regression Monitoring. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Performance budget breach count, Performance regression delta.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** PERFORMANCE, RELIABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Performance budget breach count, Performance regression delta.
**Wichtigste Analyseverfahren:** Synthetic performance profiling, Performance regression gate
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C50 — Competitive / Benchmark Analysis
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Competitive / Benchmark Analysis. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Peer percentile benchmark, Competitive feature/content gap.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, SEO, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Peer percentile benchmark, Competitive feature/content gap.
**Wichtigste Analyseverfahren:** Competitive cohort benchmarking
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C51 — Browser Compatibility & Web Platform Interoperability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Browser Compatibility & Web Platform Interoperability. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Baseline feature status, Unsupported-browser error incidence.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, RELIABILITY, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Baseline feature status, Unsupported-browser error incidence.
**Wichtigste Analyseverfahren:** Cross-browser compatibility matrix
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C52 — Third-Party Dependencies & Supply-Chain Footprint
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Third-Party Dependencies & Supply-Chain Footprint. Der Katalog enthält hier 3 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Third-party request count, Third-party transfer bytes, Third-party dependency criticality review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, PRIVACY, RELIABILITY, SECURITY, SUSTAINABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Third-party request count, Third-party transfer bytes, Third-party dependency criticality review.
**Wichtigste Analyseverfahren:** Third-party dependency analysis
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C53 — Web Sustainability & Digital Resource Efficiency
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Web Sustainability & Digital Resource Efficiency. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Transferred bytes per task/page, Sustainability guideline review.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** BUSINESS, PERFORMANCE, SUSTAINABILITY. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Transferred bytes per task/page, Sustainability guideline review.
**Wichtigste Analyseverfahren:** Sustainability evidence review
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** FULL, MANUAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

### C54 — Agentic Web / Browser-Agent Operability
**Was wird hier untersucht?** Beobachtbare Eigenschaften, Messwerte und Diagnoseverfahren rund um Agentic Web / Browser-Agent Operability. Der Katalog enthält hier 2 kanonische Messkonzepte.
**Warum existiert diese Kategorie?** Sie trennt diese Evidenzdomäne von benachbarten Bereichen, damit Messpopulation, Tool, Ursache und Aussagegrenze nicht vermischt werden.
**Welche Website-Eigenschaften erzeugen die Messwerte?** Relevante technische, inhaltliche oder verhaltensbezogene Eigenschaften; zentrale Datensätze: Agent-accessible interaction success, Semantic action discoverability.
**Was können die Ergebnisse aussagen?** Sie können Zustände, Verteilungen, Abweichungen oder reproduzierbare Risiken im definierten Scope belegen, soweit die jeweilige Evidenzklasse trägt.
**Was können sie NICHT aussagen?** Kein Einzelwert beweist automatisch Ranking, Conversion-Uplift, Umsatzwirkung oder generelle Website-Qualität. Plattform-, Tool-, Stichproben- und Kontextgrenzen bleiben erhalten.
**Potenzieller Impact:** ACCESSIBILITY, AI_VISIBILITY, BUSINESS, UX. Die Art der Impact-Evidenz wird pro Messkonzept separat geführt.
**Wichtigste Messgrößen:** Agent-accessible interaction success, Semantic action discoverability.
**Wichtigste Analyseverfahren:** Agentic web task operability experiment
**Typische Fehlinterpretationen:** numerische Werte ohne Population/Tool/Version vergleichen; Proxies als Kausalbeweis lesen; absichtliche Konfiguration als Fehler werten; Vendor-Scores als Standards behandeln.
**Automatisierbarkeit im späteren Skill:** PARTIAL. Manuelle Reviews bleiben dort Pflicht, wo Semantik, Nutzeraufgabe, Accessibility-Conformance oder Rechts-/Business-Kontext nicht deterministisch messbar sind.

## 4. MASTER KPI & METRIC CATALOG
Die vollständigen Records stehen zusätzlich in `metric_catalog.jsonl` und `metric_catalog.csv`.

| ID | Kategorie | Name | Typ | Evidenz | Definition | Messprinzip | Formel | Einheit | Modus | Scope | Threshold/Benchmark | Impact | Impact-Evidenz | Tool | Automatisierung | Scoring | Confidence | Primärquelle |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| M001 | C01 | Audit evidence coverage | KPI | E6_PLAUSIBLE_PROXY | Share of material findings backed by traceable source or direct measurement. | Count evidence-backed material findings divided by all material findings. | backed_material_findings / all_material_findings * 100 | % | MANUAL | SITE | Target range is product-defined; no universal standard. | BUSINESS, RELIABILITY | PLAUSIBLE_INDIRECT_RELATION | report validator | PARTIAL | SCORE_ELIGIBLE_WITH_CONTEXT | LOW | S035 |
| M002 | C01 | Measurement reproducibility status | DIAGNOSTIC_SIGNAL | E6_PLAUSIBLE_PROXY | Whether another run can reproduce a result under stated conditions. | Persist tool version, inputs, environment and collection time; rerun and compare. | NOT_APPLICABLE | status | HYBRID | SITE | NONE_OFFICIAL | RELIABILITY | TECHNICAL_DEPENDENCY | audit harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S035 |
| M003 | C01 | Source freshness age | METRIC | E6_PLAUSIBLE_PROXY | Age of evidence supporting a rule or benchmark. | Difference between verification date and source publication/update date. | NOT_APPLICABLE | days | MANUAL | OTHER | Context-dependent; staleness is domain-specific. | RELIABILITY | PLAUSIBLE_INDIRECT_RELATION | source ledger | FULL | DIAGNOSTIC_ONLY | LOW | S035 |
| M004 | C02 | Largest Contentful Paint (LCP) | METRIC | E2_PLATFORM_OFFICIAL | Render time of the largest visible content element in the viewport. | Use PerformanceObserver/web-vitals in field or compatible lab instrumentation. | NOT_APPLICABLE | ms | FIELD | PAGE | Good <=2500 ms; poor >4000 ms at p75, mobile/desktop segmented. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX, web-vitals, PageSpeed Insights | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M005 | C02 | Interaction to Next Paint (INP) | METRIC | E2_PLATFORM_OFFICIAL | Latency of user interactions, represented by a high percentile interaction latency per page view. | Event Timing based field measurement; aggregate page loads at p75. | NOT_APPLICABLE | ms | FIELD | PAGE | Good <=200 ms; poor >500 ms at p75. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX, web-vitals | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M006 | C02 | Cumulative Layout Shift (CLS) | METRIC | E2_PLATFORM_OFFICIAL | Accumulated unexpected layout shift score during page lifetime. | Layout Instability API / web-vitals; aggregate p75. | NOT_APPLICABLE | score | FIELD | PAGE | Good <=0.1; poor >0.25 at p75. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX, web-vitals | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M007 | C02 | Core Web Vitals pass status | KPI | E2_PLATFORM_OFFICIAL | Whether all three current Core Web Vitals meet good thresholds at p75. | Evaluate LCP, INP and CLS at the 75th percentile for the target population. | NOT_APPLICABLE | binary | FIELD | ORIGIN | PASS only if all three meet good thresholds at p75. | PERFORMANCE, UX, SEO | PLATFORM_RECOMMENDATION | CrUX | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M008 | C02 | First Input Delay (FID) | METRIC | E2_PLATFORM_OFFICIAL | Legacy input delay metric formerly used as a Core Web Vital. | Historical Event Timing measurement. | NOT_APPLICABLE | ms | FIELD | PAGE | DEPRECATED as Core Web Vital; replaced by INP. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | historical CrUX | FULL | NOT_SUITABLE_FOR_SCORING | HIGH | S001 |
| M009 | C03 | CrUX p75 LCP | METRIC | E2_PLATFORM_OFFICIAL | 75th percentile LCP from eligible Chrome real-user population. | Query CrUX API/History API or first-party interfaces. | NOT_APPLICABLE | ms | FIELD | ORIGIN | Use CWV threshold only with CrUX population/scope disclosed. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M010 | C03 | CrUX p75 INP | METRIC | E2_PLATFORM_OFFICIAL | 75th percentile INP from eligible Chrome real-user population. | Query CrUX API/History API. | NOT_APPLICABLE | ms | FIELD | ORIGIN | Use CWV threshold with field-population caveats. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M011 | C03 | CrUX p75 CLS | METRIC | E2_PLATFORM_OFFICIAL | 75th percentile CLS from eligible Chrome real-user population. | Query CrUX API/History API. | NOT_APPLICABLE | score | FIELD | ORIGIN | Use CWV threshold with field-population caveats. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | CrUX API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M012 | C03 | RUM sample size | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Count of observations underlying a field measurement. | Count valid telemetry events/page views per metric/window. | NOT_APPLICABLE | count | FIELD | SITE | No universal sufficient sample size; depends on variance and decision. | RELIABILITY | TECHNICAL_DEPENDENCY | RUM platform | FULL | DIAGNOSTIC_ONLY | MEDIUM | S001 |
| M013 | C03 | Field-lab delta | DIAGNOSTIC_SIGNAL | E6_PLAUSIBLE_PROXY | Difference between field and laboratory measurements for a nominally related experience signal. | Compare normalized lab and field values only after documenting population and environment differences. | NOT_APPLICABLE | delta | HYBRID | PAGE | No universal threshold; diagnostic only. | PERFORMANCE | PLAUSIBLE_INDIRECT_RELATION | CrUX, Lighthouse | FULL | DIAGNOSTIC_ONLY | LOW | S001 |
| M014 | C04 | Lighthouse Performance score | COMPOSITE_SCORE | E5_VENDOR_SPECIFIC | Google Lighthouse composite lab performance score. | Run Lighthouse with declared version/device/network; score is weighted from lab metrics and scoring curves. | NOT_APPLICABLE | 0-100 | LAB | PAGE | Vendor score; thresholds/categories are Lighthouse-specific, not universal website quality. | PERFORMANCE | PLATFORM_RECOMMENDATION | Lighthouse | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S001 |
| M015 | C04 | Total Blocking Time (TBT) | PROXY | E2_PLATFORM_OFFICIAL | Lab sum of main-thread blocking time above long-task threshold in a defined window. | Synthetic browser trace; sum blocking portions of long tasks. | NOT_APPLICABLE | ms | LAB | PAGE | Use tool-version thresholds only; TBT is a lab proxy, not INP. | PERFORMANCE, UX | PLAUSIBLE_INDIRECT_RELATION | Lighthouse | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M016 | C04 | First Contentful Paint (FCP) | METRIC | E2_PLATFORM_OFFICIAL | Time until first content is painted. | Performance Paint Timing in browser/lab or field. | NOT_APPLICABLE | ms | LAB | PAGE | Tool-specific good/poor thresholds; not a Core Web Vital. | PERFORMANCE, UX | PLATFORM_RECOMMENDATION | Lighthouse, CrUX | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M017 | C04 | Speed Index | METRIC | E5_VENDOR_SPECIFIC | Visual progression metric used in synthetic testing. | Analyze video/filmstrip of viewport completeness over time. | NOT_APPLICABLE | ms | LAB | PAGE | Tool-specific scoring only. | PERFORMANCE, UX | PLAUSIBLE_INDIRECT_RELATION | Lighthouse, WebPageTest | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S035 |
| M018 | C04 | Lab run variance | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Dispersion across repeated synthetic runs. | Repeat same test profile and compute dispersion/quantiles. | NOT_APPLICABLE | statistic | SYNTHETIC | PAGE | No universal threshold; report median and spread. | RELIABILITY | TECHNICAL_DEPENDENCY | Lighthouse CI, WebPageTest | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M019 | C05 | Time to First Byte (TTFB) | METRIC | E2_PLATFORM_OFFICIAL | Elapsed time from navigation request until first response byte, including network/server components. | Navigation Timing or field tooling. | NOT_APPLICABLE | ms | FIELD | PAGE | Diagnostic thresholds may be platform-specific; not a Core Web Vital. | PERFORMANCE, UX | TECHNICAL_DEPENDENCY | Navigation Timing, CrUX | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S001 |
| M020 | C05 | Server request duration | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Backend time spent serving a request in instrumented systems. | Server APM/OpenTelemetry span or metric. | NOT_APPLICABLE | s | SERVER | SERVER | SLO target is service-specific. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | OpenTelemetry, APM | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S024 |
| M021 | C05 | Backend error rate | KPI | E4_REPRODUCIBLE_INDUSTRY_METRIC | Fraction of server requests classified as errors. | Count error responses/events divided by valid requests. | error_requests / valid_requests * 100 | % | SERVER | SERVER | SLO target is service-specific. | RELIABILITY, BUSINESS | TECHNICAL_DEPENDENCY | APM, logs | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S024 |
| M022 | C06 | HTTP protocol version | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Protocol used for the audited response path. | Inspect negotiated HTTP version at client/network layer. | NOT_APPLICABLE | enum | SERVER | RESOURCE | No universal score; HTTP/3 adoption is contextual. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | curl, browser devtools | FULL | DIAGNOSTIC_ONLY | HIGH | S020 |
| M023 | C06 | Cache-Control policy | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | HTTP caching directives applied to responses. | Parse Cache-Control and related response metadata against RFC semantics. | NOT_APPLICABLE | directives | CRAWL | RESOURCE | No single universal max-age; resource semantics govern policy. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | crawler, curl | FULL | DIAGNOSTIC_ONLY | HIGH | S021 |
| M024 | C06 | Compression encoding | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Whether transferable resources use content compression where applicable. | Inspect Content-Encoding and transferred/resource sizes. | NOT_APPLICABLE | enum | CRAWL | RESOURCE | No universal threshold. | PERFORMANCE | TECHNICAL_DEPENDENCY | crawler, browser devtools | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M025 | C06 | TLS protocol version | STANDARD_OR_REQUIREMENT | E1_STANDARDIZED | TLS version negotiated for HTTPS. | Perform TLS handshake and inspect protocol/cipher. | NOT_APPLICABLE | version | SERVER | DOMAIN | TLS 1.3 currently specified by RFC 9846; support requirements remain context-specific. | SECURITY, RELIABILITY | TECHNICAL_DEPENDENCY | openssl, sslyze | FULL | DIAGNOSTIC_ONLY | HIGH | S022 |
| M026 | C06 | DNS lookup latency | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Time required for DNS resolution from a defined vantage point. | Measure resolver timing under controlled conditions. | NOT_APPLICABLE | ms | SYNTHETIC | DOMAIN | No universal threshold; highly geography/resolver dependent. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | dig, WebPageTest | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M027 | C07 | Long task count | METRIC | E2_PLATFORM_OFFICIAL | Count of main-thread tasks meeting the Long Tasks definition in a measurement window. | PerformanceObserver Long Tasks API; task threshold is 50 ms. | NOT_APPLICABLE | count | LAB | PAGE | Long task definition >=50 ms; acceptable count is context-specific. | PERFORMANCE, UX | TECHNICAL_DEPENDENCY | Chrome DevTools, PerformanceObserver | FULL | DIAGNOSTIC_ONLY | HIGH | S001 |
| M028 | C07 | Main-thread time | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | CPU time attributed to main-thread work during a defined trace window. | Browser performance trace categories. | NOT_APPLICABLE | ms | LAB | PAGE | No universal threshold. | PERFORMANCE, UX | TECHNICAL_DEPENDENCY | Chrome DevTools, Lighthouse | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M029 | C07 | JavaScript execution time | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Time spent parsing/compiling/executing JavaScript in a trace. | Aggregate JS-related trace events. | NOT_APPLICABLE | ms | LAB | PAGE | No universal threshold. | PERFORMANCE | TECHNICAL_DEPENDENCY | Chrome DevTools | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M030 | C08 | Transferred page weight | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Total encoded bytes transferred for a defined page load. | Sum network transfer sizes for in-scope resources. | NOT_APPLICABLE | bytes | LAB | PAGE | No universal threshold; use budgets/peer distributions. | PERFORMANCE, SUSTAINABILITY | PLAUSIBLE_INDIRECT_RELATION | HTTP Archive, WebPageTest | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S035 |
| M031 | C08 | Image transfer bytes | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Transferred bytes attributable to image resources. | Sum transfer sizes for image MIME/resource types. | NOT_APPLICABLE | bytes | LAB | PAGE | Budget is product/context-specific. | PERFORMANCE, SUSTAINABILITY | TECHNICAL_DEPENDENCY | crawler, WebPageTest | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M032 | C08 | Font transfer bytes | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Transferred bytes attributable to web fonts. | Sum font-resource transfer sizes. | NOT_APPLICABLE | bytes | LAB | PAGE | Budget is context-specific. | PERFORMANCE | TECHNICAL_DEPENDENCY | crawler, WebPageTest | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M033 | C08 | Modern image format coverage | PROXY | E6_PLAUSIBLE_PROXY | Share of eligible images delivered in efficient contemporary formats. | Classify image MIME/format and eligibility; calculate coverage. | NOT_APPLICABLE | % | CRAWL | SITE | No universal target; compatibility and image characteristics matter. | PERFORMANCE | PLAUSIBLE_INDIRECT_RELATION | crawler | FULL | DIAGNOSTIC_ONLY | LOW | S035 |
| M034 | C09 | Responsive viewport configuration | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Presence and suitability of mobile viewport configuration. | Parse viewport metadata and render at representative device widths. | NOT_APPLICABLE | status | CRAWL | PAGE | No numeric threshold; manual/render verification needed. | UX, SEO | PLATFORM_RECOMMENDATION | browser, crawler | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S015 |
| M035 | C09 | Horizontal overflow incidence | DIAGNOSTIC_SIGNAL | E6_PLAUSIBLE_PROXY | Presence of unintended horizontal overflow at tested viewport widths. | Render page at device classes and compare scroll width to viewport width. | NOT_APPLICABLE | count | LAB | PAGE | Zero unintended overflow is a practical target, not a universal standard metric. | UX, ACCESSIBILITY | PLAUSIBLE_INDIRECT_RELATION | Playwright, browser | FULL | DIAGNOSTIC_ONLY | LOW | S017 |
| M036 | C10 | robots.txt fetch status | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Availability and parseability of robots.txt for an origin. | Fetch /robots.txt and parse per RFC 9309. | NOT_APPLICABLE | status | CRAWL | ORIGIN | RFC behavior applies; absence is not automatically an SEO defect. | CRAWLING, AI_VISIBILITY | TECHNICAL_DEPENDENCY | crawler, curl | FULL | DIAGNOSTIC_ONLY | HIGH | S006 |
| M037 | C10 | Crawl-allowed URL share | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Share of discovered URLs allowed for a selected crawler user-agent. | Evaluate each URL against robots rules for declared user-agent. | NOT_APPLICABLE | % | CRAWL | SITE | No universal higher-is-better target; intentional blocks are valid. | CRAWLING | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | MEDIUM | S006 |
| M038 | C10 | Orphan URL count | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Known URLs with no in-scope internal crawl path from chosen entry set. | Compare URL inventories from sitemap/log/search platform against internal crawl graph. | NOT_APPLICABLE | count | HYBRID | SITE | No universal threshold; context and intended entry paths matter. | CRAWLING, UX | PLAUSIBLE_INDIRECT_RELATION | crawler, sitemap, logs | PARTIAL | DIAGNOSTIC_ONLY | MEDIUM | S009 |
| M039 | C11 | Indexable URL status | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether a URL is technically eligible for indexing under observable directives/status. | Inspect status, robots directives, canonical and optionally Search Console indexed-version data. | NOT_APPLICABLE | status | HYBRID | PAGE | Eligibility does not prove inclusion in the index. | INDEXING, SEO | TECHNICAL_DEPENDENCY | crawler, URL Inspection API | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S005 |
| M040 | C11 | Indexed URL status in Google | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Search Console-reported state of the indexed version known to Google. | Query URL Inspection API for property-authorized URL. | NOT_APPLICABLE | status | SEARCH_PLATFORM | PAGE | No universal score; API reports indexed version, not a live test. | INDEXING | TECHNICAL_DEPENDENCY | Search Console URL Inspection API | EXTERNAL_API | DIAGNOSTIC_ONLY | HIGH | S005 |
| M041 | C12 | Canonical declaration status | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Presence and validity of canonical hints and conflicts. | Parse rel=canonical, redirects, sitemap and compare with selected canonical where available. | NOT_APPLICABLE | status | HYBRID | PAGE | Canonical is a signal, not a guarantee; redirects/rel canonical stronger than sitemap hints. | INDEXING, SEO | PLATFORM_RECOMMENDATION | crawler, Search Console | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S007 |
| M042 | C12 | Sitemap capacity validity | STANDARD_OR_REQUIREMENT | E2_PLATFORM_OFFICIAL | Whether sitemap files respect Google-supported size/URL limits. | Parse sitemap uncompressed size and URL count. | NOT_APPLICABLE | binary | CRAWL | RESOURCE | <=50 MB uncompressed and <=50,000 URLs per sitemap file. | CRAWLING, INDEXING | PLATFORM_RECOMMENDATION | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S009 |
| M043 | C12 | Robots meta / X-Robots directive status | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Indexing/serving directives expressed in HTML or HTTP headers. | Parse robots meta and X-Robots-Tag; ensure crawler can fetch page to observe directives. | NOT_APPLICABLE | directives | CRAWL | PAGE | Directive semantics are platform-defined; intentional noindex is not a defect. | INDEXING | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S008 |
| M044 | C13 | HTTP success/error distribution | METRIC | E1_STANDARDIZED | Distribution of HTTP response status classes across crawled URLs. | Crawl URL set and aggregate status codes by class. | NOT_APPLICABLE | % | CRAWL | SITE | Status semantics per RFC 9110; acceptable distribution is site-specific. | SEO, RELIABILITY, CRAWLING | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S020 |
| M045 | C13 | HTTPS canonical coverage | PROXY | E6_PLAUSIBLE_PROXY | Share of canonical/indexable URLs served over HTTPS. | Crawl canonical target set and classify scheme. | NOT_APPLICABLE | % | CRAWL | SITE | Modern production sites generally target full HTTPS; no standalone ranking guarantee. | SECURITY, SEO | PLATFORM_RECOMMENDATION | crawler | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | LOW | S015 |
| M046 | C14 | Primary heading presence | DIAGNOSTIC_SIGNAL | E6_PLAUSIBLE_PROXY | Presence and semantic plausibility of a primary page heading. | Parse document headings and compare visible hierarchy/content. | NOT_APPLICABLE | status | CRAWL | PAGE | No universal one-H1 ranking rule; evaluate semantic structure. | UX, SEO, ACCESSIBILITY | PLAUSIBLE_INDIRECT_RELATION | crawler, browser | PARTIAL | DIAGNOSTIC_ONLY | LOW | S010 |
| M047 | C14 | Descriptive link text coverage | PROXY | E2_PLATFORM_OFFICIAL | Share of internal links whose accessible text describes destination sufficiently for context. | Extract links/accessibility names; flag empty/generic labels for expert review. | NOT_APPLICABLE | % | CRAWL | SITE | No universal percentage threshold. | SEO, ACCESSIBILITY, UX | PLATFORM_RECOMMENDATION | crawler, accessibility engine | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S015 |
| M048 | C15 | HTML validity / parse anomalies | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Document-structure problems relative to HTML parsing/semantics. | Parse documents and optionally run standards validator; classify consequential issues. | NOT_APPLICABLE | count | CRAWL | PAGE | Not every validator warning has user/search impact. | ACCESSIBILITY, SEO, RELIABILITY | TECHNICAL_DEPENDENCY | Nu HTML Checker, parser | FULL | DIAGNOSTIC_ONLY | HIGH | S010 |
| M049 | C15 | Landmark/semantic element coverage | PROXY | E6_PLAUSIBLE_PROXY | Use of semantic HTML elements/landmarks appropriate to page structure. | Parse DOM and accessibility tree; compare to content roles. | NOT_APPLICABLE | coverage | HYBRID | PAGE | No universal score. | ACCESSIBILITY, AI_VISIBILITY, UX | PLAUSIBLE_INDIRECT_RELATION | browser, accessibility tree | PARTIAL | DIAGNOSTIC_ONLY | LOW | S010 |
| M050 | C16 | Document title presence | STANDARD_OR_REQUIREMENT | E1_STANDARDIZED | Presence of a non-empty HTML title element. | Parse document head. | NOT_APPLICABLE | binary | CRAWL | PAGE | Presence is normative HTML; quality remains contextual. | UX, SEO | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S010 |
| M051 | C16 | Meta description presence | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Presence of a meta description that may be used for snippets. | Parse meta name=description. | NOT_APPLICABLE | binary | CRAWL | PAGE | No official universal character-length threshold. | SEO | PLATFORM_RECOMMENDATION | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S014 |
| M052 | C16 | Language metadata consistency | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Consistency of declared document language with rendered content and localization metadata. | Parse html lang/hreflang and compare to content language detection/manual review. | NOT_APPLICABLE | status | HYBRID | PAGE | No universal numeric threshold. | ACCESSIBILITY, SEO, UX | TECHNICAL_DEPENDENCY | crawler, language detector | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S010 |
| M053 | C17 | Title-link source consistency | ANALYSIS_METHOD | E2_PLATFORM_OFFICIAL | Consistency among title element, prominent page title, headings, og:title and anchor references used as possible title-link sources. | Extract candidate title sources and compare for conflicts/truncation risk. | NOT_APPLICABLE | status | HYBRID | PAGE | Google may rewrite title links; no fixed title length ensures rendering. | SEO, UX | PLATFORM_RECOMMENDATION | crawler, browser | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S013 |
| M054 | C17 | SERP snippet representation review | QUALITATIVE_REVIEW | E2_PLATFORM_OFFICIAL | Structured assessment of how page content/meta may be represented in search snippets. | Compare query context, snippet sources, meta description and current search appearance where available. | NOT_APPLICABLE | review | SEARCH_PLATFORM | QUERY | No guarantee a supplied meta description is used. | SEO, UX | PLATFORM_RECOMMENDATION | Search Console, SERP observation | PARTIAL | NOT_SUITABLE_FOR_SCORING | HIGH | S014 |
| M055 | C18 | Structured data syntax validity | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether structured data parses and uses recognized vocabulary/types. | Parse JSON-LD/Microdata/RDFa and validate vocabulary. | NOT_APPLICABLE | status | CRAWL | PAGE | Syntax validity does not guarantee rich-result eligibility or appearance. | SEO, AI_VISIBILITY | TECHNICAL_DEPENDENCY | Schema validator, Rich Results Test | FULL | DIAGNOSTIC_ONLY | HIGH | S011 |
| M056 | C18 | Rich-result eligibility diagnostics | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether markup satisfies documented requirements for a supported rich-result type. | Validate against current Search documentation and required/recommended properties. | NOT_APPLICABLE | status | HYBRID | PAGE | Eligibility never guarantees display. | SEO | PLATFORM_RECOMMENDATION | Rich Results Test | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S012 |
| M057 | C19 | Machine-readable entity identifier coverage | PROXY | E6_PLAUSIBLE_PROXY | Presence of stable identifiers and consistent entity references in structured/semantic markup. | Extract sameAs/URL/IDs/organization/person identifiers and test consistency. | NOT_APPLICABLE | coverage | CRAWL | SITE | No standard evidence that higher coverage directly raises AI citations/rankings. | AI_VISIBILITY, SEO | PLAUSIBLE_INDIRECT_RELATION | crawler, Schema parser | PARTIAL | DIAGNOSTIC_ONLY | LOW | S011 |
| M058 | C19 | Entity consistency across page signals | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Agreement among names, URLs, structured data, headings and metadata for a represented entity. | Normalize extracted entity references and compare contradictions. | NOT_APPLICABLE | status | HYBRID | ENTITY | No universal threshold or ranking-factor status. | AI_VISIBILITY, SEO | PLAUSIBLE_INDIRECT_RELATION | semantic parser, LLM review | PARTIAL | DIAGNOSTIC_ONLY | LOW | S011 |
| M059 | C20 | Content helpfulness evidence review | QUALITATIVE_REVIEW | E2_PLATFORM_OFFICIAL | Structured review of whether content appears created primarily to help users and demonstrates first-hand usefulness where relevant. | Apply documented Search guidance using human review and evidence pointers. | NOT_APPLICABLE | review | MANUAL | PAGE | No public universal formula; E-E-A-T is not a single numeric ranking factor. | SEO, BUSINESS, UX | PLATFORM_RECOMMENDATION | review rubric | MANUAL | NOT_SUITABLE_FOR_SCORING | HIGH | S015 |
| M060 | C20 | Content freshness status | PROXY | E6_PLAUSIBLE_PROXY | Whether time-sensitive content is current enough for its subject and user task. | Compare publication/update evidence against domain-specific change rate and current facts. | NOT_APPLICABLE | status | HYBRID | PAGE | No universal freshness interval. | SEO, UX, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | crawler, web verification | PARTIAL | DIAGNOSTIC_ONLY | LOW | S015 |
| M061 | C21 | Query-content alignment | QUALITATIVE_REVIEW | E6_PLAUSIBLE_PROXY | Degree to which page content answers the observed query/user task. | Map Search Console queries or research set to page propositions and missing intent facets. | NOT_APPLICABLE | review | HYBRID | QUERY | No universal score or causal ranking claim. | SEO, UX, CONVERSION | PLAUSIBLE_INDIRECT_RELATION | Search Console, manual/semantic review | PARTIAL | NOT_SUITABLE_FOR_SCORING | LOW | S003 |
| M062 | C22 | Topic coverage gap | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Material subtopics/questions expected by the target task but absent from the page/site. | Build evidence-based topic set from user/search data and compare page/site coverage. | NOT_APPLICABLE | gap set | HYBRID | SITE | No universal information-gain formula for audits. | SEO, UX, AI_VISIBILITY | PLAUSIBLE_INDIRECT_RELATION | Search Console, content corpus, semantic analysis | PARTIAL | DIAGNOSTIC_ONLY | LOW | S015 |
| M063 | C23 | Exact duplicate content cluster count | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Groups of URLs with identical normalized main content. | Hash normalized content/body after excluding known boilerplate. | NOT_APPLICABLE | count | CRAWL | SITE | No universal threshold; duplicates can be legitimate. | INDEXING, CRAWLING | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | MEDIUM | S007 |
| M064 | C23 | Near-duplicate similarity | PROXY | E6_PLAUSIBLE_PROXY | Similarity between page bodies after normalization. | Compute shingles/embeddings/simhash with declared method and threshold. | NOT_APPLICABLE | similarity | CRAWL | SITE | Threshold is algorithm/product-specific; not a search-engine standard. | INDEXING, SEO | PLAUSIBLE_INDIRECT_RELATION | crawler, similarity model | FULL | DIAGNOSTIC_ONLY | LOW | S007 |
| M065 | C24 | Information architecture depth distribution | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Distribution of shortest internal-navigation depth from selected entry points. | Build directed internal-link graph and shortest paths. | NOT_APPLICABLE | clicks | CRAWL | SITE | No universal three-click rule. | UX, CRAWLING, SEO | PLAUSIBLE_INDIRECT_RELATION | crawler, graph analysis | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M066 | C25 | Internal inlink count | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Number of in-scope internal links pointing to a URL. | Build deduplicated internal link graph. | NOT_APPLICABLE | count | CRAWL | PAGE | More is not automatically better; position/context matter. | CRAWLING, SEO, UX | PLAUSIBLE_INDIRECT_RELATION | crawler | FULL | DIAGNOSTIC_ONLY | MEDIUM | S015 |
| M067 | C25 | Broken internal link count | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Internal links resolving to broken/error destinations under audit conditions. | Crawl link targets and classify response/error. | NOT_APPLICABLE | count | CRAWL | SITE | Zero unintended broken links is a practical target. | UX, CRAWLING, RELIABILITY | TECHNICAL_DEPENDENCY | crawler | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S020 |
| M068 | C26 | Navigation task path length | METRIC | E3_RESEARCH_VALIDATED | Steps required for representative users to reach a defined target through the interface. | Run task-based usability test or instrumented path analysis. | NOT_APPLICABLE | steps | MANUAL | SESSION | No universal target; task complexity matters. | UX, CONVERSION | EMPIRICAL_ASSOCIATION | usability test, analytics | MANUAL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S040 |
| M069 | C27 | Referring domain count | METRIC | E5_VENDOR_SPECIFIC | Count of distinct linking domains observed by a backlink provider or owned log/index. | Query provider backlink index under a declared freshness scope. | NOT_APPLICABLE | count | THIRD_PARTY | DOMAIN | Provider indexes differ; cross-tool values are not directly interchangeable. | SEO, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | Ahrefs, Semrush | EXTERNAL_API | DIAGNOSTIC_ONLY | MEDIUM | S033 |
| M070 | C27 | Domain Rating / Authority Score | COMPOSITE_SCORE | E5_VENDOR_SPECIFIC | Vendor-specific composite or relative authority estimate derived from backlink/traffic/spam signals. | Use exact vendor methodology and version; never normalize as a search-engine metric. | NOT_APPLICABLE | 0-100 | THIRD_PARTY | DOMAIN | No universal official good/bad threshold; vendor-relative only. | SEO, BUSINESS | PRACTITIONER_HYPOTHESIS | Ahrefs DR, Semrush Authority Score | EXTERNAL_API | NOT_SUITABLE_FOR_SCORING | MEDIUM | S033 |
| M071 | C28 | Google Search impressions | METRIC | E2_PLATFORM_OFFICIAL | Search Console count of eligible appearances of site links/content in Google surfaces under documented rules. | Query Search Console Performance report/API. | NOT_APPLICABLE | count | SEARCH_PLATFORM | QUERY | No universal higher-is-better target; query mix and meaningfulness matter. | SEO, BUSINESS | TECHNICAL_DEPENDENCY | Search Console API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S003 |
| M072 | C28 | Google Search clicks | METRIC | E2_PLATFORM_OFFICIAL | Count of Search Console-recorded clicks from Google to the site under documented rules. | Query Search Console. | NOT_APPLICABLE | count | SEARCH_PLATFORM | QUERY | No universal threshold. | SEO, BUSINESS | TECHNICAL_DEPENDENCY | Search Console API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S003 |
| M073 | C28 | Google Search CTR | KPI | E2_PLATFORM_OFFICIAL | Clicks divided by impressions for the selected Search Console scope. | Query clicks/impressions and compute or use Search Console CTR. | clicks / impressions * 100 | % | SEARCH_PLATFORM | QUERY | No universal CTR benchmark; result type, position, brand and query intent confound. | SEO, BUSINESS | EMPIRICAL_ASSOCIATION | Search Console API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S003 |
| M074 | C28 | Google average position | METRIC | E2_PLATFORM_OFFICIAL | Average of the topmost position occupied by the property/page for recorded impressions. | Use Search Console Performance metric with query/result-type context. | NOT_APPLICABLE | position | SEARCH_PLATFORM | QUERY | No universal direct cross-query benchmark; complex and potentially misleading. | SEO | EMPIRICAL_ASSOCIATION | Search Console API | EXTERNAL_API | DIAGNOSTIC_ONLY | HIGH | S003 |
| M075 | C29 | hreflang cluster validity | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether alternate-language/region annotations form valid reciprocal clusters for audited URLs. | Parse hreflang annotations, validate language/region codes, return links and canonical relationships. | NOT_APPLICABLE | status | CRAWL | SITE | No universal score; correctness is cluster-specific. | SEO, UX | TECHNICAL_DEPENDENCY | crawler | FULL | DIAGNOSTIC_ONLY | HIGH | S015 |
| M076 | C29 | Localization content parity review | QUALITATIVE_REVIEW | E6_PLAUSIBLE_PROXY | Whether localized pages preserve intended purpose while adapting language, offers and regulatory context appropriately. | Compare localized page sets with human/semantic review. | NOT_APPLICABLE | review | MANUAL | SITE | No universal parity target. | UX, SEO, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | review rubric | MANUAL | NOT_SUITABLE_FOR_SCORING | LOW | S015 |
| M077 | C30 | Local relevance completeness | QUALITATIVE_REVIEW | E2_PLATFORM_OFFICIAL | Completeness/consistency of business information relevant to local search relevance. | Review business profile/site location/service information and query relevance. | NOT_APPLICABLE | review | HYBRID | ENTITY | No universal score; relevance, distance and prominence are distinct factors. | SEO, BUSINESS | PLATFORM_RECOMMENDATION | Google Business Profile, site review | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S016 |
| M078 | C30 | NAP consistency | PROXY | E7_PRACTITIONER_HEURISTIC | Consistency of name/address/phone representations across owned and sampled external sources. | Normalize and compare identifiers across sampled sources. | NOT_APPLICABLE | % | THIRD_PARTY | ENTITY | Sampling-dependent practitioner proxy; not a Google-defined KPI. | SEO, BUSINESS | PRACTITIONER_HYPOTHESIS | crawler, directory APIs | PARTIAL | DIAGNOSTIC_ONLY | LOW | SOURCE_NEEDED |
| M079 | C31 | Image alt-text coverage | PROXY | E1_STANDARDIZED | Share of content images with appropriate text alternatives or correct decorative treatment. | Parse img/role attributes and inspect context; human review determines appropriateness. | NOT_APPLICABLE | % | HYBRID | SITE | No universal percentage threshold; decorative images may correctly have empty alt. | ACCESSIBILITY, SEO, UX | TECHNICAL_DEPENDENCY | crawler, accessibility engine | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S017 |
| M080 | C31 | Image discoverability status | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether important images are represented in crawlable HTML and can be discovered/indexed under current guidance. | Render/crawl DOM, inspect img/src/srcset, robots and optional image sitemap. | NOT_APPLICABLE | status | HYBRID | RESOURCE | Eligibility/discoverability does not guarantee image ranking. | SEO, CRAWLING | PLATFORM_RECOMMENDATION | browser crawler | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S015 |
| M081 | C32 | Video page eligibility signals | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Presence of crawlable video, stable thumbnail and metadata needed for supported video search features. | Render page, inspect video embedding, thumbnails, structured metadata and indexing controls. | NOT_APPLICABLE | status | HYBRID | PAGE | Eligibility does not guarantee video result appearance. | SEO | PLATFORM_RECOMMENDATION | browser crawler, structured-data validator | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S015 |
| M082 | C32 | Video transcript/caption availability | DIAGNOSTIC_SIGNAL | E6_PLAUSIBLE_PROXY | Whether meaningful video content has accessible captions/transcript usable by people and machines. | Inspect media tracks, captions and page transcript. | NOT_APPLICABLE | status | HYBRID | RESOURCE | Does not prove video ranking or AI citation. | ACCESSIBILITY, SEO, AI_VISIBILITY | PLAUSIBLE_INDIRECT_RELATION | browser, manual review | PARTIAL | DIAGNOSTIC_ONLY | LOW | S017 |
| M083 | C33 | GEO experimental visibility score | PROXY | E3_RESEARCH_VALIDATED | Experimental visibility measure used in a defined generative-engine evaluation corpus. | Run fixed prompt/query set and compute the published experiment-specific visibility formulation. | NOT_APPLICABLE | experiment-specific | THIRD_PARTY | QUERY | Only valid within declared experimental setup; not a universal GEO KPI. | GEO, AI_VISIBILITY | EMPIRICAL_ASSOCIATION | research harness | PARTIAL | NOT_SUITABLE_FOR_SCORING | MEDIUM | S031 |
| M084 | C33 | AI-query coverage | PROXY | E6_PLAUSIBLE_PROXY | Share of a declared prompt/query panel for which the audited entity/source appears in an AI answer/search surface. | Define representative prompt panel, repeat runs, record inclusion and uncertainty. | NOT_APPLICABLE | % | THIRD_PARTY | QUERY | No cross-platform standard; sample design and run count dominate interpretation. | GEO, AI_VISIBILITY | PLAUSIBLE_INDIRECT_RELATION | AI visibility harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S028 |
| M085 | C34 | Google generative-AI impressions | METRIC | E2_PLATFORM_OFFICIAL | First-party Search Console impressions attributable to supported generative AI Search reporting surfaces. | Use Search Console generative-AI performance report where available for property. | NOT_APPLICABLE | count | SEARCH_PLATFORM | QUERY | No universal benchmark; reporting availability/scope can evolve. | AI_VISIBILITY, SEO | TECHNICAL_DEPENDENCY | Search Console | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S028 |
| M086 | C34 | Google generative-AI clicks | METRIC | E2_PLATFORM_OFFICIAL | First-party clicks from supported generative AI Search reporting surfaces. | Use Search Console generative-AI performance report. | NOT_APPLICABLE | count | SEARCH_PLATFORM | QUERY | No universal benchmark. | AI_VISIBILITY, BUSINESS | TECHNICAL_DEPENDENCY | Search Console | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S028 |
| M087 | C34 | Vendor AI Share of Voice | COMPOSITE_SCORE | E5_VENDOR_SPECIFIC | Vendor-defined relative share of AI visibility/mentions within a configured competitor and prompt set. | Use vendor prompt database/competitor configuration and exact documented formula. | NOT_APPLICABLE | % | THIRD_PARTY | ENTITY | Vendor- and configuration-specific; not cross-platform comparable by default. | AI_VISIBILITY, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | Ahrefs Brand Radar, Semrush AI Visibility | EXTERNAL_API | NOT_SUITABLE_FOR_SCORING | MEDIUM | S032 |
| M088 | C34 | AI answer inclusion rate | PROXY | E6_PLAUSIBLE_PROXY | Fraction of repeated sampled AI responses in which a target entity/domain appears. | Run repeated prompt panel per model/time window and record inclusion. | NOT_APPLICABLE | % | THIRD_PARTY | QUERY | No standardized sample size or universal threshold. | AI_VISIBILITY | PLAUSIBLE_INDIRECT_RELATION | custom harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S031 |
| M089 | C35 | AI citation rate | PROXY | E6_PLAUSIBLE_PROXY | Fraction of sampled AI answers that explicitly cite or link the audited source. | Run repeated query panel; capture explicit source citations/links by platform. | NOT_APPLICABLE | % | THIRD_PARTY | QUERY | Citation semantics differ by platform and prompt; not directly comparable across systems. | AI_VISIBILITY, GEO | PLAUSIBLE_INDIRECT_RELATION | AI visibility harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S030 |
| M090 | C35 | AI mention rate | PROXY | E6_PLAUSIBLE_PROXY | Fraction of sampled answers mentioning a target brand/entity regardless of citation. | Repeated prompt sampling and entity recognition. | NOT_APPLICABLE | % | THIRD_PARTY | ENTITY | Mention != citation, recommendation, correctness or positive sentiment. | AI_VISIBILITY, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | AI visibility harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S032 |
| M091 | C35 | ChatGPT referral sessions | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Analytics sessions attributed to ChatGPT referral traffic using referrer/campaign data such as documented utm_source tagging. | Query analytics acquisition data with transparent attribution rules. | NOT_APPLICABLE | sessions | ANALYTICS | SESSION | Attribution can be incomplete and does not measure unclicked citations/mentions. | AI_VISIBILITY, BUSINESS | TECHNICAL_DEPENDENCY | GA4, analytics warehouse | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S030 |
| M092 | C36 | OAI-SearchBot crawl permission | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether robots policy permits OAI-SearchBot access to the audited paths. | Evaluate RFC-compatible robots rules for OAI-SearchBot. | NOT_APPLICABLE | status | CRAWL | URL | Allowing crawl does not guarantee ChatGPT inclusion/citation. | AI_VISIBILITY, CRAWLING | TECHNICAL_DEPENDENCY | robots parser | FULL | DIAGNOSTIC_ONLY | HIGH | S006 |
| M093 | C36 | Googlebot crawl permission | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether robots policy permits Googlebot access to audited paths. | Evaluate robots rules for Googlebot. | NOT_APPLICABLE | status | CRAWL | URL | Crawl permission does not guarantee indexing. | CRAWLING, INDEXING, AI_VISIBILITY | TECHNICAL_DEPENDENCY | robots parser | FULL | DIAGNOSTIC_ONLY | HIGH | S006 |
| M094 | C36 | AI crawler policy matrix | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Declared access policy across selected AI/search crawler user agents. | Create explicit user-agent list from official docs; evaluate robots rules per path and record unknowns/conflicts. | NOT_APPLICABLE | matrix | CRAWL | SITE | Crawler identities and product purposes differ; do not infer one bot from another. | AI_VISIBILITY, CRAWLING | TECHNICAL_DEPENDENCY | robots parser | FULL | DIAGNOSTIC_ONLY | LOW | S006 |
| M095 | C37 | Passage answerability review | QUALITATIVE_REVIEW | E6_PLAUSIBLE_PROXY | Whether a passage can answer a target question clearly with sufficient local context and sourceable facts. | Map target questions to passages; expert/semantic review for explicit answer, context, qualifiers and evidence. | NOT_APPLICABLE | review | MANUAL | PAGE | No standardized passage-retrievability KPI or threshold. | AI_VISIBILITY, UX, SEO | PLAUSIBLE_INDIRECT_RELATION | semantic review | MANUAL | NOT_SUITABLE_FOR_SCORING | LOW | S029 |
| M096 | C37 | Heading-to-passage structure | PROXY | E6_PLAUSIBLE_PROXY | Degree to which major content passages are organized under descriptive semantic headings. | Parse heading/content hierarchy and inspect descriptive alignment. | NOT_APPLICABLE | coverage | HYBRID | PAGE | Does not prove retrieval, ranking or citation. | AI_VISIBILITY, ACCESSIBILITY, UX | PLAUSIBLE_INDIRECT_RELATION | crawler, semantic review | PARTIAL | DIAGNOSTIC_ONLY | LOW | S010 |
| M097 | C38 | AI entity representation consistency | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Consistency of factual brand/entity attributes across repeated AI answers. | Define factual attribute set; sample repeated model outputs; compare omissions/contradictions to verified facts. | NOT_APPLICABLE | agreement | THIRD_PARTY | ENTITY | Model-dependent and time-dependent; cannot be treated as ground truth. | AI_VISIBILITY, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | AI sampling harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S032 |
| M098 | C38 | AI attribution accuracy | QUALITATIVE_REVIEW | E6_PLAUSIBLE_PROXY | Correctness of claims attributed to an audited brand/entity in AI answers. | Compare sampled claims against first-party/verified sources and classify supported/unsupported/incorrect. | NOT_APPLICABLE | review | HYBRID | ENTITY | No universal score; answer systems may vary per run. | AI_VISIBILITY, BUSINESS | TECHNICAL_DEPENDENCY | AI sampling harness, source verification | PARTIAL | DIAGNOSTIC_ONLY | LOW | S030 |
| M099 | C39 | WCAG 2.2 success-criterion conformance | STANDARD_OR_REQUIREMENT | E1_STANDARDIZED | Per-success-criterion conformance assessment against WCAG 2.2 for declared level/scope. | Combine automated checks, manual inspection and user-oriented tests; record criterion evidence. | NOT_APPLICABLE | status | HYBRID | SITE | Conformance cannot be determined by automated tools alone. | ACCESSIBILITY, UX, BUSINESS | TECHNICAL_DEPENDENCY | axe, manual review, WCAG-EM | PARTIAL | NOT_SUITABLE_FOR_SCORING | HIGH | S017 |
| M100 | C39 | Target Size (Minimum) compliance | STANDARD_OR_REQUIREMENT | E1_STANDARDIZED | Conformance with WCAG 2.2 SC 2.5.8 minimum target-size/spacing conditions. | Measure CSS-pixel target bounds and exceptions/spacing. | NOT_APPLICABLE | status | HYBRID | PAGE | 24x24 CSS px minimum target or applicable spacing/exception conditions for AA. | ACCESSIBILITY, UX | TECHNICAL_DEPENDENCY | browser, accessibility review | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S017 |
| M101 | C39 | Automated accessibility issue count | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Count of issues detected by a declared automated accessibility rule set. | Run fixed engine/version and rule set. | NOT_APPLICABLE | count | LAB | PAGE | Tool-specific; zero automated issues does not prove WCAG conformance. | ACCESSIBILITY | TECHNICAL_DEPENDENCY | axe, Lighthouse accessibility | FULL | DIAGNOSTIC_ONLY | MEDIUM | S018 |
| M102 | C40 | Task completion rate | KPI | E3_RESEARCH_VALIDATED | Share of representative users who complete a defined task under stated success criteria. | Moderated/unmoderated usability test with representative participants and binary task success. | successful_users / attempted_users * 100 | % | MANUAL | USER | Benchmark is task/product-specific. | UX, CONVERSION, BUSINESS | EMPIRICAL_ASSOCIATION | usability study | MANUAL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S040 |
| M103 | C40 | Time on task | METRIC | E3_RESEARCH_VALIDATED | Elapsed time for representative users to complete a defined task. | Usability test instrumentation. | NOT_APPLICABLE | s | MANUAL | USER | Compare only like tasks and populations. | UX, CONVERSION | EMPIRICAL_ASSOCIATION | usability study | MANUAL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S040 |
| M104 | C40 | Usability heuristic review | HEURISTIC | E7_PRACTITIONER_HEURISTIC | Expert review against a named heuristic set such as Nielsen heuristics. | Expert inspection with issue evidence, severity and rationale. | NOT_APPLICABLE | review | MANUAL | PAGE | Heuristics are rules of thumb, not validated universal numeric KPIs. | UX | PRACTITIONER_HYPOTHESIS | expert review | MANUAL | NOT_SUITABLE_FOR_SCORING | LOW | S041 |
| M105 | C41 | HTTPS availability | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Whether audited site paths are available over authenticated HTTPS without certificate/protocol failure. | Connect with standards-capable TLS client, validate certificate chain/hostname and HTTP response. | NOT_APPLICABLE | status | SYNTHETIC | DOMAIN | Binary availability is not a complete security audit. | SECURITY, RELIABILITY, UX | TECHNICAL_DEPENDENCY | browser, openssl | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S022 |
| M106 | C41 | Mixed content incidence | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | HTTPS pages that load or request insecure subresources under browser mixed-content rules. | Render in browser and inspect security/network events. | NOT_APPLICABLE | count | LAB | PAGE | Zero unintended active mixed content is a practical target. | SECURITY, UX | TECHNICAL_DEPENDENCY | browser devtools | FULL | DIAGNOSTIC_ONLY | HIGH | S022 |
| M107 | C41 | Security-header configuration review | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Presence/configuration of browser security response headers relevant to site threat model. | Inspect headers and evaluate against current standard/browser semantics and application context. | NOT_APPLICABLE | status | CRAWL | PAGE | No one header score proves site security. | SECURITY | TECHNICAL_DEPENDENCY | curl, securityheaders | FULL | DIAGNOSTIC_ONLY | MEDIUM | S020 |
| M108 | C42 | Consent prior to non-essential storage/tracking | STANDARD_OR_REQUIREMENT | E1_STANDARDIZED | Whether non-essential cookies/tracking requiring consent are withheld until valid user choice in applicable scope. | Instrument clean browser, observe storage/network before/after consent; map purposes/legal scope. | NOT_APPLICABLE | status | LAB | SESSION | Jurisdiction and purpose matter; legal advice/expert review may be required. | PRIVACY, BUSINESS | TECHNICAL_DEPENDENCY | browser automation, network capture | PARTIAL | NOT_SUITABLE_FOR_SCORING | HIGH | S043 |
| M109 | C42 | GPC signal handling | DIAGNOSTIC_SIGNAL | E1_STANDARDIZED | Observed handling of Global Privacy Control signal where applicable. | Send Sec-GPC / navigator signal in controlled browser and compare tracking/response behavior. | NOT_APPLICABLE | status | LAB | SESSION | W3C GPC is a Working Draft; legal obligations vary. | PRIVACY | TECHNICAL_DEPENDENCY | browser automation | PARTIAL | DIAGNOSTIC_ONLY | HIGH | S042 |
| M110 | C42 | Tracker/cookie inventory | ANALYSIS_METHOD | E4_REPRODUCIBLE_INDUSTRY_METRIC | Observed first- and third-party storage/network endpoints under defined consent states. | Automated browser crawl with storage/network capture and domain/entity classification. | NOT_APPLICABLE | inventory | LAB | SITE | Detection is not a legal classification by itself. | PRIVACY, SECURITY, PERFORMANCE | TECHNICAL_DEPENDENCY | browser automation, tracker classifier | FULL | DIAGNOSTIC_ONLY | MEDIUM | S036 |
| M111 | C43 | Analytics event schema validity | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Whether observed analytics events match the documented measurement plan and required parameters. | Capture events or query analytics/warehouse; compare to versioned schema. | NOT_APPLICABLE | % | ANALYTICS | SITE | Target is implementation-specific. | BUSINESS, RELIABILITY | TECHNICAL_DEPENDENCY | GA4, data warehouse, tag debugger | PARTIAL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S025 |
| M112 | C43 | Analytics thresholding status | DIAGNOSTIC_SIGNAL | E2_PLATFORM_OFFICIAL | Whether privacy/data thresholds affect the displayed GA report. | Inspect GA data-quality indicators/metadata and compare reports where supported. | NOT_APPLICABLE | status | ANALYTICS | SITE | Thresholding can hide data; absence/presence is not site quality. | BUSINESS | TECHNICAL_DEPENDENCY | GA4 | EXTERNAL_API | DIAGNOSTIC_ONLY | HIGH | S027 |
| M113 | C43 | Measurement-plan coverage | PROXY | E6_PLAUSIBLE_PROXY | Share of explicitly required product/business events and properties observed and validated. | Compare versioned measurement plan to implementation and collected data. | NOT_APPLICABLE | % | HYBRID | SITE | Product-defined; no universal threshold. | BUSINESS, CONVERSION | TECHNICAL_DEPENDENCY | tag manager, analytics, warehouse | PARTIAL | SCORE_ELIGIBLE_WITH_CONTEXT | LOW | S025 |
| M114 | C44 | GA4 engagement rate | KPI | E2_PLATFORM_OFFICIAL | Percentage of sessions that qualify as engaged sessions under GA4 definitions. | Use GA4 engaged sessions / sessions. | engaged_sessions / sessions * 100 | % | ANALYTICS | SESSION | No universal good rate; depends on site/task/channel and GA configuration. | BUSINESS, UX | EMPIRICAL_ASSOCIATION | GA4 Data API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S026 |
| M115 | C44 | GA4 bounce rate | KPI | E2_PLATFORM_OFFICIAL | Percentage of sessions that are not engaged sessions in GA4. | Use GA4 bounce rate; inverse concept to engagement rate. | NOT_APPLICABLE | % | ANALYTICS | SESSION | No universal good rate; GA4 definition differs from legacy analytics concepts. | BUSINESS, UX | EMPIRICAL_ASSOCIATION | GA4 Data API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S026 |
| M116 | C44 | Key-event conversion rate | KPI | E2_PLATFORM_OFFICIAL | Share of relevant sessions/users triggering configured key events under selected GA4 scope. | Query configured key events and denominator matching business question. | NOT_APPLICABLE | % | ANALYTICS | SESSION | Configuration-specific; not comparable across sites without aligned definitions. | CONVERSION, BUSINESS | TECHNICAL_DEPENDENCY | GA4 Data API | EXTERNAL_API | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S025 |
| M117 | C45 | Verified search-bot request share | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Share of server requests attributable to verified search crawlers. | Parse server logs; verify crawler IP/host using official mechanisms where available. | NOT_APPLICABLE | % | SERVER | SITE | No universal target; crawl demand depends on site and engine. | CRAWLING, SEO | TECHNICAL_DEPENDENCY | log analyzer | FULL | DIAGNOSTIC_ONLY | MEDIUM | S044 |
| M118 | C45 | Bot status-code distribution | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | HTTP response distribution observed specifically for verified crawler traffic. | Aggregate verified crawler log requests by status class/URL pattern. | NOT_APPLICABLE | % | SERVER | SITE | Interpret against intended crawl paths and change events. | CRAWLING, RELIABILITY | TECHNICAL_DEPENDENCY | log analyzer | FULL | DIAGNOSTIC_ONLY | MEDIUM | S020 |
| M119 | C45 | Bot crawl waste proxy | PROXY | E6_PLAUSIBLE_PROXY | Share of verified crawler requests spent on duplicate, parameterized, redirected or intentionally non-indexable URL patterns. | Classify bot log requests by URL outcome and intended indexability. | NOT_APPLICABLE | % | SERVER | SITE | No official crawl-waste percentage threshold. | CRAWLING, SEO | PLAUSIBLE_INDIRECT_RELATION | log analyzer, crawler | PARTIAL | DIAGNOSTIC_ONLY | LOW | S044 |
| M120 | C46 | Availability SLI | KPI | E4_REPRODUCIBLE_INDUSTRY_METRIC | Fraction of valid requests/time windows meeting defined successful-service condition. | Define valid events and success criteria, then compute good/valid ratio. | good_events / valid_events * 100 | % | SERVER | SITE | SLO target is product/business-specific; do not impose universal nines. | RELIABILITY, BUSINESS | TECHNICAL_DEPENDENCY | monitoring, synthetic probes | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S024 |
| M121 | C46 | Latency percentile SLI | KPI | E4_REPRODUCIBLE_INDUSTRY_METRIC | Selected percentile of service latency for a defined request population. | Collect latency histogram/distribution; compute p50/p95/p99 as decision requires. | NOT_APPLICABLE | ms | SERVER | SERVER | Percentile and target are service-specific. | RELIABILITY, PERFORMANCE | TECHNICAL_DEPENDENCY | monitoring, OpenTelemetry | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S024 |
| M122 | C47 | Redirect chain length | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Number of redirect hops from requested URL to terminal response. | Follow redirects with declared maximum; count hops and loops. | NOT_APPLICABLE | hops | CRAWL | URL | Zero/one is often preferable but no universal standard threshold. | PERFORMANCE, CRAWLING, UX | TECHNICAL_DEPENDENCY | crawler, curl | FULL | DIAGNOSTIC_ONLY | MEDIUM | S020 |
| M123 | C47 | 4xx/5xx URL incidence | METRIC | E1_STANDARDIZED | Share/count of crawled URL requests ending in client/server error status classes. | Crawl target set; classify RFC-defined response classes. | NOT_APPLICABLE | % | CRAWL | SITE | Intentional 404/410 can be correct; scope interpretation required. | RELIABILITY, CRAWLING, UX | TECHNICAL_DEPENDENCY | crawler | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | HIGH | S020 |
| M124 | C48 | Technology inventory | ANALYSIS_METHOD | E4_REPRODUCIBLE_INDUSTRY_METRIC | Observed frameworks, servers, CMS, libraries and service dependencies detectable from public/runtime signals. | Combine headers, DOM/scripts, asset signatures and optional repository/owner data. | NOT_APPLICABLE | inventory | HYBRID | SITE | Detection may be incomplete or false-positive; public evidence is not architecture truth. | RELIABILITY, SECURITY, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | Wappalyzer-like detector, crawler | FULL | DIAGNOSTIC_ONLY | MEDIUM | S035 |
| M125 | C48 | Client-side rendering dependency | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Extent to which meaningful page content/links require JavaScript execution. | Compare raw HTTP HTML to rendered DOM and content/link inventory. | NOT_APPLICABLE | delta | HYBRID | PAGE | JS dependence is not inherently bad; evaluate crawler/user compatibility. | CRAWLING, AI_VISIBILITY, PERFORMANCE | TECHNICAL_DEPENDENCY | crawler, headless browser | FULL | DIAGNOSTIC_ONLY | MEDIUM | S029 |
| M126 | C49 | Performance budget breach count | KPI | E6_PLAUSIBLE_PROXY | Number of versioned product-defined performance budgets exceeded in a build/run. | Compare measured metrics/resource sizes to repository budget configuration. | NOT_APPLICABLE | count | LAB | PAGE | Budgets are product decisions unless a source-specific threshold is adopted. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | Lighthouse CI, WebPageTest | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | LOW | S001 |
| M127 | C49 | Performance regression delta | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Change in a stable metric between baseline and candidate under comparable conditions. | Run controlled repeated tests or compare aligned field windows; compute delta/confidence. | NOT_APPLICABLE | delta | HYBRID | PAGE | Regression threshold is product-specific and must account for variance. | PERFORMANCE, RELIABILITY | TECHNICAL_DEPENDENCY | CI, RUM | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S001 |
| M128 | C50 | Peer percentile benchmark | PROXY | E4_REPRODUCIBLE_INDUSTRY_METRIC | Position of a site metric in a declared comparable peer/reference distribution. | Select peer cohort and same measurement definition; compute percentile. | NOT_APPLICABLE | percentile | THIRD_PARTY | SITE | Only valid if cohort and measurement conditions are comparable. | BUSINESS, PERFORMANCE, SEO | EMPIRICAL_ASSOCIATION | HTTP Archive, benchmark dataset | PARTIAL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S035 |
| M129 | C50 | Competitive feature/content gap | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Audited differences in capabilities/content coverage versus a declared competitor set. | Define comparison rubric, collect same evidence for each site, separate observation from recommendation. | NOT_APPLICABLE | gap set | HYBRID | SITE | Competitor presence does not prove user value or causality. | BUSINESS, UX, SEO | PLAUSIBLE_INDIRECT_RELATION | crawler, manual review | PARTIAL | DIAGNOSTIC_ONLY | LOW | S035 |
| M130 | C51 | Baseline feature status | STANDARD_OR_REQUIREMENT | E2_PLATFORM_OFFICIAL | Web-platform feature availability status across core browsers using Baseline. | Map used features/APIs to current Baseline status. | NOT_APPLICABLE | status | THIRD_PARTY | RESOURCE | Baseline availability is compatibility evidence, not proof of correct implementation. | UX, RELIABILITY | TECHNICAL_DEPENDENCY | web-features/Baseline data | FULL | DIAGNOSTIC_ONLY | HIGH | S037 |
| M131 | C51 | Unsupported-browser error incidence | DIAGNOSTIC_SIGNAL | E4_REPRODUCIBLE_INDUSTRY_METRIC | Observed functional/render errors across explicitly supported browser/device matrix. | Run cross-browser functional/visual checks on representative flows. | NOT_APPLICABLE | count | LAB | SITE | Support matrix is product-defined. | UX, RELIABILITY, BUSINESS | TECHNICAL_DEPENDENCY | Playwright, BrowserStack | FULL | SCORE_ELIGIBLE_WITH_CONTEXT | MEDIUM | S037 |
| M132 | C52 | Third-party request count | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Number of network requests to organizationally external third parties in a defined page load. | Capture network requests and classify registrable domains/entities. | NOT_APPLICABLE | count | LAB | PAGE | Lower is not always better; functional value/context matters. | PERFORMANCE, PRIVACY, SECURITY | TECHNICAL_DEPENDENCY | HTTP Archive, WebPageTest | FULL | DIAGNOSTIC_ONLY | MEDIUM | S036 |
| M133 | C52 | Third-party transfer bytes | METRIC | E4_REPRODUCIBLE_INDUSTRY_METRIC | Transferred bytes attributable to third-party resources. | Classify network requests by party and sum transfer sizes. | NOT_APPLICABLE | bytes | LAB | PAGE | No universal threshold. | PERFORMANCE, PRIVACY, SUSTAINABILITY | TECHNICAL_DEPENDENCY | WebPageTest, browser | FULL | DIAGNOSTIC_ONLY | MEDIUM | S036 |
| M134 | C52 | Third-party dependency criticality review | ANALYSIS_METHOD | E6_PLAUSIBLE_PROXY | Business/runtime criticality and failure blast radius of external website dependencies. | Inventory dependency, purpose, failure mode, data access, fallback and owner. | NOT_APPLICABLE | review | HYBRID | SITE | No universal composite score; supply-chain risk is context-specific. | RELIABILITY, SECURITY, PRIVACY, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | network capture, architecture review | PARTIAL | NOT_SUITABLE_FOR_SCORING | LOW | S036 |
| M135 | C53 | Transferred bytes per task/page | PROXY | E6_PLAUSIBLE_PROXY | Network data transferred for a defined page or user task as a resource-efficiency proxy. | Measure comparable page/task loads with cache state declared. | NOT_APPLICABLE | bytes | LAB | PAGE | Sustainability impact is indirect; WSG is draft and no universal carbon conversion is asserted. | SUSTAINABILITY, PERFORMANCE | PLAUSIBLE_INDIRECT_RELATION | WebPageTest, browser | FULL | DIAGNOSTIC_ONLY | LOW | S038 |
| M136 | C53 | Sustainability guideline review | QUALITATIVE_REVIEW | E8_UNCLEAR_OR_UNVALIDATED | Structured review against current W3C Web Sustainability Guidelines draft. | Map evidence to draft guidelines and clearly mark draft status/impact ratings. | NOT_APPLICABLE | review | MANUAL | SITE | Draft guidance; not a stable conformance standard or certification. | SUSTAINABILITY, BUSINESS | PRACTITIONER_HYPOTHESIS | expert review | MANUAL | NOT_SUITABLE_FOR_SCORING | LOW | S038 |
| M137 | C54 | Agent-accessible interaction success | PROXY | E8_UNCLEAR_OR_UNVALIDATED | Success of declared browser-agent tasks using accessible semantic interaction surfaces. | Run deterministic task scripts with a declared browser agent/runtime and record success/failure plus fallback. | NOT_APPLICABLE | % | LAB | SESSION | Emerging capability; model/runtime specific and not standardized as a universal website KPI. | AI_VISIBILITY, UX, BUSINESS | PLAUSIBLE_INDIRECT_RELATION | browser agent harness | PARTIAL | NOT_SUITABLE_FOR_SCORING | LOW | S039 |
| M138 | C54 | Semantic action discoverability | PROXY | E8_UNCLEAR_OR_UNVALIDATED | Whether important actions expose labels/roles/states usable by accessibility trees and browser agents. | Inspect accessibility tree/semantic HTML and run representative agent task attempts. | NOT_APPLICABLE | coverage | HYBRID | PAGE | Does not guarantee operation by all agents/models. | AI_VISIBILITY, ACCESSIBILITY, UX | PLAUSIBLE_INDIRECT_RELATION | browser accessibility tree, agent harness | PARTIAL | DIAGNOSTIC_ONLY | LOW | S010 |

## 5. ANALYSIS METHODS CATALOG
| ID | Methode | Kategorien | Zweck | Inputs | Verfahren | Outputs | Auto | Reproduzierbarkeit | Evidenz | Quellen |
|---|---|---|---|---|---|---|---|---|---|---|
| AM01 | Evidence-ledger audit governance | C01 | Ensure every material claim has an observation/source or explicit uncertainty label. | findings, sources | Build claim-evidence matrix, verify source class, mark SOURCE_NEEDED/MISSING. | evidence ledger, coverage status | PARTIAL | HIGH | E6_PLAUSIBLE_PROXY | S035 |
| AM02 | Rendered technical crawl | C10, C11, C12, C13, C15, C16, C18 | Discover and inspect URLs, HTML, directives, links and rendered DOM. | seed URLs, crawl policy | Crawl raw HTML and optionally JS-rendered pages; retain response/DOM evidence. | URL inventory, technical findings | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S006, S010, S020 |
| AM03 | CrUX field-data analysis | C02, C03 | Assess real-user performance distributions for eligible Chrome populations. | origin/URL, device scope, time window | Query CrUX interfaces; record p75 and population limitations. | CWV field metrics | EXTERNAL_API | HIGH | E2_PLATFORM_OFFICIAL | S001, S002 |
| AM04 | Synthetic performance profiling | C04, C07, C08, C49 | Diagnose reproducible lab performance and regressions. | URL/build, device/network profile | Run repeated Lighthouse/WebPageTest/trace captures; report median/spread. | lab metrics, trace diagnostics | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S001, S035 |
| AM05 | RUM instrumentation review | C03, C43 | Validate first-party field telemetry quality and segmentation. | RUM schema, events, sampling | Inspect instrumentation, sample coverage, dimensions and aggregation. | RUM QA, data-quality findings | PARTIAL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S001 |
| AM06 | HTTP/TLS/DNS protocol inspection | C06, C41, C47 | Inspect transport, response semantics, caching and protocol configuration. | URLs/domains | Collect DNS, TLS handshake and HTTP headers/status/redirects. | protocol inventory, configuration findings | FULL | HIGH | E1_STANDARDIZED | S020, S021, S022, S023 |
| AM07 | Internal link-graph analysis | C24, C25, C26 | Model crawl/navigation graph, depth, orphan candidates and link distribution. | crawl graph, entry points | Build directed graph; compute shortest paths, indegree, components. | graph metrics, orphan/depth findings | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S035 |
| AM08 | Content duplicate clustering | C23 | Identify exact and near-duplicate page clusters. | page corpus | Normalize main content; hash exact duplicates; run declared similarity method for near duplicates. | duplicate clusters | FULL | MEDIUM | E6_PLAUSIBLE_PROXY | S007 |
| AM09 | Search Console query-performance analysis | C21, C28 | Analyze first-party Google query/page visibility and clicks. | Search Console property/access | Query API/report by page/query/device/country/date; retain aggregation caveats. | impressions, clicks, CTR, position, query clusters | EXTERNAL_API | HIGH | E2_PLATFORM_OFFICIAL | S003, S004 |
| AM10 | URL indexation inspection | C10, C11 | Compare technical eligibility with Google indexed-version state. | Search Console access, URL set | Crawl technical signals and query URL Inspection for selected URLs. | eligibility/index-state matrix | EXTERNAL_API | HIGH | E2_PLATFORM_OFFICIAL | S005, S008 |
| AM11 | Structured-data validation | C18, C19 | Validate machine-readable structured data and rich-result prerequisites. | rendered/raw HTML | Parse vocabulary, validate syntax/properties, map to current supported features. | schema inventory, eligibility diagnostics | PARTIAL | HIGH | E2_PLATFORM_OFFICIAL | S011, S012 |
| AM12 | Metadata conflict analysis | C16, C17 | Find conflicting or duplicate metadata across HTML, HTTP and social/semantic representations. | page corpus | Extract titles, descriptions, canonical, robots, lang, social and HTTP metadata; normalize and compare. | conflict matrix | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S008, S010, S013, S014 |
| AM13 | Intent and content-fit review | C20, C21, C22 | Assess whether content satisfies a defined user/search task and identify evidence-backed gaps. | query/task set, page corpus | Map query/task to explicit propositions, supporting evidence and missing facets. | fit review, coverage gaps | PARTIAL | MEDIUM | E6_PLAUSIBLE_PROXY | S003, S015 |
| AM14 | International annotation audit | C29 | Validate language/region alternate clusters and localization signals. | URL set | Parse hreflang/canonical/lang; test reciprocal relationships and target validity. | hreflang matrix, localization findings | FULL | HIGH | E2_PLATFORM_OFFICIAL | S015 |
| AM15 | Search-bot log analysis | C45 | Observe verified crawler behavior from server evidence. | server logs | Verify bot identities, aggregate URL/status/frequency patterns, compare to indexability and site changes. | bot traffic metrics, crawl diagnostics | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S044 |
| AM16 | WCAG-EM-oriented accessibility evaluation | C39 | Evaluate accessibility across a defined website scope using representative samples and mixed methods. | scope, sample, WCAG target level | Define scope/sample; run automated and manual checks; record per-criterion evidence. | criterion findings, conformance evidence | PARTIAL | HIGH | E1_STANDARDIZED | S017, S018, S019 |
| AM17 | Task-based usability testing | C40 | Measure effectiveness, efficiency and satisfaction on representative tasks. | target users, tasks, success criteria | Observe representative users; record completion, time, errors and qualitative friction. | task KPIs, usability findings | MANUAL | MEDIUM | E3_RESEARCH_VALIDATED | S040 |
| AM18 | Heuristic usability review | C40 | Quick expert identification of usability risks using a named heuristic framework. | interfaces, heuristic set | Expert inspection; cite observed UI evidence and severity. | heuristic findings | MANUAL | MEDIUM | E7_PRACTITIONER_HEURISTIC | S041 |
| AM19 | Consent-state browser audit | C42 | Observe storage/network behavior before and after consent choices. | public pages, consent states | Use clean browser profiles; capture cookies/storage/requests before choice, accept, reject and GPC where relevant. | tracker inventory, consent findings | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S042, S043 |
| AM20 | Analytics implementation QA | C43, C44 | Test whether analytics data represents the intended measurement plan. | measurement plan, analytics access, event capture | Compare events/parameters with plan, inspect thresholding/sampling and reconcile selected journeys. | data-quality report, KPI readiness | PARTIAL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S025, S027 |
| AM21 | Reliability SLI/SLO review | C46 | Evaluate availability, latency, error and traffic indicators against explicit product SLOs. | monitoring data, SLOs | Compute selected SLIs and compare to product-defined objectives and error budgets. | SLI dashboard, SLO gaps | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S024 |
| AM22 | Third-party dependency analysis | C52 | Measure external dependency footprint and operational/privacy/performance risk. | network trace, vendor inventory | Classify third parties by bytes/requests/purpose/data access/fallback/criticality. | dependency register, risk findings | PARTIAL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S036 |
| AM23 | Cross-browser compatibility matrix | C51 | Test representative flows/features across explicitly supported browsers/devices. | support matrix, flows | Map APIs to Baseline and run functional/visual test suite across matrix. | compatibility matrix, failures | FULL | HIGH | E2_PLATFORM_OFFICIAL | S037 |
| AM24 | AI visibility repeated-sampling experiment | C33, C34, C35, C38 | Estimate model/platform-specific mentions, citations and representation with uncertainty. | prompt panel, models, run count, time window | Freeze prompt set; run repeated randomized samples; record answer, citation, mention, rank/position only if platform defines it; report variance. | mention/citation distributions, uncertainty | PARTIAL | MEDIUM | E6_PLAUSIBLE_PROXY | S028, S030, S031, S032 |
| AM25 | AI crawler accessibility audit | C36 | Assess declared crawl access for distinct search/AI crawler identities. | robots.txt, official bot docs, URL set | Build bot-purpose registry; evaluate robots per bot/path; flag conflicts/unknowns. | crawler access matrix | FULL | HIGH | E2_PLATFORM_OFFICIAL | S006, S030 |
| AM26 | Passage answerability audit | C37 | Assess whether important questions can be answered from coherent local passages with explicit facts and qualifiers. | question set, content corpus | Map questions to best passages; evaluate completeness, ambiguity, sourceability and semantic structure. | passage map, answerability findings | PARTIAL | MEDIUM | E6_PLAUSIBLE_PROXY | S029, S031 |
| AM27 | Competitive cohort benchmarking | C50 | Compare metrics against a declared, methodologically comparable peer cohort. | peer set, same metric collection | Collect same metrics under aligned conditions; use distributions/percentiles, not arbitrary universal thresholds. | peer percentiles, gaps | PARTIAL | MEDIUM | E4_REPRODUCIBLE_INDUSTRY_METRIC | S035 |
| AM28 | Performance regression gate | C49 | Prevent releases that exceed product-defined performance budgets beyond expected variance. | baseline, candidate, budgets | Run repeated controlled tests and/or aligned RUM windows; compare deltas to versioned budgets. | gate result, regression evidence | FULL | HIGH | E4_REPRODUCIBLE_INDUSTRY_METRIC | S001 |
| AM29 | Sustainability evidence review | C53 | Assess resource-efficiency and draft sustainability practices without pretending a universal carbon truth. | page/task measurements, WSG draft | Measure bytes/requests/work where reproducible; map practices to WSG draft with draft labels. | resource-efficiency findings, draft-guideline map | PARTIAL | LOW | E8_UNCLEAR_OR_UNVALIDATED | S038 |
| AM30 | Agentic web task operability experiment | C54 | Test whether declared browser agents can complete representative website tasks reliably. | tasks, agent/runtime/version, browser profile | Run repeated task scripts, capture accessibility tree/interaction failures, compare fallback paths. | success distribution, agent friction findings | PARTIAL | LOW | E8_UNCLEAR_OR_UNVALIDATED | S039, S030 |

## 6. THRESHOLD & BENCHMARK REGISTER
Nur Schwellenwerte mit nachvollziehbarer Herkunft sind hier enthalten. Fehlt ein belastbarer Threshold, bleibt das Metric Record ausdrücklich bei `NONE_OFFICIAL`, `CONTEXT_DEPENDENT` oder einer Produktentscheidung.

| Metric | Threshold | Source | Scope | Population | Measurement Conditions | Official vs Empirical | Version/Date | Limitations |
|---|---|---|---|---|---|---|---|---|
| LCP | good <= 2.5 s; poor > 4.0 s | S001 | page/origin field population | eligible field users | 75th percentile; mobile and desktop segmented | PLATFORM_OFFICIAL | current CWV | Field population and tool scope must be disclosed. |
| INP | good <= 200 ms; poor > 500 ms | S001 | page/origin field population | eligible field users | 75th percentile; mobile and desktop segmented | PLATFORM_OFFICIAL | current CWV | Field only for true user interaction; lab tools use proxies. |
| CLS | good <= 0.1; poor > 0.25 | S001 | page/origin field population | eligible field users | 75th percentile; mobile and desktop segmented | PLATFORM_OFFICIAL | current CWV | Session/windowing semantics matter. |
| Core Web Vitals pass | all LCP, INP and CLS meet good threshold at p75 | S001 | page/origin assessment | eligible field users | p75 for all three metrics | PLATFORM_OFFICIAL | current CWV | Not a complete UX score. |
| WCAG 2.2 Target Size (Minimum) | 24 by 24 CSS pixels OR documented spacing/exception conditions | S017 | interactive target | not population-based | WCAG 2.2 SC 2.5.8, Level AA | STANDARD | 2023-10-05 | Exceptions and spacing conditions must be evaluated. |
| Sitemap file capacity | <=50 MB uncompressed and <=50,000 URLs | S009 | individual sitemap file | not population-based | Google-supported sitemap guidance | PLATFORM_OFFICIAL | verified 2026-08-26 | Sitemap index can split larger sites. |
| Long Task definition | >=50 ms task duration | S001 | browser main-thread task | runtime event | Long Tasks API semantics | PLATFORM_OFFICIAL | verified 2026-08-26 | Definition threshold, not an acceptable page-count target. |

## 7. GEO & AI DISCOVERABILITY SPECIAL REPORT
### Bereits reproduzierbar messbar
- Plattform-eigene Messungen, wenn die Plattform sie ausweist: z. B. Google Search Console generative-AI performance reporting; ChatGPT referral attribution in eigener Analytics-Pipeline.
- robots-basierte Erreichbarkeit für klar dokumentierte Crawler wie OAI-SearchBot oder Googlebot. Das beweist nur Zugangspolitik, nicht Aufnahme, Retrieval oder Zitation.
### Vendor-spezifisch messbar
- AI Share of Voice, mention/citation/impressions scores aus Ahrefs/Semrush/anderen Plattformen. Diese sind E5, weil Prompt-Korpus, Konkurrenzset und Formel vendorabhängig sind.
### Experimentell messbar
- Repeated prompt sampling für answer inclusion, mention rate, citation rate, entity consistency; nur mit festem Promptpanel, Modellversion, Run-Anzahl, Zeitpunkt und Varianzbericht.
- GEO-Forschung kann experimentelle Interventionswirkungen zeigen, liefert aber keinen universellen dauerhaften Cross-Platform-KPI.
### Theoretisch plausibel, aber nicht ausreichend standardisiert
- Passage answerability/retrievability, machine-readable entity consistency, agentic action discoverability. Nützlich diagnostisch; harte Scores wären Scheingenauigkeit.
### Benchmark-Design
1. Prompt-/Query-Universum aus realen Nutzerfragen definieren; 2. stratified sampling; 3. mehrere Runs pro Prompt/Modell; 4. Modell/Version/Zeitpunkt fixieren; 5. mention und citation strikt trennen; 6. Quellen-/Attributionsqualität separat prüfen; 7. Konfidenzintervalle/Run-Varianz berichten; 8. Plattformen nicht ohne Methodennormalisierung aggregieren.

## 8. DEPRECATED / WEAK / MISLEADING METRICS
| Metrik/Behauptung | Status | Warum problematisch | Stattdessen | Quellen |
|---|---|---|---|---|
| First Input Delay as current Core Web Vital | DEPRECATED | INP replaced FID as a Core Web Vital; historical FID can be retained only for trend context. | INP | S001 |
| Universal 50-60 character title threshold | MISLEADING_HEURISTIC | Google documents multiple title-link sources but no fixed official character-count ranking threshold. | content/title consistency plus observed representation | S013 |
| Universal 150-160 character meta-description threshold | MISLEADING_HEURISTIC | Snippet length and source selection vary; no fixed official length threshold. | descriptive relevance and observed snippet behavior | S014 |
| Domain Rating / Domain Authority as Google authority | VENDOR_SPECIFIC | Vendor backlink composites are not official Google metrics and indexes/methods differ. | vendor metric with explicit source plus direct backlink/query evidence | S033, S034, S016 |
| Lighthouse Performance score as real-user UX | MISLEADING_IF_UNQUALIFIED | It is a lab composite; field users differ by devices, networks and behavior. | CWV field data plus repeated lab diagnostics | S001 |
| Average position as exact stable Google rank | MISLEADING_IF_UNQUALIFIED | Search Console position is an averaged topmost element position with result-type and impression semantics. | query/page/device/time-segmented position plus impressions/clicks | S003 |
| Bounce rate as universal content-quality KPI | CONTEXT_DEPENDENT | GA4 bounce is the inverse of engaged-session logic; good/bad depends on page task and measurement design. | task/key-event metrics plus engagement context | S026 |
| E-E-A-T score | NON_STANDARDIZED | No official universal numeric E-E-A-T score is defined for site audits. | evidence-backed content/source/author/entity review | S015, S016 |
| Single SEO health score | COMPOSITE_PRODUCT_DECISION | Combines heterogeneous signals and can hide blockers/context; no universal weighting exists. | category findings plus transparent product-defined weighting if needed | S035 |
| AI Share of Voice as cross-platform standard | VENDOR_SPECIFIC | Prompt sets, competitors, models, sessions and vendor methods differ. | platform-specific distributions with sampling metadata | S032 |
| AI citation rate as ranking factor | UNSUPPORTED_CAUSAL_CLAIM | Citation frequency can be observed experimentally/vendor-side, but no universal causal ranking-factor interpretation is established. | diagnostic AI visibility experiment with uncertainty | S028, S030, S031, S032 |
| llms.txt presence as universal AI visibility requirement | LOW_EVIDENCE | Current major-platform guidance does not establish it as a universal inclusion requirement. | crawl/index controls and high-quality accessible content per platform guidance | S029, S030 |
| Automated accessibility score as WCAG conformance | MISLEADING | W3C explicitly requires human judgment; tools cannot alone determine conformance. | per-criterion mixed-method assessment | S017, S018, S019 |
| Universal 99.9% website availability target | PRODUCT_DECISION | SLO targets must follow user/business reliability needs and cost tradeoffs. | explicit service SLI/SLO/error budget | S024 |
| Generic carbon score without disclosed model | LOW_EVIDENCE | Sustainability conversion depends on energy/network/device assumptions and W3C guidance remains draft. | direct resource-efficiency measurements plus transparent model if used | S038 |

## 9. SOURCE LEDGER
| Source ID | Organisation/Autor | Titel | URL | Publikation | Update | Abruf | Tier | Kategorien | Gestützte Aussagen | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| S001 | Google / web.dev | Web Vitals | https://web.dev/articles/vitals | 2020-05-04 | 2024-10-31 | 2026-08-26 | A | C02, C03, C04 | Core Web Vitals definitions, p75 aggregation, thresholds, field/lab distinction | VERIFIED |
| S002 | Google Chrome | Chrome User Experience Report documentation | https://developer.chrome.com/docs/crux | UNKNOWN | UNKNOWN | 2026-08-26 | A | C03 | CrUX field-data model and interfaces | VERIFIED |
| S003 | Google | Search Console: impressions, position and clicks | https://support.google.com/webmasters/answer/7042828 | UNKNOWN | UNKNOWN | 2026-08-26 | A | C28 | Definitions and limitations of impressions, clicks, CTR and average position | VERIFIED |
| S004 | Google | Search Analytics API | https://developers.google.com/webmaster-tools/v1/searchanalytics/query | UNKNOWN | 2026-08-11 | 2026-08-26 | A | C28 | Search Analytics API dimensions, aggregation and row limitations | VERIFIED |
| S005 | Google | URL Inspection API | https://developers.google.com/webmaster-tools/v1/urlInspection.index/inspect | UNKNOWN | UNKNOWN | 2026-08-26 | A | C10, C11 | Indexed-version inspection limitations | VERIFIED |
| S006 | IETF | RFC 9309: Robots Exclusion Protocol | https://www.rfc-editor.org/rfc/rfc9309.html | 2022-09 | UNKNOWN | 2026-08-26 | A | C10, C12, C36 | Standardized robots.txt syntax and behavior | VERIFIED |
| S007 | Google Search Central | Consolidate duplicate URLs / canonicalization | https://developers.google.com/search/docs/crawling-indexing/consolidate-duplicate-urls | UNKNOWN | UNKNOWN | 2026-08-26 | A | C11, C12, C23 | Canonical signal strengths and non-guarantee | VERIFIED |
| S008 | Google Search Central | Robots meta tag and X-Robots-Tag | https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag | UNKNOWN | UNKNOWN | 2026-08-26 | A | C11, C12, C16 | Indexing directives and crawlability prerequisite | VERIFIED |
| S009 | Google Search Central | Build and submit a sitemap | https://developers.google.com/search/docs/crawling-indexing/sitemaps/build-sitemap | UNKNOWN | UNKNOWN | 2026-08-26 | A | C10, C12 | Sitemap size and URL requirements | VERIFIED |
| S010 | WHATWG | HTML Living Standard | https://html.spec.whatwg.org/ | UNKNOWN | 2026-08-26 | 2026-08-26 | A | C15, C16, C19 | Normative HTML semantics and metadata vocabulary | VERIFIED |
| S011 | Schema.org | Schema.org v30.0 | https://schema.org/ | 2026-03-19 | UNKNOWN | 2026-08-26 | A | C18, C19 | Structured-data vocabulary | VERIFIED |
| S012 | Google Search Central | Structured data general guidelines | https://developers.google.com/search/docs/appearance/structured-data/sd-policies | UNKNOWN | UNKNOWN | 2026-08-26 | A | C18 | Eligibility requirements and no-guarantee of rich results | VERIFIED |
| S013 | Google Search Central | Influencing title links | https://developers.google.com/search/docs/appearance/title-link | UNKNOWN | UNKNOWN | 2026-08-26 | A | C16, C17 | Title-link source signals and absence of a fixed title-length threshold | VERIFIED |
| S014 | Google Search Central | Control snippets in search results | https://developers.google.com/search/docs/appearance/snippet | UNKNOWN | UNKNOWN | 2026-08-26 | A | C16, C17 | Snippet generation and meta-description role; no universal character threshold | VERIFIED |
| S015 | Google Search Central | Search Essentials | https://developers.google.com/search/docs/essentials | UNKNOWN | UNKNOWN | 2026-08-26 | A | C13, C14, C20, C21 | Baseline technical and content requirements | VERIFIED |
| S016 | Google Search Central | A guide to Google Search ranking systems | https://developers.google.com/search/docs/appearance/ranking-systems-guide | UNKNOWN | UNKNOWN | 2026-08-26 | A | C13, C20, C27 | Many ranking systems/signals and link analysis/PageRank role | VERIFIED |
| S017 | W3C | Web Content Accessibility Guidelines (WCAG) 2.2 | https://www.w3.org/TR/WCAG22/ | 2023-10-05 | UNKNOWN | 2026-08-26 | A | C39 | Accessibility success criteria and conformance levels | VERIFIED |
| S018 | W3C WAI | Evaluating Web Accessibility Overview | https://www.w3.org/WAI/test-evaluate/ | UNKNOWN | UNKNOWN | 2026-08-26 | A | C39 | Automated tools cannot alone determine accessibility conformance | VERIFIED |
| S019 | W3C WAI | WCAG-EM 1.0 | https://www.w3.org/TR/WCAG-EM/ | UNKNOWN | UNKNOWN | 2026-08-26 | A | C39, C01 | Structured website accessibility evaluation methodology | VERIFIED |
| S020 | IETF | RFC 9110: HTTP Semantics | https://www.rfc-editor.org/rfc/rfc9110.html | 2022-06 | UNKNOWN | 2026-08-26 | A | C06, C47 | HTTP semantics and status codes | VERIFIED |
| S021 | IETF | RFC 9111: HTTP Caching | https://www.rfc-editor.org/rfc/rfc9111.html | 2022-06 | UNKNOWN | 2026-08-26 | A | C06 | HTTP caching semantics | VERIFIED |
| S022 | IETF | RFC 9846: TLS Protocol Version 1.3 | https://www.rfc-editor.org/rfc/rfc9846.html | 2026-07 | UNKNOWN | 2026-08-26 | A | C06, C41 | Current TLS 1.3 protocol; obsoletes RFC 8446 | VERIFIED |
| S023 | IETF | RFC 9114: HTTP/3 | https://www.rfc-editor.org/rfc/rfc9114.html | 2022-06 | UNKNOWN | 2026-08-26 | A | C06 | HTTP/3 semantics over QUIC | VERIFIED |
| S024 | Google SRE | Monitoring Distributed Systems | https://sre.google/sre-book/monitoring-distributed-systems/ | UNKNOWN | UNKNOWN | 2026-08-26 | C | C05, C46 | Latency, traffic, errors and saturation as operational signals | VERIFIED |
| S025 | Google Analytics | GA4 dimensions and metrics | https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema | UNKNOWN | 2026-08-19 | 2026-08-26 | A | C43, C44 | Analytics metrics and dimensions | VERIFIED |
| S026 | Google Analytics | Engagement rate and bounce rate | https://support.google.com/analytics/answer/12195621 | UNKNOWN | UNKNOWN | 2026-08-26 | A | C44 | GA4 engaged-session and rate definitions | VERIFIED |
| S027 | Google Analytics | Data thresholds | https://support.google.com/analytics/answer/9383630 | UNKNOWN | UNKNOWN | 2026-08-26 | A | C43 | Privacy thresholding can suppress report data | VERIFIED |
| S028 | Google Search Central | Generative AI performance reports in Search Console | https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports | 2026-06-03 | UNKNOWN | 2026-08-26 | A | C33, C34, C35 | First-party Search Console reporting for generative AI search surfaces | VERIFIED |
| S029 | Google Search Central | AI features and your website | https://developers.google.com/search/docs/appearance/ai-features | UNKNOWN | UNKNOWN | 2026-08-26 | A | C33, C34, C36, C37 | No special AI technical requirements beyond core Search; query fan-out and crawl/index prerequisites | VERIFIED |
| S030 | OpenAI | Publishers and Developers FAQ | https://help.openai.com/en/articles/12627856 | UNKNOWN | 2026-08 | 2026-08-26 | A | C34, C35, C36, C54 | OAI-SearchBot controls, GPTBot distinction, noindex behavior and ChatGPT referral attribution | VERIFIED |
| S031 | Aggarwal et al. | GEO: Generative Engine Optimization | https://arxiv.org/html/2311.09735v3 | 2024 | UNKNOWN | 2026-08-26 | B | C33, C34, C35, C37 | GEO-bench and experimental visibility interventions | VERIFIED |
| S032 | Ahrefs | AI Visibility Metrics | https://help.ahrefs.com/en/articles/15501968-ai-visibility-metrics | UNKNOWN | 2026 | 2026-08-26 | D | C34, C35, C38 | Vendor definitions of mentions, citations, impressions and AI share of voice | VERIFIED |
| S033 | Ahrefs | Domain Rating | https://help.ahrefs.com/en/articles/1409408-what-is-domain-rating-dr | UNKNOWN | UNKNOWN | 2026-08-26 | D | C27, C50 | Vendor-specific relative backlink score; not an official search-engine metric | VERIFIED |
| S034 | Semrush | Authority Score explained | https://www.semrush.com/kb/747-authority-score-backlink-scores | UNKNOWN | UNKNOWN | 2026-08-26 | D | C27, C50 | Vendor composite authority score | VERIFIED |
| S035 | HTTP Archive | Web Almanac 2025 - Table of Contents | https://almanac.httparchive.org/en/2025/table-of-contents | 2026-01 | UNKNOWN | 2026-08-26 | C | C01, C48, C50, C51, C52 | Large-scale audit dimensions and gap discovery | VERIFIED |
| S036 | HTTP Archive | Web Almanac 2025 - Third Parties | https://almanac.httparchive.org/en/2025/third-parties | 2026-01 | UNKNOWN | 2026-08-26 | C | C52 | Third-party prevalence, performance, privacy and security implications | VERIFIED |
| S037 | web.dev | Baseline | https://web.dev/baseline/ | UNKNOWN | UNKNOWN | 2026-08-26 | A | C51 | Cross-browser feature availability status and Baseline definitions | VERIFIED |
| S038 | W3C Sustainable Web IG | Web Sustainability Guidelines | https://www.w3.org/TR/web-sustainability-guidelines/ | 2026-07 | 2026-08 | 2026-08-26 | A | C53 | Draft sustainability guidance; explicitly work in progress | VERIFIED_DRAFT |
| S039 | Google Search Central | AI optimization / agentic experiences guidance | https://developers.google.com/search/docs/appearance/ai-features | UNKNOWN | 2026 | 2026-08-26 | A | C33, C54 | Agentic experiences are emerging/optional; core crawlable semantic web remains foundational | VERIFIED |
| S040 | ISO | ISO 9241-11:2018 Ergonomics of human-system interaction — Usability | https://www.iso.org/standard/63500.html | 2018 | UNKNOWN | 2026-08-26 | A | C40 | Usability concepts of effectiveness, efficiency and satisfaction | VERIFIED |
| S041 | Nielsen Norman Group | 10 Usability Heuristics for User Interface Design | https://www.nngroup.com/articles/ten-usability-heuristics/ | UNKNOWN | UNKNOWN | 2026-08-26 | E | C40 | Widely used qualitative heuristics; rules of thumb, not standardized numeric KPIs | VERIFIED |
| S042 | W3C | Global Privacy Control (GPC) | https://www.w3.org/TR/gpc/ | 2026-06-11 | UNKNOWN | 2026-08-26 | A | C42 | Sec-GPC / navigator.globalPrivacyControl specification; Working Draft | VERIFIED_DRAFT |
| S043 | CJEU | Planet49 judgment C-673/17 | https://curia.europa.eu/juris/liste.jsf?num=C-673/17 | 2019-10-01 | UNKNOWN | 2026-08-26 | A | C42 | Consent requires active behavior for non-essential cookies; pre-ticked boxes insufficient | VERIFIED |
| S044 | Google Search Central | Verify Googlebot | https://developers.google.com/search/docs/crawling-indexing/verifying-googlebot | UNKNOWN | UNKNOWN | 2026-08-26 | A | C10, C45 | Reverse/forward DNS and published IP ranges for bot verification | VERIFIED |

## 10. COVERAGE & GAP REPORT
- **Status:** `COVERAGE_SATURATION_REACHED` — Relative saturation for the documented source/query strategy, not a claim that every website metric worldwide has been found.
- **Baseline:** C01-C50 wurden alle mit mindestens einem normalisierten Record abgedeckt.
- **Pass A:** Missing dimensions and alternate audit frameworks: browser interoperability, third parties, sustainability, capabilities/PWA. Neu: C51, C52, C53; 9 neue valide Konzepte; 6 verworfen/eingefaltet.
- **Pass B:** AI/agentic guidance plus cross-check against broad Web Almanac and standards coverage. Neu: C54; 3 neue valide Konzepte; 8 verworfen/eingefaltet.
- **Neue Kategorien:** C51 Browser Compatibility & Interoperability; C52 Third-Party Dependencies; C53 Web Sustainability; C54 Agentic Web Operability.
- **Offene Evidenzlücken:** Standardized cross-platform GEO measurement; Stable agentic-web metrics; Stable sustainability conformance/impact model; Jurisdiction-specific privacy compliance mapping; Industry-specific conversion benchmarks.

## 11. SKILL IMPLEMENTATION CATALOG
| Modul | Messungen | benötigte Inputs | Tool/API | automatisierbar | Skill-Logik | Report-Output | Scoring möglich? | Einschränkungen |
|---|---|---|---|---|---|---|---|---|
| MOD01 Audit Governance | M001, M002, M003 | scope, claims, evidence | report validator/source ledger | PARTIAL | claim-evidence gating and uncertainty labels | evidence coverage, missing evidence | context only | does not improve weak sources |
| MOD02 Performance Field | M004, M005, M006, M007, M009, M010, M011 | origin/URL | CrUX API/RUM | EXTERNAL_API/FULL | p75 field population and CWV thresholds | field performance | yes with context | CrUX eligibility/population |
| MOD03 Performance Lab | M014, M015, M016, M017, M018, M027, M028, M029 | URL/build/test profile | Lighthouse/WebPageTest/browser | FULL | repeat runs, variance, diagnostics | lab profile | vendor/context | not field UX |
| MOD04 Crawl & Index | M036, M037, M039, M040, M041, M042, M043, M044 | site URL + optional Search Console | crawler, URL Inspection | FULL/EXTERNAL_API | separate crawlability, indexability, platform state | URL state matrix | diagnostic | eligibility != index/rank |
| MOD05 Semantics & Metadata | M046, M048, M049, M050, M051, M052, M053, M054 | HTML/rendered DOM | crawler/browser | FULL/PARTIAL | normalize semantic/metadata conflicts | semantic metadata findings | diagnostic | presentation may be rewritten |
| MOD06 Structured Data & Entity | M055, M056, M057, M058 | HTML/JSON-LD | schema parsers/Rich Results Test | FULL/PARTIAL | syntax, eligibility, entity consistency | machine-readability findings | diagnostic | no appearance guarantee |
| MOD07 Content & Intent | M059, M060, M061, M062, M063, M064 | content, query/task data | Search Console + semantic/manual review | PARTIAL | task-fit and evidence-backed gaps | content findings | mostly no | subjectivity/causality |
| MOD08 Architecture & Links | M065, M066, M067, M068, M069, M070 | crawl graph + optional backlink provider | crawler/graph/vendor APIs | FULL/EXTERNAL_API | graph before vendor authority proxies | link/IA diagnostics | context only | vendor index differences |
| MOD09 Search Performance | M071, M072, M073, M074 | Search Console access | Search Analytics API | EXTERNAL_API | query/page/device/time segmentation | organic search performance | context | platform aggregation semantics |
| MOD10 Accessibility & UX | M099, M100, M101, M102, M103, M104 | pages, tasks, users where available | axe/browser/manual/usability study | PARTIAL | automation plus human review | WCAG evidence and usability findings | criterion/task specific | automated-only conformance prohibited |
| MOD11 Security Privacy Reliability | M105, M106, M107, M108, M109, M110, M120, M121, M122, M123 | public site + optional monitoring | browser/network/server monitoring | FULL/PARTIAL | standards behavior plus jurisdiction/SLO context | trust/reliability findings | context only | not legal/security certification |
| MOD12 Analytics Integrity | M111, M112, M113, M114, M115, M116 | measurement plan + analytics credentials | GA4 Data API/tag debugger | EXTERNAL_API/PARTIAL | validate data before business KPI interpretation | measurement integrity + KPI readiness | product-specific | credentials/configuration required |
| MOD13 Logs & Architecture | M117, M118, M119, M124, M125 | server logs + public/runtime site | log parser/browser crawler | FULL | server truth for bot behavior, rendered/raw comparison | bot and architecture diagnostics | diagnostic | logs/architecture access vary |
| MOD14 AI/GEO Evidence | M083, M084, M085, M086, M087, M088, M089, M090, M091, M092, M093, M094, M095, M096, M097, M098 | Search Console/vendor/model access + prompt panel | GSC, crawler, model/vendor APIs | PARTIAL/EXTERNAL_API | platform-specific sampling with variance; no universal GEO score | AI visibility distributions and crawler access | mostly diagnostic | stochastic/vendor/model/time dependence |
| MOD15 Advanced Platform | M126, M127, M128, M129, M130, M131, M132, M133, M134, M135, M136, M137, M138 | CI/peers/browser matrix/network/agent tasks | CI, HTTP Archive, browser, agent harness | PARTIAL/FULL | advanced enterprise diagnostics and emerging capabilities | regression, compatibility, supply chain, sustainability, agentic findings | context/experimental | C53/C54 emerging |

## 12. IMPLEMENTATION PRIORITIES
- **P0 — fundamentale Auditfähigkeit:** C01, C02, C03, C04, C05, C06, C10, C11, C12, C13, C15, C16, C18, C25, C28, C39, C41, C46, C47. Kern: technische Erreichbarkeit, Performance, Index-/HTTP-Semantik, Search Performance, Accessibility, Security/Reliability.
- **P1 — hoher zusätzlicher Erkenntniswert:** C07, C08, C09, C14, C17, C20, C21, C23, C24, C26, C29, C31, C32, C40, C42, C43, C44, C45, C49, C51, C52. Ergänzt Diagnose, UX/Content, Analytics, Privacy, Logs, Regression, Interop und Third Parties.
- **P2 — Advanced Enterprise Capability:** C19, C22, C27, C30, C36, C37, C48, C50. Benötigt mehr Kontext, externe Daten oder vorsichtige Proxy-Interpretation.
- **P3 — experimentell / geringe Standardisierung:** C33, C34, C35, C38, C53, C54. GEO/AI-Sampling, Sustainability und Agentic Web dürfen nicht als stabile harte KPI-Ebene verkauft werden.

## 13. MACHINE-READABLE FIELD MODEL
```json
{
  "metric_id": "",
  "canonical_name": "",
  "aliases": [],
  "category": "",
  "subcategory": "",
  "item_type": "",
  "definition": "",
  "evidence_class": "",
  "measurement": {
    "mode": "",
    "scope": "",
    "formula": "",
    "unit": "",
    "procedure": "",
    "required_inputs": []
  },
  "interpretation": {
    "directionality": "",
    "thresholds": [],
    "benchmarks": [],
    "does_not_prove": []
  },
  "impact": {
    "areas": [],
    "mechanism": "",
    "evidence_type": ""
  },
  "comparability": {
    "cross_page": "",
    "cross_site": "",
    "cross_tool": "",
    "limitations": []
  },
  "implementation": {
    "tools": [],
    "api_options": [],
    "automation_feasibility": "",
    "scoring_eligibility": ""
  },
  "confidence": "",
  "sources": []
}
```
Das ausführbare Schema liegt zusätzlich als `metric_record.schema.json` vor.

## 14. FINAL RESEARCH VERDICT
1. **Methodisch am ausgereiftesten:** Web-/HTTP-Standards, Core Web Vitals mit Feldpopulation und p75-Schwellen, Search-Console-Messdefinitionen, robots/canonical/index directives, WCAG-Kriterien, Status-/Reliability-Messung.
2. **Gut messbar, Impact aber unsicher:** viele resource/runtime diagnostics, internal-link graph metrics, third-party footprint, vendor backlink metrics; Messung ist real, Business-/Rankingwirkung oft nur indirekt.
3. **Stark vendorabhängig:** DR/Authority Scores, Backlink-Indizes, SERP-volatility scores, die meisten AI visibility/SOV products.
4. **Bereits belastbare GEO/AI-Messung:** crawler access als technische Bedingung; plattformeigene Reportingdaten, sofern verfügbar; eigene Referral-Daten. Cross-platform visibility bleibt nicht standardisiert.
5. **Nicht als harte KPI:** allgemeiner GEO Score, AI citation/mention rate ohne Samplingprotokoll, DR/DA als Google authority, automatischer accessibility score als Conformance, starre title/meta length rules, avg position als exakter Rang.
6. **Enterprise-unverzichtbar:** Crawl/Index/HTTP, field+lab performance, semantics/metadata, structured data eligibility, Search Console, accessibility, security/privacy behavior, analytics integrity, reliability/error architecture.
7. **Nur diagnostisch:** Proxies, Vendor-Scores, semantic/entity consistency, content-gap scores, AI passage/agentic metrics, many comparative benchmarks.
8. **Zwingende Daten/Tools:** crawler + JS browser, HTTP/TLS/DNS inspector, CrUX/RUM, Search Console for owner data, accessibility mixed-method tooling, analytics/log/monitoring when deeper business/runtime claims are desired.
9. **Ohne Credentials möglich:** public crawl/render, lab performance, HTML/metadata/schema, robots/sitemaps, HTTP/TLS, many accessibility automation checks, third-party/network footprint, cross-browser basic tests. Owner metrics require credentials.
10. **Offene Forschung:** stable GEO standardization, sampling science for AI visibility, durable cross-model causal effects, agentic-web interoperability, standardized sustainability impact, domain-specific business benchmarks.

### Quality Gate
| Check | Status | Evidence |
|---|---|---|
| CHECK_1_TAXONOMY_COVERAGE | PASS | All C01-C50 investigated; gap passes added C51-C54. |
| CHECK_2_SOURCE_QUALITY | PASS | Central definitions/thresholds anchored in W3C, IETF, WHATWG, Google/OpenAI official docs; vendor sources isolated. |
| CHECK_3_METRIC_NORMALIZATION | PASS | Canonical IDs and one primary item type per record; aliases/vendor variants represented without merging semantics. |
| CHECK_4_KPI_VS_HEURISTIC | PASS | Nine item types retained; vendor/proxy/heuristic records explicitly classified. |
| CHECK_5_IMPACT_DISCIPLINE | PASS | Each metric includes impact_evidence and does_not_prove; causal claims are not inferred from correlation. |
| CHECK_6_THRESHOLD_VALIDITY | PASS | Threshold register contains only traceable standard/platform thresholds; common SEO character limits excluded. |
| CHECK_7_COMPARABILITY | PASS | Every metric includes comparison requirements and confounders; cross-tool/site claims are conditional. |
| CHECK_8_GEO_SKEPTICISM | PASS | GEO/AI metrics split into official first-party, vendor, experimental and proxy classes; no universal GEO score. |
| CHECK_9_IMPLEMENTABILITY | PASS | 15 implementation modules map inputs, tools/APIs, automation and report output. |
| CHECK_10_DEPRECATION | PASS | Deprecated/weak register covers FID, fixed title/meta lengths, authority scores, single scores and AI overclaims. |
| CHECK_11_AUTOMATION | PASS | Every metric has measurement mode, possible tools/APIs and automation_feasibility. |
| CHECK_12_UNCERTAINTY | PASS | MISSING/SOURCE_NEEDED semantics preserved; draft and emerging domains labeled. |

**Release decision:** `RELEASE` as a research and implementation basis. This is not certification, legal compliance confirmation, or proof that every possible metric worldwide has been discovered.
