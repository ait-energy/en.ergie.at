---
title: "Zusammenfassung und Vergleich der Praxisbeispiele"
topics: []
authors: [afischer]
showSummary: true
weight: 7
series: ["Variable Tarife – International"]
series_order: 7
showTableOfContents: false
---

Die folgende Übersicht stellt die beschriebenen Praxisbeispiele anhand der fünf [Gestaltungsdimensionen]({{< ref "themen/variable-tarife/grundlagen.md#gestaltungsdimensionen" >}}) gegenüber.

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

{{< accordion >}}
{{< accordionItem title="Legende der Abkürzungen" >}}
| Dimension | Abkürzungen |
|----|----|
| Block + Richtung | „En-Bez“: Energiepreis Bezug;<br>„En-Ein“: Energiepreis Einspeisung;<br>„NE-Bez“: Netzentgelt Bezug;<br>„NE-Ein“: Netzentgelt Einspeisung;<br>„Abg-Bez“: Abgaben Bezug;<br>„Abg-Ein“: Abgaben Einspeisung |
| Art der Differenzierung | „Stat-ZV“: statisch-zeitvariabel;<br>„Dyn-ZV“: dynamisch-zeitvariabel;<br>„Stat-OV“: statisch-ortsvariabel;<br>„Dyn-OV“: dynamisch-ortsvariabel<br>„kD“: keine Dynamik |
| Komponente | „AP“: Arbeitspreis;<br>„LP“: Leistungspreis (gemessen);<br>„KP“: Kapazitätspreis (kontrahiert);<br>„GP“: Grundpreis;<br>„AE“: Anschlussentgelt;<br>„„-MS“ an AP/LP“: mit Mengenschwelle (Zusatz, z.B. AP-MS) |
| Primäre Wirkung | „SLR“: Spitzenlastreduktion;<br>„LV“: Lastverschiebung;<br>„IR“: Investitionsanreiz; „–“: anreizfrei (Kostendeckung) |
| Zugang (Nutzer:innensicht) | „Pfl“: verpflichtend;<br>„Opt“: Wahlfreiheit / Opt-in;<br>„Opt-GG“: optional, an Gegenleistung geknüpft (z. B. § 14a EnWG) |
{{< /accordionItem >}}
{{< /accordion >}}

