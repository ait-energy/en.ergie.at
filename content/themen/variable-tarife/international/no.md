---
title: "Norwegen"
topics: []
authors: [afischer]
showSummary: true
weight: 3
series: ["Variable Tarife – International"]
series_order: 3
---

Seit 1. Juli 2022 müssen alle norwegischen Verteilnetzbetreiber für Haushalte einen kapazitätsbasierten Netztarif anwenden. Ziel der Reform war es, Anreize zur [Reduktion von Lastspitzen]({{< ref "wissen/peakshaving/index.md" >}}) zu schaffen und damit den Netzausbau effizienter zu gestalten[^nve_tariffs].

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

Ein Haushalts-Netztarif besteht typischerweise aus zwei Komponenten:

1.  <mark>Leistungskomponente (capacity charge / fastledd)</mark>

    - Die monatliche Gebühr richtet sich nach der durchschnittlichen Leistung der drei höchsten Tageslastspitzen (jeweils höchste Stundenleistung eines Tages) innerhalb eines Monats.

    - Daraus ergibt sich eine Zuordnung zu einer Leistungsstufe (capacity step), für die ein fixer Monatsbetrag bezahlt wird.

2.  <mark>Arbeitspreis (energy charge / energiledd)</mark>

    - Zusätzlich wird ein Arbeitspreis in NOK/kWh verrechnet.

    - Viele DSOs unterscheiden zwischen

      - Tag (werktags 06:00–22:00) und

      - Nacht & Wochenende,\
        sodass nachts und am Wochenende ein geringerer Arbeitspreis anfällt. Dies ist jedoch keine landesweit einheitliche Tarifhöhe, sondern wird vom jeweiligen DSO festgelegt. Die Regulierung erlaubt eine zeitliche Differenzierung; die konkrete Ausgestaltung liegt beim Netzbetreiber.

## Beispiel: Elvia (größter DSO Norwegens, gültig ab 1. Juli 2026) {#elvia}

<span id="tab-7"></span>*Tabelle 7: Leistungspreise (brutto) des Verteilernetzbetreibers Elvia für Privatkund:innen in Norwegen 2026 [^elvia_2026].*

| Durchschnit der drei höchsten Tagesmaxima | Monatliche Kapazitätsgebühr |
|:--:|:--:|
| 0–2 kW | 150 NOK/Monat (ca. 12,8 €/Monat) |
| 2–5 kW | 250 NOK/Monat (ca. 21,2 €/Monat) |
| 5–10 kW | 420 NOK/Monat (ca. 35,7 €/Monat) |
| 10–15 kW | 585 NOK/Monat (ca. 49,7 €/Monat) |
| 15–20 kW | 755 NOK/Monat (ca. 64,2 €/Monat) |

<mark>Zusätzlich gilt ein zeitabhängiger Arbeitspreis:</mark>

- Tag (06:00–22:00): 46,60 øre/kWh (ca. 4,0 €ct/kWh)

- Nacht & Wochenende: 31,40 øre/kWh (ca. 2,7 €ct/kWh)[^elvia_abgaben]

Die Zuordnung zur Leistungsstufe erfolgt anhand des Durchschnitts der drei höchsten Stundenlasten an drei verschiedenen Tagen innerhalb eines Monats[^elvia_leistungsstufe].

[^nve_tariffs]: [Network tariffs<br>(nve.no)](https://www.nve.no/norwegian-energy-regulatory-authority/network-regulation/network-tariffs/), [Grid rent prices for private customers<br>(elvia.no)](https://www.elvia.no/english/grid-rent-prices-for-private-customers/), [arXiv:2307.07580<br>(arxiv.org)](https://arxiv.org/abs/2307.07580)
[^elvia_2026]: [Ny pris for privatkunder fra 1. juli 2026<br>(elvia.no)](https://www.elvia.no/nettleie/alt-om-nettleiepriser/ny-pris-for-privatkunder-fra-1.-juli-2026)
[^elvia_abgaben]: Die Tarife verstehen sich inklusive aller Abgaben: Gesetzlich vorgeschriebener Beitrag zum Energiefonds (Enova): 1,0 Øre/kWh, Stromsteuer (Elavgift): 7,13 Øre/kWh und 25 % Mehrwertsteuer.
[^elvia_leistungsstufe]: [Grid rent prices for private customers<br>(elvia.no)](https://www.elvia.no/english/grid-rent-prices-for-private-customers/), [Ny pris for privatkunder fra 1. juli 2026<br>(elvia.no)](https://www.elvia.no/nettleie/alt-om-nettleiepriser/ny-pris-for-privatkunder-fra-1.-juli-2026)
