---
title: "Spanien"
topics: []
authors: [afischer]
showSummary: true
weight: 1
series: ["Variable Tarife – International"]
series_order: 1
---

Spanien dient auf dieser Seite als eines von mehreren europäischen Beispielen für Tarifstrukturen, die sowohl die Arbeits- als auch den Leistungskomponente auf Energie und Netzseite zeitlich staffeln. Je nach vertraglich vereinbarter Anschlussleistung gelten unterschiedliche Netzentgelt-Tarife (2.0 TD bis 15 kW (siehe „[Tarif 2.0 TD](#tarif-2-0-td)“), 3.0 TD für 15–450 kW (siehe „[Tarif 3.0 TD](#tarif-3-0-td)“), 6.XTD für \>450 kW) mit unterschiedlichen Zeitfenstern. Ergänzend bietet der staatlich regulierte PVPC-Kleinverbrauchern einen dynamischen, aus Energiepreis, Netzentgelten und Abgaben kombinierten Gesamtstrompreis.

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Spanischer Netztarif bis 15 KW (Tarif 2.0 TD) {#tarif-2-0-td}

Die tarifa de acceso 2.0 TD ist der regulierte spanische Netzentgelt-Tarif (peaje de acceso) für Niederspannungsanschlüsse mit einer vertraglich vereinbarten Leistung bis 15 kW und legt ausschließlich das Entgelt für die Netznutzung fest. Er entstand am 1. Juni 2021 durch Zusammenlegung der bis dahin bestehenden Zugangstarife zu einer einheitlichen Struktur und gilt unabhängig vom gewählten Energiepreismodell.[^ide_tarif_2_0_td]

Die 2.0 TD gliedert sich in zwei unterschiedliche Komponenten, einen Arbeitspreis und Leistungsanteil, für den jeweils unterschiedliche Zeitfenster definiert sind. Der Arbeitspreis Netzentgeltanteil gliedert sich in drei ganzjährig fixe Verbrauchszeitzonen Valle (Valley), Llano (Off-Peak) und Punta (Peak), welche in [Abbildung 11](#abb-11) dargestellt sind.

![Abbildung 11 Überblick über Tariffenster der 2.0 TD Tarifs für die Arbeitspreiskomponente](/images/variable-tarife/international/abb-11.png)

<span id="abb-11"></span>*Abbildung 11 Überblick über Tariffenster der 2.0 TD Tarifs für die Arbeitspreiskomponente*

Zudem gibt es zwei Leistungspreis Zeitzonen (Punta-Llano und Valle), welche in [Tabelle 2](#tab-2) dargestellt sind. Die Bepreisung der Leistung findet dabei anhand der installierten Leistung statt und wird für die Niederspannungskunden im Normalfall über einen Leistungsbegrenzungsschalter begrenzt, der bei Überschreitung der kontrahierten Leistung auslöst und die Stromzufuhr kappt.[^voltiva_potencia] Für die Leistungskomponente können Kund:innen je Zeitfenster unterschiedliche Anschlussleistungen vertraglich vereinbaren, um die Fixkosten an das eigene Lastprofil anzupassen.

<span id="tab-2"></span>*Tabelle 2 Übersicht über Zeitfenster der Leistungspreises des 2.0 TD Tarifs in Spanien*

| Leistungszeitzone | Zeitraum |
|:---|:---|
| Punta-Llano (Peak & Off-Peak)<br>-\> höhere Leistungspreise | Werktags 08:00–24:00 Uhr |
| Valle (Valley)<br>-\> niedrigere Leistungspreise | Werktags 00:00–08:00 Uhr sowie Wochenenden und Feiertage |

Das staatlich regulierte Gesamtstrompreismodell PVPC (siehe „[PVPC](#pvpc)“) übernimmt die 2.0 TD unverändert als ihre Netzentgeltkomponente und kombiniert sie additiv mit dem dynamischen Energiepreis sowie den Systemumlagen (cargos).

## Spanischer Netztarif für 15-450 kW (3.0 TD) {#tarif-3-0-td}

Der Tarif 3.0 TD ist der spanische Netzentgelt-Tarif für Netzanschlüsse mit einer vertraglich vereinbarten Leistung zwischen 15 und 450 kW und damit die gängigste Struktur für KMU, Hotels, Supermärkte und Gewerbebetriebe. Im Unterschied zur 2.0 TD gliedert er sowohl den Arbeits- als auch den Leistungspreis in sechs Zeitzonen (P1–P6), wobei P1 die teuerste und P6 die günstigste Zone ist. Die genauen Zeitfenster variieren saisonal (Winter, Sommer, restliches Jahr) und sind in [Tabelle 3](#tab-3) dargestellt.

<span id="tab-3"></span>*Tabelle 3 Übersicht über Zeitfenster des spanischen T3.0 Tarifs der Netzentgelte für Energie & Leistungskomponente*

| Zeitzone | Relative Kosten | Winter (Nov.–Feb.) | Sommer (Jul.–Aug.) | Restliches Jahr |
|----|----|----|----|----|
| P1 (Punta) | am teuersten | 10:00–14:00 / 18:00–22:00 | 11:00–15:00 / 19:00–23:00 | nur in Hochsaison |
| P2 | hoch | 08:00–10:00 / 14:00–18:00 | 08:00–11:00 / 15:00–19:00 | 10:00–14:00 / 18:00–22:00 |
| P3 | mittelhoch | \- | \- | 08:00–10:00 / 14:00–18:00 |
| P4 | mittel | \- | \- | Samstage und landesweite Feiertage |
| P5 | mittelniedrig | Samstage und landesweite Feiertage | Samstage und landesweite Feiertage | — |
| P6 (Valle) | am günstigsten | 00:00–08:00 | 00:00–08:00 | 00:00–08:00 |

Zudem existiert für Anschlüsse mit einer Leistung über 450 kW die Tarifgruppe 6.XTD, die sich an Großverbraucher, die Schwerindustrie und Unternehmen mit hohem Energiebedarf richtet und je nach Spannungsebene die Subtarife 6.1TD bis 6.4TD umfasst.[^eleia_tarifas_2026] Er wird im Rahmen dieser Übersicht nicht weiter ausgeführt, da sie im Kontext von Energiegemeinschaften nicht relevant ist.

## Staatlich reguliertes Gesamtstrompreismodell für Kleinverbraucher \<10kW (PVPC) {#pvpc}

Der PVPC (Precio Voluntario para el Pequeño Consumidor) ist ein optionaler staatlich regulierter spanische Stromtarif für Kleinverbraucher (Haushalte und Kleinstunternehmen mit Niederspannungsanschluss) und einer vertraglich vereinbarten Leistung bis 10 kW. Neben der Energiekomponente umfasst die PVPC additiv die regulierten Netzentgelte (peajes de acceso) und Systemumlagen (cargos), sowie einen Vertriebskostenanteil. Es handelt sich also um eine Kombination verschiedener Preisbestandteile (Netz, Energie & Abgaben) die in Richtung des Endkunden ein einheitliches Preissignal aufgebaut aus den beschriebenen Einzelkomponenten sendet. Der Tarif ist dynamisch: Der Preis bewegt sich in definierten Korridoren und richtet sich innerhalb dieser stundenscharf (seit September 2025 viertelstündlich) nach dem [Day-Ahead-]({{< ref "wissen/markt-day-ahead/index.md" >}}) und [Intraday-Großhandelsmarkt]({{< ref "wissen/markt-intraday/index.md" >}}) und seit 2024 fließen zusätzlich, mit steigendem Gewicht (2024: 25 %, 2025: 40 %, 2026: 55 %), Terminmarktpreise ein, um die Volatilität zu dämpfen.[^comparadorluz_pvpc] Die Preise werden täglich veröffentlicht[^esios_pvpc].

[^ide_tarif_2_0_td]: [Access tariff 2.0 TD<br>(i-de.es)](https://www.i-de.es/electric-distribution/access-tariff-2-0-td)
[^voltiva_potencia]: [Penalización por exceso de potencia eléctrica<br>(voltiva.energy)](https://voltiva.energy/penalizacion-por-exceso-de-potencia-electrica-que-es-y-cuando-se-da/)
[^eleia_tarifas_2026]: [Tarifas de luz para empresas en España 2026<br>(eleiaenergia.com)](https://eleiaenergia.com/tarifas-luz-empresas-espana-2026/)
[^comparadorluz_pvpc]: [Tarifa PVPC<br>(comparadorluz.com)](https://comparadorluz.com/tarifas/pvpc)
[^esios_pvpc]: [PVPC<br>(esios.ree.es)](https://www.esios.ree.es/en/pvpc)