| Land | Mechanismus | Block + Richtung | Art | Kompo-nente | Wirkung | Zugang | Anmerkung |
|----|----|----|----|----|----|----|----|
| [ES]({{< ref "themen/variable-tarife/international/es.md" >}}) | Netztarif 2.0 TD – Arbeitspreis (\< 15 kW) | NE-Bez | Stat-ZV | AP | LV | Pfl | Drei ganzjährig fixe Zeitzonen (Valle / Llano / Punta). |
| [ES]({{< ref "themen/variable-tarife/international/es.md" >}}) | Netztarif 2.0 TD – Leistungsanteil | NE-Bez | Stat-ZV | KP | SLR | Pfl | Zwei Zeitzonen; kontrahierte Leistung je Zeitfenster frei wählbar, Begrenzung über Leistungsschalter. |
| [ES]({{< ref "themen/variable-tarife/international/es.md" >}}) | Netztarif 3.0 TD – Arbeitspreis (15–450 kW) | NE-Bez | Stat-ZV | AP | LV | Pfl | Sechs Zeitzonen (P1–P6), saisonal variierende Zeitfenster. |
| [ES]({{< ref "themen/variable-tarife/international/es.md" >}}) | Netztarif 3.0 TD – Leistungsanteil | NE-Bez | Stat-ZV | KP | SLR | Pfl | Gleiche sechs Zeitzonen wie der Arbeitspreis. |
| [ES]({{< ref "themen/variable-tarife/international/es.md" >}}) | PVPC – Energiekomponente (\< 10 kW) | En-Bez | Dyn-ZV | AP | LV | Opt | Viertelstündlich nach Day-Ahead/Intraday, gedämpft durch Terminmarktanteil (2026: 55 %); Netzentgelt (2.0 TD) und cargos additiv, aber nicht variabel. |
| [FR]({{< ref "themen/variable-tarife/international/fr.md" >}}) | TURPE 7 – Fixe Bezugskomponente (CSF) | NE-Bez | kD | KP | SLR | Pfl | €/kVA/Jahr auf Basis der vertraglich vereinbarten Leistung, ohne zeitliche Differenzierung. |
| [FR]({{< ref "themen/variable-tarife/international/fr.md" >}}) | TURPE 7 – Variable Bezugskomponente (CSV) | NE-Bez | Stat-ZV | AP | LV | Pfl | Vier Zeitfenster aus zwei Saisons × HP/HC; 8 Niederstunden pro Tag, davon mind. 5 nachts. |
| [FR]({{< ref "themen/variable-tarife/international/fr.md" >}}) | TURPE 7 – Speicheroption (ab 08/2026) | NE-Bez + NE-Ein | Stat-ZV + Stat-OV | AP | LV | Opt | Symmetrisch über beide Flussrichtungen. |
| [NO]({{< ref "themen/variable-tarife/international/no.md" >}}) | Kapazitätskomponente (fastledd) | NE-Bez | kD | LP | SLR | Pfl | Stufung nach dem Durchschnitt der drei höchsten Tageslastspitzen eines Monats |
| [NO]({{< ref "themen/variable-tarife/international/no.md" >}}) | Arbeitspreis (energiledd) | NE-Bez | Stat-ZV | AP | LV | Pfl | Tag vs. Nacht/Wochenende; Differenzierung regulatorisch erlaubt, Ausgestaltung und Höhe liegen beim DSO. |
| [DE]({{< ref "themen/variable-tarife/international/de.md" >}}) | § 14a EnWG – Modul 1 (pauschale Reduzierung) | NE-Bez | kD | GP | – | Opt-GG | Fixbetrag 110–190 €/a als Kompensation für die Duldung der Steuerung; keine eigene Preissignalwirkung. |
| [DE]({{< ref "themen/variable-tarife/international/de.md" >}}) | § 14a EnWG – Modul 2 (prozentuale Reduzierung) | NE-Bez | kD | AP | – | Opt-GG | Arbeitspreis auf 40 % am separaten Zählpunkt, kein Grundpreis; Reduktion ist nicht zeitlich differenziert. |
| [DE]({{< ref "themen/variable-tarife/international/de.md" >}}) | § 14a EnWG – Modul 3 (zeitvariables Netzentgelt) | NE-Bez | Stat-ZV | AP | LV | Opt-GG | Drei Preisstufen (HT/ST/NT), kalenderjährlich und netzgebietsweit festgelegt; nur in Kombination mit Modul 1; intelligentes Messsystem erforderlich. |
| [DE]({{< ref "themen/variable-tarife/international/de.md" >}}) | AgNes – Netzentgelte mit Anreizfunktion (Konzept Dez. 2025) | NE-Bez + NE-Ein | Dyn-ZV + Dyn-OV | AP | LV | Opt / Pfl | Einziges Beispiel für echte Dynamik im Sinne der [Begriffsdefinition]({{< ref "themen/variable-tarife/grundlagen.md#zeitliche-differenzierung" >}}): 15-minütig, räumlich vor/hinter Engpass differenziert, symmetrisch vorzeichengerecht, Veröffentlichung vor Day-Ahead-Closure. Konkretisierung auf 2027 verschoben; Einführung frühestens 2030 (Speicher) bzw. 2032 (Einspeisende). |
| [DE]({{< ref "themen/variable-tarife/international/de.md" >}}) | AgNes – Finanzierungsfunktion Niederspannung (\< 100.000 kWh) | NE-Bez | kD | GP | – | Pfl | Verpflichtender Grundpreis; Prosumer-Aufschlag von 70–90 % korrigiert den gesunkenen Finanzierungsbeitrag, ist aber ausdrücklich kein Verhaltensanreiz. |
| [IE]({{< ref "themen/variable-tarife/international/einspeiseentgelte.md#irland" >}}) | GTUoS – Einspeisenetzentgelt (\> 5 MW) | NE-Ein | Stat-OV | KP | IR | Pfl | Pauschalanteil ≥ 70 %, standortabhängiger Anteil ≤ 30 %, jährlich angepasst; Freibetrag von 5 MW für alle Erzeuger. Ziel ist die Standortwahl, nicht der Betrieb. |
| [UK]({{< ref "themen/variable-tarife/international/einspeiseentgelte.md#grossbritannien" >}}) | TNUoS – Einspeisenetzentgelt (Übertragungsnetz) | NE-Ein | Stat-OV | KP | IR | Pfl | 27 Erzeugungszonen (Wider Tariff) plus lokale Komponenten, £/kW auf Basis der kontrahierten TEC; Freigrenzen schließen kleine dezentrale Anlagen aus. |
| [RO]({{< ref "themen/variable-tarife/international/einspeiseentgelte.md#rumaenien" >}}) | Einspeisenetzentgelt (\> 5 MW, Verteilnetz) | NE-Ein | Stat-OV | AP | IR | Pfl | Acht Netzregionen, Erhebung nur in Regionen mit Erzeugungsüberschuss (2025: zwei von acht), Höhe 6 % bzw. 17 % der jeweiligen Entnahmeentgelte. |
| [AT]({{< ref "themen/variable-tarife/oesterreich.md" >}}) | [SNAP / WiNAP]({{< ref "themen/variable-tarife/oesterreich/netzentgelte.md#zeitvariable-nne" >}}) | NE-Bez | Stat-ZV | AP | LV | Pfl | Sommer 10–16 Uhr auf 80 % des Basiswerts, Winter 22–4 Uhr; gemeinsame Energienutzung im Nahebereich ist nach § 7 Abs. 5 SNE-GV-E ausgenommen. Im ElWG eig optional aber Praxis aktuell kein Wahlrecht (da nur vorteilig) |
| [AT]({{< ref "themen/variable-tarife/oesterreich.md" >}}) | [Netznutzungsentgelt-Reduktion im Nahebereich]({{< ref "themen/variable-tarife/oesterreich/netzentgelte.md#nahebereich" >}}) | NE-Bez | Stat-OV | AP | IR | Pfl | Für Energiegemeinschaften: Nach Lokal- bzw. Regionalbereich gestaffelte Reduktion des Arbeitspreises – örtliche Differenzierung ohne zeitliche Komponente. |
