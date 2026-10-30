---
title: "Energiepreise für Endkund:innen"
topics: []
authors: [afischer]
showSummary: true
weight: 1
series: ["Variable Tarife – Österreich"]
series_order: 1
summary: "Wie Energiepreise für Endkund:innen gestaltet sind, wie verbreitet dynamische Energiepreise in Österreich sind und wie sich die Großhandelspreise entwickelt haben."
---

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Zusammensetzung und Design {#zusammensetzung}

Der Energiepreis ist der Preis für den Strom selbst und der einzige Block, dessen Preis im Wettbewerb gebildet wird. Der Stromlieferant kann den Strom selbst erzeugen oder ihn extern beschaffen (typischerweise über Großhandelsmärkte). Während der Lieferant an den Strombörsen den marktwirtschaftlich gebildeten Preis des Marktintervalls zahlt (aktuell am Spotmarkt viertelstündlich), hat er bei der Weitergabe an Endkund:innen einen breiten Gestaltungsspielraum. Der Endkundenpreis wird vom Lieferanten so kalkuliert, dass neben den Energiebeschaffungskosten sämtliche weiteren Kostenkomponenten vollständig abgedeckt sind (darunter Fixkosten, Marge, Risikoausgleich für Preisschwankungen, sowie Kosten für Ausgleichsenergie). Im Status Quo überwiegen im Endkundenbereich statische Preismodelle.

§ 22 ElWG verpflichtet Lieferanten mit mehr als 25.000 Zählpunkten, einen Liefervertrag mit dynamischen Energiepreisen anzubieten. Dabei müssen die Preise die Entwicklungen auf den Spotmärkten – zumindest am [Day-Ahead-Markt]({{< ref "wissen/markt-day-ahead/index.md" >}}) – in den jeweiligen stündlichen oder viertelstündlichen Abrechnungsintervallen widerspiegeln.

Die folgende Übersicht stellt die typischen Konzepte des arbeitsbezogenen Bestandteils der Lieferantenverträge dar, welche oftmals durch weitere Elemente wie eine Grundgebühr ergänzt werden.

<span id="tab-1"></span>*Tabelle 1 Übersicht über arbeitsbezogene Bestandteil der Energiekomponente*

| Art | Beschreibung |
|----|----|
| Fixer Strompreis | Endkund:in zahlt über den Vertragszeitraum einen fixierten, konstanten Preis je verbrauchter Kilowattstunde. Kund:in trägt kein Marktpreisrisiko und profitiert von maximaler Planungssicherheit. |
| Strommarkt-gekoppelt | Der Energiepreis orientiert sich unmittelbar am Großhandels-Spotmarkt oder Futures-Markt. Die zeitliche Granularität der Preisanpassung ist dabei frei gestaltbar, von sehr kurzfristigen Intervallen bis hin zu saisonalen Zeiträumen und ermöglicht Kund:innen durch Lastverschiebungen von günstigeren Preisfenstern zu profitieren:<br>• Viertelstündlich / stündlich: Preise folgen dem Day-Ahead-Markt<br>• Täglich / wöchentlich: z. B. über Peak/Off-Peak Zeiträume oder definierte Tagesabschnitte[^evn_garant_sonnenstrom]<br>• Monatlich: Orientierung an Vormonatspreisen oder Börsenfutures (z. B. EEX Month Futures)[^evn_aktiv_strom]<br>• Saisonal / jährlich: Preisanpassung auf Basis längerfristiger Marktentwicklungen / Erwartungen |
| Weitere Ausgestaltungen | • Stromtarife mit Mengenschwellen z.B. Wärmepumpentarife, in denen bei einem Verbrauchsschwellwert (z.B. 3500[^kelag_vorteilstarife] oder 4000[^esteiermark_waerme] kWh) der Preis sinkt<br>• Spotmarktgekoppelte Stromtarife mit Risikoabsicherung: Stromtarife, bei denen Preissignale dynamisch sind, jedoch Komponenten zur Risikoabsicherung wie ein Höchstpreis (z.B. 60 ct/kWh[^salzburgag_flexspot]) definiert sind<br>• Weitere Ausgestaltungen sind möglich |

Die Beschriebenen Energiepreiskomponenten können dabei sowohl auf der Bezugs-, als auch auf der Einspeiseseite angewendet werden.

## Verbreitung dynamischer Energiepreise {#verbreitung}

Nach § 22 ElWG sind Lieferanten mit mehr als 25.000 Zählpunkten verpflichtet, einen Liefervertrag mit dynamischen Energiepreisen anzubieten (vgl. „[Zusammensetzung und Design](#zusammensetzung)“). Wie viele Haushalte dieses Angebot aktuell tatsächlich nutzen, ist für Österreich jedoch nicht exakt dokumentiert. Einen vergangene Datenpunkt liefert der ACER Market Monitoring Report 2024, wie [Abbildung 2](#abb-2) zeigt, mit 6% für dynamischen Tarif und 11% monatlich zeitvariable Tarifen[^acer_mmr_retail_2024], womit sich Österreich im Ländervergleich im oberen Mittelfeld positioniert. Eine für Österreich repräsentative Erhebung zu Bekanntheit von und Einstellungen gegenüber dynamischen Energiepreisen liefern El Gohary et al. auf Basis einer Online-Befragung vom November 2023 (n = 1.067).[^el_gohary_2026] Wie [Abbildung 4](#abb-4) (links) zeigt, gaben 5,2 % an bereits einen dynamischen Vertrag zu haben, was sich also in der Größenordnung mit dem ACER Bericht deckt.

![Abbildung 2 Anteil der Haushaltsverträge für Strompreise in den EU Mitgliedstatten und EEA Mitgliedern Norwegen und GB](/images/variable-tarife/oesterreich/abb-02.png)

<span id="abb-2"></span>*Abbildung 2 Anteil der Haushaltsverträge für Strompreise in den EU Mitgliedstatten und EEA Mitgliedern Norwegen und GB*

### Bekanntheit dynamischer Preise {#bekanntheit}

Die Studie von El Gohary et al liefert darüber hinaus Einblicke in die österreichische Bevölkerung und Themen im Kontext dynamischer Tarife (dynamisch wie in Abschnitt „[Zeitliche Differenzierung]({{< ref "themen/variable-tarife/grundlagen.md#zeitliche-differenzierung" >}})“ definiert, also zeitvariable nicht einbezogen[^befragung_definition]). Wie [Abbildung 3](#abb-3) zeigt, hatten 47,3 % der Befragten noch nie von dynamischen Preisen gehört, weitere 40,1 % hatten zwar davon gehört, fühlten sich aber nicht gut informiert, und lediglich 12,6 % schätzten sich als gut informiert ein. Dies lässt vermuten, dass mangelnde Bekanntheit eine signifikante Barriere in der Verbreitung dieser dynamischen Tarife ist.[^el_gohary_2026]

![Abbildung 3 Bekanntheit dynamischer Preise in Österreich, Befragung November 2023 (n = 1.067)](/images/variable-tarife/oesterreich/abb-03.png)

<span id="abb-3"></span>*Abbildung 3 Bekanntheit dynamischer Preise in Österreich, Befragung November 2023 (n = 1.067)[^el_gohary_2026]*

### Haltung gegenüber dynamischen Preisen {#haltung}

[Abbildung 4](#abb-4) (links) zeigt: Neben den 5,2 %, die bereits einen dynamischen Vertrag haben, planten weitere 2,8 % einen baldigen Wechsel, und 6,2 % würden gerne einen dynamischen Vertrag abschließen, verfügten jedoch über keinen Smart Meter und 22,6% geben an es in der Zukunft in Betracht zu ziehen. Die größte Gruppe bilden mit 45,1 % jene Befragten, die nach eigener Angabe zu wenig Informationen für eine Entscheidung haben. Für 16,0 % kommt ein dynamischer Vertrag nicht in Frage. Zusammengefasst ([Abbildung 4](#abb-4), rechts) stehen 14,3 % der Befragten dynamischen Preisen positiv und 16,5 % ablehnend gegenüber, während 69,1 % eine ambivalente Haltung einnehmen.

![Abbildung 4 Haltung (links) und Grundeinstellung (rechts) gegenüber dynamischen Preisen in Österreich, Befragung November 2023 (n = 1.067)](/images/variable-tarife/oesterreich/abb-04.png)

<span id="abb-4"></span>*Abbildung 4 Haltung (links) und Grundeinstellung (rechts) gegenüber dynamischen Preisen in Österreich, Befragung November 2023 (n = 1.067)[^el_gohary_2026]*

Wie [Abbildung 5](#abb-5) zeigt, hängt die Haltung gegenüber dynamischen Preisen deutlich vom Informationsstand ab. Mit steigender Bekanntheit sinkt der Anteil Unentschlossener: von 82,5 % bei Personen, die noch nie davon gehört haben, über 64,5 % bei schlecht Informierten auf 34,1 % bei gut Informierten. Das Verhältnis von Zustimmung zu Ablehnung bleibt dabei in allen drei Gruppen ähnlich, mit einem leichten Überhang einer ablehnenden Haltung.

![Abbildung 5 Grundeinstellung gegenüber dynamischen Preisen nach Bekanntheitsgrad, Befragung November 2023 (n = 1.046)](/images/variable-tarife/oesterreich/abb-05.png)

<span id="abb-5"></span>*Abbildung 5 Grundeinstellung gegenüber dynamischen Preisen nach Bekanntheitsgrad, Befragung November 2023 (n = 1.046)[^el_gohary_2026]*

### Einordnung {#einordnung}

Daraus lässt sich ableiten, dass dynamische Energiepreise in Österreich nach den verfügbaren Daten bislang ein Nischenprodukt sind und ein Großteil der Bevölkerung wenig mit ihnen vertraut ist. Da der Anteil der Befürworter:innen mit der Bekanntheit steigt, ist davon auszugehen, dass eine höhere Bekanntheit tendenziell auch zu einer stärkeren Verbreitung dynamischer Tarife beiträgt, auch wenn zugleich die Ablehnung zunimmt. Für Energiegemeinschaften ist anzunehmen, dass das Bewusstsein für Energiethemen und die Möglichkeiten, auf Preissignale zu reagieren, bei Personen, die sich aktiv für eine Teilnahme entscheiden, höher sind als in der Durchschnittsbevölkerung. Dadurch könnten dynamische Energiepreise bei Energiegemeinschaftsteilnehmern potenziell weiterverbreitet sein als im Durchschnitt, was die Relevanz dynamischer Tarife für Energiegemeinschaften stärken könnte, in den genannten Studien aber nicht betrachtet wurde. Welche weiteren Faktoren, etwa wahrgenommene Vorteile und Risiken, Vorhersehbarkeit, verfügbare Flexibilität und soziale Rahmenbedingungen, Akzeptanz und Wechselbereitschaft beeinflussen, wird in Abschnitt „[Akzeptanz, Reaktion und Wechselbereitschaft]({{< ref "themen/variable-tarife/akzeptanz.md" >}})“ vertieft.

## Entwicklung der Preise auf Großhandelsmärkten {#grosshandel}

Zeitvariable und dynamische Energiepreismodelle sind, wie in Abschnitt „[Zusammensetzung und Design](#zusammensetzung)“ beschrieben, in aller Regel an die Entwicklung der Großhandelsmärkte gekoppelt. Im Folgenden wird daher deren Entwicklung der vergangenen Jahre dargestellt. Neben dem Einfluss des Erneuerbaren Ausbaus haben insbesondere geopolitische Ereignisse wie die russische Vollinvasion der Ukraine ab 2022 und der Iran-Krieg 2026 für erhebliche Unruhe an den Energiemärkten gesorgt: Sie führten zu einem strukturell höheren Preisniveau der häufig [preissetzenden]({{< ref "wissen/merit order/index.md" >}}) fossilen Kraftwerke, sowie zu einer erhöhten Preisvolatilität, die sich unmittelbar auch in zeitvariablen und dynamischen Preismodellen widerspiegelt.

### Preisniveau und Preisspreads {#preisniveau}

[Abbildung 6](#abb-6) zeigt die jährliche Verteilung der Day-Ahead-Preise in Österreich (EPEX-Spot) und veranschaulicht den beschriebenen Anstieg des Preisniveaus sowie der Preisstreuung seit 2021.

![Abbildung 6 Verteilung der Day-ahead Preise Österreich (EPEX-Spot)](/images/variable-tarife/oesterreich/abb-06.svg)

<span id="abb-6"></span>*Abbildung 6 Verteilung der Day-ahead Preise Österreich (EPEX-Spot)*

Ergänzend zeigt [Abbildung 7](#abb-7) die Verteilung der täglichen Day-Ahead-Spreads (Differenz zwischen täglichem Maximal- und Minimalpreis) und bestätigt seit 2021 deutlich erhöhte Preisspreads auf einem insgesamt merklich höheren Niveau als in den Jahren davor.

![Abbildung 7 Verteilung Day Ahead Spreads (Differenz zwischen täglichem Max/Min)](/images/variable-tarife/oesterreich/abb-07.png)

<span id="abb-7"></span>*Abbildung 7 Verteilung Day Ahead Spreads (Differenz zwischen täglichem Max/Min)*

### Negative Preise {#negative-preise}

[Abbildung 8](#abb-8) zeigt die Anzahl der Stunden mit negativen Preisen im Jahresvergleich: Nach einem bereits zwischen 2017 und 2020 zu beobachtenden Anstieg kam es während der geopolitisch bedingten Energiekrisenjahre 2021/2022 zunächst zu einem Rückgang, bevor die Anzahl seit 2022 wieder deutlich zunahm.

![Abbildung 8 Anzahl Stunden mit negativen Preisen – Jahresvergleich](/images/variable-tarife/oesterreich/abb-08.png)

<span id="abb-8"></span>*Abbildung 8 Anzahl Stunden mit negativen Preisen – Jahresvergleich*

[Abbildung 9](#abb-9) zeigt zudem, dass negative Preise vor allem in den Sommermonaten auftreten, was nahelegt, dass diese primär durch eine hohe PV-Einspeisung verursacht werden.

![Abbildung 9 Anzahl Stunden mit negativen Preisen – Monatsvergleich](/images/variable-tarife/oesterreich/abb-09.png)

<span id="abb-9"></span>*Abbildung 9 Anzahl Stunden mit negativen Preisen – Monatsvergleich*

### Bedeutung für Energiegemeinschaften {#bedeutung-eg}

Insbesondere die Niedrigpreisstunden mit stark negativen oder nahe null liegenden Großhandelspreisen stehen damit in unmittelbarer Konkurrenz zum EG-internen Verrechnungspreis: Für Mitglieder einer [Energiegemeinschaft]({{< ref "wissen/energiegemeinschaften/index.md" >}}) kann der Bezug am freien Markt in diesen Stunden günstiger sein als der interne Tarif, was eine Abstimmung zwischen Großhandelspreisentwicklung und EG-interner Tarifgestaltung erforderlich macht (vgl. Abschnitt „[Energiegemeinschaften und interne Tarife]({{< ref "themen/variable-tarife/oesterreich/energiegemeinschaften.md" >}})“). Dies ist insbesondere der Fall, wenn zusätzlich ein zeitvariabler oder dynamischer Netztarif angewandt wird der in diesen Stunden potenziellen Netzbezug begünstigt, weshalb die Netzkomponente im folgenden Abschnitt „[Netzentgelte]({{< ref "themen/variable-tarife/oesterreich/netzentgelte.md" >}})“ genauer betrachtet wird.

[^evn_garant_sonnenstrom]: Z.B. [Optima Garant Sonnenstrom<br>(evn.at)](https://www.evn.at/home/strom/optimagarantsonnestrom)
[^evn_aktiv_strom]: Z.B. [Optima Aktiv Strom<br>(evn.at)](https://www.evn.at/home/strom/optimaaktivstrom)
[^kelag_vorteilstarife]: [Neue, günstigere Vorteilstarife für Kelag-Kunden in Kärnten ab 1. April 2024<br>(kelag.at)](https://presse.kelag.at/news-neue-guenstigere-vorteilstarife-fuer-kelag-kunden-in-kaernten-ab-1-april-2024?id=192970&l=deutsch&menueid=27565)
[^esteiermark_waerme]: [Tarifblatt Privatkunden SteirerStrom Wärme<br>(e-steiermark.com)](https://www.e-steiermark.com/fileadmin/user_upload/downloads/E-Steiermark_Tarifblatt_Privatkunden_SteirerStrom_Waerme.pdf)
[^salzburgag_flexspot]: [Strom FlexSpot<br>(salzburg-ag.at)](https://www.salzburg-ag.at/strom/privat/stromprodukte/strom-flexspot.html)
[^acer_mmr_retail_2024]: [ACER-CEER Market Monitoring Report 2024 – Retail<br>(acer.europa.eu)](https://www.acer.europa.eu/sites/default/files/documents/Publications/ACER-CEER_2024_MMR_Retail.pdf)
[^el_gohary_2026]: [Reluctant to respond: Public attitudes towards dynamic pricing in Austria<br>(El Gohary et al., 2026)](https://doi.org/10.1016/j.enpol.2026.115328)
[^befragung_definition]: Für die Frage nach der Haltung gegenüber dynamischen Preisen wurden diese den Befragten als Preise beschrieben, die sich stündlich oder viertelstündlich ändern können; dies entspricht der Definition „dynamisch“ im Abschnitt „[Zeitliche Differenzierung]({{< ref "themen/variable-tarife/grundlagen.md#zeitliche-differenzierung" >}})“, statisch-zeitvariable Modelle fallen nicht unter diese Beschreibung)
