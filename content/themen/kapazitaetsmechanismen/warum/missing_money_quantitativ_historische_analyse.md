---
title: "Missing Money - Quantitativ-Historische Analyse"
topics: []
authors: ["afischer"]
---

## 1. Kernfragestellung und methodischer Ansatz

Der folgende Abschnitt beschäftigt sich mit der Frage, ob bestehende und neue Kraftwerkskapazitäten im Setting eines [Energy-Only-Marktes]({{< ref "wissen/markt-energy-only/index.md" >}}) ausreichend finanziert werden können. Ziel der Analyse ist somit ein "quantitativer Nachweis" des Missing Money Problems auf Basis historischer Jahre für Österreich. Dazu wurden folgende Kraftwerkstechnologien untersucht:

- Gas- und Dampfkraftwerk Wasserstoff (GuD Wasserstoff)
- Gas- und Dampfkraftwerk Erdgas (GuD Erdgas)
- Gasturbine Wasserstoff (GT Wasserstoff)
- Gasturbine Erdgas (GT Erdgas)
- Pumpspeicherkraftwerk
- Laufwasserkraft (klein)
- Photovoltaik
- Windkraft (Onshore)

Zur Beurteilung der Wirtschaftlichkeit wurden die gesamten Kosten (variable und fixe Kosten der Erzeugung auf Basis historischer Marktdaten und Kostenannahmen) den Erlösen (Kraftwerkseinsatz zu Marktpreisen) gegenübergestellt. Um die Unsicherheit 
in den Annahmen zu berücksichtigen, wurde eine Monte Carlo Simulation durchgeführt, der eine Normalverteilung zugrunde 
gelegt wurde. Mittels der normalverteilten Monte Carlo Simulation wurde die Höhe der gewählten Parameter (OPEX, CPAEX, FOM
VOM, WACC, Effizienz, Lebensdauer und Wasserstoffpreis) innerhalb einer Spannweite (niedrig - hoch) variiert und dadurch
in Summe 20.000 Szenarien generiert.

### Kraftwerkseinsatz
Zur Modellierung des stündlichen Kraftwerkseinsatzes wurden zwei verschiedene Ansätze verfolgt. Einerseits
ein historischer Ansatz, bei dem die historischen Erzeugungsprofile für Österreich laut
<abbr title="European Network of Transmission System Operators for Electricity">ENTSO-E</abbr>
Transparency Platform[^1] herangezogen wurden. Andererseits wurde ein theoretischer Ansatz gewählt, bei dem der
Kraftwerkseinsatz auf Basis von wirtschaftlichen Kriterien erfolgt. Dabei erfolgt der Einsatz eines Kraftwerks, sobald der
historische Strompreis oberhalb der unterstellten Grenzkosten liegt.

Der theoretische Kraftwerkseinsatz wurde hierbei nur für die thermischen Kraftwerke (GuD Erdgas & Wasserstoff, GT Erdgas
& Wasserstoff) bestimmt, da davon auszugehen ist, dass die Erzeugungsanlagen basierend auf den erneuerbaren Energien
(Wind, Solar, Wasserkraft) bereits durch
ihre Verfügbarkeit beschränkt sind und somit in einer theoretischen Betrachtung keinen stark veränderten Kraftwerkseinsatz
aufweisen. Tabelle **x** gibt einen Überblick welche Technologien in der historischen und theoretischen Analyse betrachtet wurden.

| Historischer Ansatz | Theoretischer Ansatz |
|---------------------|----------------------|
| Erdgas              | GuD Wasserstoff      |
| PV                  | GuD Erdgas           |
| Windkraft           | GT Wasserstoff       |
| Laufwasserkraft (klein)    | GT Erdgas            |
| Pumpspeicher        |            -         |

Die Grenzkosten setzten sich zusammen
aus der Summe von variablen Betriebs- und Instandhaltungskosten 
<abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> (siehe Tabelle 1) und variablen
Brennstoffkosten:

Grenzkosten = Variable <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> Kosten + Variable Brennstoffkosten

Die variablen Brennstoffkosten ergeben sich auf Basis von Effizienz, Preis des Brennstoffes, CO<sub>2</sub>-Intensität und Preis für CO<sub>2</sub>-Zertifikate:

<p>
  Variable Brennstoffkosten =
  <span style="display: inline-block; vertical-align: middle;">
    <span style="display: block; text-align: center;">
      Brennstoffpreis + CO₂ Preis × CO₂ Intensität
    </span>
    <span style="display: block; border-top: 1px solid #000; text-align: center;">
      Effizienz
    </span>
  </span>
</p>

Bei der theoretischen Betrachtung wurde ein optimaler Kraftwerkseinsatz unterstellt, d.h. sobald der Strompreis die Grenzkosten übersteigt, erzeugt das Kraftwerk mit der vollen Kapazität. Wenn der Strompreis unterhalb der Grenzkosten liegt, erfolgt kein Kraftwerkseinsatz. Es wird somit ideale Flexibilität unterstellt und auf die Berücksichtigung von Rampen sowie minimal, erforderliche Einspeiseleistung verzichtet. Die Analyse erfolgt auf historischer Basis für die Jahre 2019-2024.

## 2. Annahmen und Eingangsgrößen

### Preisentwicklung

Zur Entwicklung der Strompreise wurden die stündlichen Werte der EPEX Spot [Day-ahead]({{< ref "wissen/markt-energy-only/index.md" >}}) 60-Minuten Auktion für Österreich herangezogen [^1]. 
Für die Ermittlung der Grenzkosten der jeweiligen Kraftwerke wurden die CH<sub>4</sub>-Preise von [investing.com](https://www.investing.com/commodities/dutch-ttf-gas-c1-futures-historical-data) und die CO<sub>2</sub>-Preise von [energy-charts.info](https://www.energy-charts.info/charts/price_spot_market/chart.htm?l=de&c=AT&legendItems=6w1&interval=year)
verwendet. Die täglichen CH<sub>4</sub>-Preise wurden auf Stundenbasis interpoliert und in einem weiteren Schritt wurden
alle Rohstoff- und Strompreise auf reale Werte für 2024 umgerechnet. Die Entwicklung der Rohstoff-, CO<sub>2</sub>- und Strompreise ist in Abbildung 1 dargestellt.

![Preisentwicklung Commodities und Strom](/images/missing_money_quantitativ_historische_analyse/preisentwicklung_commodities_und_strom.png)
*Abb. 1: Preisentwicklung Rohstoffe und Strom*

Abbildung 2 stellt den Zusammenhang zwischen Strompreisen und Grenzkosten auf monatlicher Basis dar. Es zeigt sich, dass der Strommarkt die Grenzkosten der Stromerzeugung auf Basis der Preise für Gas und Kohle sehr deutlich widerspiegelt. Der Strompreis folgt über weite Strecken den Grenzkosten und pendelt zwischen denen eines Gas- und Dampfkraftwerks und eines Kohlekraftwerks. Je nach Marktsituation (Verhältnis der Brennstoffpreise) bzw. Stromnachfrage entspricht der Strompreis tendenziell dem Minimum der Grenzkosten eines Gas- bzw. Kohlekraftwerks. Während im Jahr 2015 tendenziell Kohlekraftwerke den Preis setzen, entspricht der Strompreis seit Beginn 2019 tendenziell den Grenzkosten eines Gas- und Dampfkraftwerks.

![Zusammenhang Strompreis und Grenzkosten: monatlich](/images/missing_money_quantitativ_historische_analyse/zusammenhang_strompreis_und_grenzkosten_monatlich.png)
*Abb. 2: Zusammenhang Strompreis und Grenzkosten: monatlich*

### Investitions- und Betriebskosten, Inflation und technische Annahmen

Des Weiteren wurden generische Annahmen bezüglich der Investitions- und Betriebskosten der jeweiligen Kraftwerkstechnologie auf Basis der Fraunhofer Studie *Stromgestehungskosten Erneuerbarer Energien* [^5] herangezogen. Für die Laufwasser- und Pumpspeicherkraftwerke wurden Annahmen aus Status Bericht 2024 der Europäischen Kommission zu *Wasserkraft und Pumpspeicherkraftwerken in der Europäischen Union* herangezogen [^8]. 

<table>
  <caption style="caption-side: bottom; text-align: left;">
    <em>Tabelle 1: Quellenübersicht</em>
  </caption>
  <thead>
    <tr>
      <th>Technologie</th>
      <th>Quelle</th>
      <th>Anmerkung</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff</td>
      <td>Fraunhofer</td>
      <td></td>
    </tr>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas</td>
      <td>Fraunhofer</td>
      <td></td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Wasserstoff</td>
      <td>Fraunhofer</td>
      <td></td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Erdgas</td>
      <td>Fraunhofer</td>
      <td></td>
    </tr>
    <tr>
      <td>Pumpspeicherkraftwerk</td>
      <td>Europäische Kommission</td>
      <td>WACC von Windkraft übernommen, Mittlerer CAPEX ± 20 % für Werte hoch/niedrig</td>
    </tr>
    <tr>
      <td>Laufwasserkraftwerk (klein)</td>
      <td>Europäische Kommission</td>
      <td>WACC von Windkraft übernommen, Angegebene Spannbreite für CAPEX Werte hoch/niedrig übernommen</td>
    </tr>
    <tr>
      <td>Solar PV</td>
      <td>Fraunhofer</td>
      <td>Werte für PV Freiflächen ab 1000 kWp</td>
    </tr>
    <tr>
      <td>Windkraft</td>
      <td>Fraunhofer</td>
      <td>Werte für Wind Onshore</td>
    </tr>
  </tbody>
</table>

Um einen adäquaten Unsicherheitsbereich in die Analyse aufzunehmen, wurden sämtliche CAPEX Werte aus der Fraunhofer Studie [^5] für ‚hoch‘ und ‚niedrig‘ herangezogen. Für Laufwasserkraft und Pumpspeicher wurden die <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> Werte aus dem Status Bericht 2024 der Europäischen Kommission [^8] herangezogen, wobei für Laufwasserkraft die gesamte, angegebene Spannbreite für ‚hoch‘ und ‚niedrig‘ verwendet wurde, während für Pumpspeicherkraftwerke der mittlere <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> Wert um &#177; 20% variiert wurde.
Die fixen <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> Kosten wurden pro Technolgie als 1-3% der mittleren <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> angenommen, um Werte für ‚hoch‘ und niedrig zu erhalten.
Weiters wurden die durchschnittlichen <abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr> um -1/+3 %, und die variablen <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr>-Kosten um &#177;&nbsp;0.5 variiert. Eine Zusammenfassung der Werte ist in den Tabellen 2 und 3 dargestellt. Sämtliche Werte entsprechen realen Geldwerteinheiten 2024, der <abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr> ist in realen Einheiten zu verstehen.

<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <title>Tabelle 2: Annahmen zu Investitions- und Kapitalkosten</title>
  <style>
    :root {
      --divider: 2px solid #ccc;
    }
    table.grouped {
      border-collapse: collapse;
      width: 100%;
      font-family: sans-serif;
    }
    table.grouped th,
    table.grouped td {
      padding: 8px 12px;
      text-align: center;
    }
    /* Erste Spalte linksbündig */
    table.grouped th:first-child,
    table.grouped td:first-child {
      text-align: left;
    }
    /* Vertikale Linien über die gesamte Tabelle:
       - nach der ersten Spalte
       - vor der WACC-Spalte */
    table.grouped col.tech {
      border-right: var(--divider);
    }
    table.grouped col.wacc {
      border-left: var(--divider);
    }
  </style>
</head>
<body>

<table class="grouped">
  <caption style="caption-side: bottom; text-align: left; font-style: italic;">
    Tabelle 2: Annahmen zu Investitions- und Kapitalkosten
  </caption>

  <colgroup>
    <col class="tech">   <!-- Linie rechts nach Technologie -->
    <col>                <!-- CAPEX hoch -->
    <col>                <!-- CAPEX niedrig -->
    <col class="wacc">   <!-- Linie links vor WACC -->
    <col>                <!-- WACC niedrig -->
  </colgroup>

  <thead>
    <tr>
      <th rowspan="2">Technologie</th>
      <th colspan="2"><abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> [MEUR/MW]</th>
      <th colspan="2"><abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr> [%]</th>
    </tr>
    <tr>
      <th>hoch</th>
      <th>niedrig</th>
      <th>hoch</th>
      <th>niedrig</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff</td><td>2.40</td><td>1.10</td><td>9.9 %</td><td>5.9 %</td>
    </tr>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas</td>     <td>1.30</td><td>0.90</td><td>9.4 %</td><td>5.4 %</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Wasserstoff</td> <td>1.20</td><td>0.55</td><td>9.9 %</td><td>5.9 %</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Erdgas</td>      <td>0.70</td><td>0.45</td><td>9.4 %</td><td>5.4 %</td>
    </tr>
    <tr>
      <td>Pumpspeicher</td><td>3.0</td><td>2.0</td><td>6.9 %</td><td>2.9 %</td>
    </tr>
    <tr>
      <td>Laufwasserkraft (klein)</td>     <td>1.8</td><td>1.0</td><td>6.9 %</td><td>2.9 %</td>
    </tr>
    <tr>
      <td>PV</td>      <td>0.90</td><td>0.70</td><td>6.5 %</td><td>2.5 %</td>
    </tr>
    <tr>
      <td>Windkraft</td>     <td>1.90</td><td>1.30</td><td>6.9 %</td><td>2.9 %</td>
    </tr>
  </tbody>
</table>

</body>
</html>

<table class="grouped">
  <caption style="caption-side: bottom; text-align: left; font-style: italic;">
    Tabelle 3: Annahmen zu O&amp;M-Kosten
  </caption>

  <colgroup>
    <col class="tech">   <!-- Linie rechts nach Technologie -->
    <col>                <!-- Variable O&M hoch -->
    <col>                <!-- Variable O&M niedrig -->
    <col class="wacc">   <!-- Linie links vor Fixe O&M -->
    <col>                <!-- Fixe O&M niedrig -->
  </colgroup>

  <thead>
    <tr>
      <th rowspan="2">Technologie</th>
      <th colspan="2">Variable <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> [€/MWh]</th>
      <th colspan="2">Fixe <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> [€/kW/a]</th>
    </tr>
    <tr>
      <th>hoch</th>
      <th>niedrig</th>
      <th>hoch</th>
      <th>niedrig</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff</td><td>5.5</td><td>4.5</td><td>52.5</td><td>17.5</td>
    </tr>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas</td>     <td>5.5</td><td>4.5</td><td>33.0</td><td>11.0</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Wasserstoff</td> <td>5.5</td><td>4.5</td><td>26.3</td><td>8.8</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Erdgas</td>      <td>4.5</td><td>3.5</td><td>17.3</td><td>5.8</td>
    </tr>
    <tr>
      <td>Pumpspeicher</td><td>0.5</td><td>0.0</td><td>75.0</td><td>25.0</td>
    </tr>
    <tr>
      <td>Laufwasserkraft (klein)</td>     <td>0.5</td><td>0.0</td><td>42.0</td><td>14.0</td>
    </tr>
    <tr>
      <td>PV</td>      <td>0.5</td><td>0.0</td><td>24.0</td><td>8.0</td>
    </tr>
    <tr>
      <td>Windkraft</td>     <td>7.5</td><td>6.5</td><td>48.0</td><td>16.0</td>
    </tr>
  </tbody>
</table>

Tabelle 4 zeigt die Annahmen zur Effizienz und der Lebensdauer. Auch hier wurden die Werte der ursprünglichen Quellen um &#177;1% (Effizienz) variiert. Da es sich bei der Lebensdauer in den Quellen um die technische Lebensdauer handelt, wurde diese
als Wert ‚hoch‘ angenommen, und für den Wert ‚niedrig‘ um 1/6 reduziert, wodurch die oft kürzer ausfallende, finanzielle Lebensdauer berücksichtigt wird.

<table class="grouped">
  <caption style="caption-side: bottom; text-align: left; font-style: italic;">
    Tabelle 4: Annahmen zu Effizienz und Lebensdauer
  </caption>

  <colgroup>
    <col class="tech">   <!-- Linie rechts nach Technologie -->
    <col>                <!-- Effizienz hoch -->
    <col>                <!-- Effizienz niedrig -->
    <col class="wacc">   <!-- Linie links vor Lebensdauer -->
    <col>                <!-- Lebensdauer niedrig -->
  </colgroup>

  <thead>
    <tr>
      <th rowspan="2">Technologie</th>
      <th colspan="2">Effizienz [LHV]</th>
      <th colspan="2">Lebensdauer [Jahre]</th>
    </tr>
    <tr>
      <th>hoch</th>
      <th>niedrig</th>
      <th>hoch</th>
      <th>niedrig</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff</td><td>58 %</td><td>56 %</td><td>30</td><td>25</td>
    </tr>
    <tr>
      <td><abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas</td>     <td>58 %</td><td>56 %</td><td>30</td><td>25</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Wasserstoff</td> <td>41 %</td><td>39 %</td><td>30</td><td>25</td>
    </tr>
    <tr>
      <td><abbr title="Gasturbine">GT</abbr> Erdgas</td>      <td>41 %</td><td>39 %</td><td>30</td><td>25</td>
    </tr>
    <tr>
      <td>Pumpspeicher</td><td>100 %</td><td>100 %</td><td>50</td><td>42</td>
    </tr>
    <tr>
      <td>Laufwasserkraft (klein)</td>     <td>100 %</td><td>100 %</td><td>50</td><td>42</td>
    </tr>
    <tr>
      <td>PV</td>      <td>100 %</td><td>100 %</td><td>30</td><td>25</td>
    </tr>
    <tr>
      <td>Windkraft</td>     <td>100 %</td><td>100 %</td><td>25</td><td>21</td>
    </tr>
  </tbody>
</table>

Für Erdgas und CO<sub>2</sub> wurden die Preise auf Basis der historischen Zeitreihen (Abbildung 1) herangezogen. Für Wasserstoff wurden für alle Szenarien Werte wischen 3 - 9 €/kg<sub>H2</sub> angenommen, wobei diese Preise wiederum im Rahmen einer normalverteilten Monte Carlo Simulation variiert wurden. Um die Kreuzpreiselastizität der unterschiedlichen Brennstoffe in den Jahren der hohen Strompreise zu berücksichtigen, wurde der gezogene Wasserstoffpreis in jedem Szenario als untere Schranke herangezogen. Überstieg der stündliche Erdgaspreis den Wasserstoffpreis, so wurde in dieser Stunde der Erdgaspreis als Näherung für den Wasserstoffpreis angenommen.
<!--Aufgrund der Tatsache, dass nahezu alle Annahmen einer gewissen Unsicherheit unterliegen, wurden für alle Annahmen (mit Ausnahme der historischen Strom-, Brennstoff und CO<sub>2</sub> Kosten) entlang der Szenarien ‚hoch‘ und ‚niedrig‘ in einer plausiblen Bandbreite variiert. Für die Auswertung wurden sämtliche Szenario-Kombinationen herangezogen. Da es sieben Dimensionen (<abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr>, <abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr>; <abbr title="Variable Operations & Maintenance (variable Betriebskosten)">VOM</abbr>, <abbr title="Fixed Operations & Maintenance (fixe Betriebskosten)">FOM</abbr>, Effizienz, Lebensdauer und H<sub>2</sub>-Preise) in zwei Ausprägungen (hoch, niedrig) gibt, ergeben sich für jeden der neun Kraftwerkstypen 2<sup>7</sup> = 128 Kombinationsmöglichkeiten. Darüber hinaus wurden zehn historische Jahre (2015-2024) betrachtet, woraus sich 1.280 Beobachtungen für jeden Kraftwerkstyp ergeben. -->

Weiters wurde für die CO<sub>2</sub>-Intensität des Erdgases der <abbr title="Ten-year network development plan">TYNDP</abbr>-Wert für das Jahr 2030 herangezogen.
|                              | Erdgas  |
|------------------------------|------|
| CO<sub>2</sub>-Intensität (kg CO<sub>2</sub> / GJ) | 51.57 |
*Tabelle 5: CO<sub>2</sub>-Intensität*

Die nominalen Geldwerte hinsichtlich der Strom- und Brennstoffpreise wurden auf reale Werte 2024 angepasst, basierend auf den Inflationsdaten für Österreich laut des Harmonisierten Verbraucherpreisindex (<abbr title="Harmonised Index of Consumer Prices (harmonisierter Verbraucherpreisindex)">HICP</abbr>) von Eurostat[^7].

<table>
  <caption style="caption-side: bottom; text-align: left;">
    <em>Tabelle 6: Inflationsanpassung auf Basis des jährlichen (<abbr title="Harmonised Index of Consumer Prices (harmonisierter Verbraucherpreisindex)">HICP</abbr>) für Österreich laut (<abbr title="Harmonised Index of Consumer Prices (harmonisierter Verbraucherpreisindex)">HICP</abbr>) Eurostat</em>
  </caption>
  <thead>
    <tr>
      <th>Year</th><th>2015</th><th>2016</th><th>2017</th><th>2018</th><th>2019</th><th>2020</th><th>2021</th><th>2022</th><th>2023</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Index</td><td>1.34</td><td>1.33</td><td>1.30</td><td>1.27</td><td>1.25</td><td>1.24</td><td>1.20</td><td>1.11</td><td>1.03</td>
    </tr>
  </tbody>
</table>

## 3. Resultate

### Auslastung

Abbildung 3 zeigt den Kraftwerkseinsatz auf Jahresbasis für den theoretischen/historischen Ansatz. Zunächst ist evident, dass der theoretische Ansatz nicht mit den historischen Daten korrespondiert und zu deutlich abweichenden Ergebnissen führt. Während der theoretische Ansatz zu einer Auslastung von 30-40% für Gas und 40-80% für Kohle führt, ergibt sich im historischen Ansatz ein Einsatz von etwa 20-30%.

Das ist eine direkte Folge der impliziten idealen Flexibilität, die das modellierte Kraftwerk besitzt. In der theoretischen Betrachtung besteht keinerlei Einschränkung bezüglich Anfahrtsrampen. Das Kraftwerk kann somit voll flexibel agieren und den Deckungsbeitrag maximieren. In der Realität ist die Flexibilität stärker eingeschränkt, zumindest aufgrund technischer Limitationen bzgl. Startrampen (vor allem bei Kohle), aber auch aufgrund von Wärmelieferungsverpflichtungen.

![Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/jahrliche_kraftwerksauslastung_fur_kohlegud_fur_historischentheoretischen_kraftwerkseinsatz.png)
*Abb. 3: Jährliche Kraftwerksauslastung für alle Technologien im historischen/theoretischen Kraftwerkseinsatz*

Abbildung 5 stellt noch einmal den Kraftwerkseinsatz der beiden Ansätze auf stündlicher Ebene gegenüber. Daraus wird der Unterschied klar ersichtlich: das modellierte Kraftwerk agiert deutlich flexibler (und profitmaximierend) und kann somit einen deutlich höheren Deckungsbeitrag erwirtschaften. Die historischen Profile korrelieren durchaus mit der theoretisch optimalen Version, der Kraftwerkseinsatz fällt jedoch deutlich träger aus.

![Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/jahrliche_kraftwerksauslastung_fur_kohle_gud_fur_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 4: Jährliche Kraftwerksauslastung für Kohle/<abbr title="Gas- und Dampfkraftwerk">GuD</abbr> für historischen und theoretischen Kraftwerkseinsatz*

![Stündliche Kraftwerksauslastung für GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/stundliche_kraftwerksauslastung_fur_gud_fur_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 5: Stündliche Kraftwerksauslastung für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> für historischen/theoretischen Kraftwerkseinsatz*

### Wirtschaftlichkeit

Abbildung 6 zeigt die über alle Szenario-Kombinationen gemittelten Profite auf jährlicher Basis und stellt die Ergebnisse des theoretischen und historischen Kraftwerkseinsatzes gegenüber. Zunächst zeigt sich, dass die Profite über die Jahre stark schwanken, wobei das für alle Kraftwerkstypen gilt. Des Weiteren zeigt sich, dass nahezu alle Kraftwerkstypen bis 2021 Geld verloren haben. Mit Beginn der Energiekrise Ende 2021 bis in das Jahr 2024 sind die beobachtbaren Profite von <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas sowohl in der theoretischen als auch historischen Betrachtung merklich angestiegen. Erneuerbare Erzeugungstechnologien (Laufwasserkraft, Speicherwasserkraft, Solar PV und Wind) erlebten 2022 einen sprunghaften Anstieg der Profite bzw. eine Umkehr von Verlusten in Gewinne.

Zum einen ist ersichtlich, dass abseits der Jahre der Energiekrise (2021+2022) für keinen Kraftwerkstyp ausreichend Deckungsbeitrag erwirtschaftet werden konnte, um die laufenden Kosten zu decken. Zum anderen hatten die Jahre der Energiekrise (2021+2022) eine signifikant positive Auswirkung auf die Erlöse aller Kraftwerkstypen.

Abbildung 8 vergleicht direkt die Profite zwischen dem historischen und dem theoretischen Kraftwerkseinsatz für Kohle und <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas. Daraus zeigt, sich, dass die theoretische Betrachtung konsequent optimistischere Resultate liefert als sich aus den historisch beobachtbaren Einsatzzeiten ableiten lassen würde.

![Mittlere Profite über alle Szenarien auf Basis historischer Erzeugungsprofile](/images/missing_money_quantitativ_historische_analyse/mittlere_profite_uber_alle_szenarien_auf_basis_historischer_erzeugungsprofile.png)
*Abb. 6: Mittlere Profite über alle Szenarien auf Basis historischer Erzeugungsprofile*

![Mittlere Profite über alle Szenarien verglichen zwischen historischem und theoretischem Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/mittlere_profite_uber_alle_szenarien_verglichen_zwischen_historischem_und_theoretischem_kraftwerkseinsatz.png)
*Abb. 7: Mittlere Profite über alle Szenarien verglichen zwischen historischem und theoretischem Kraftwerkseinsatz*

Der Mittelwert der Profite über den gesamten Zeitraum (2015-2024) und alle Szenarien ist in Abbildung 7 dargestellt. Wenig überraschend zeigen sich die allermeisten Kraftwerkstypen im Durchschnitt verlustreich. Für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas ergibt sich in der historischen Betrachtungsweise ein ‚Missing Money‘ von etwa 80 €/kW, in der theoretischen Betrachtung ist die Technologie knapp kostendeckend. Wichtig zu beachten ist an dieser Stelle, dass es sich hier um eine Durchschnittsbetrachtung handelt, die zehn historische Jahre und 128 Szenario-Kombinationen umfasst. Die Schwankungsbreite dahinter ist durchaus groß und die Jahre der Energiekrise 2021-2023 stellen außerordentliche Ereignisse dar, die die Durchschnittsbetrachtung wesentlich verzerren.

![Mittlere Profite über alle Jahre und Szenarien in beiden Betrachtungsweisen](/images/missing_money_quantitativ_historische_analyse/mittlere_profite_uber_alle_jahre_und_szenarien_in_beiden_betrachtungsweisen.png)
*Abb. 8: Mittlere Profite über alle Jahre und Szenarien in beiden Betrachtungsweisen*

Abbildung 9 illustriert die Schwankungsbreite hinter den Durchschnittsergebnissen in Form von Boxplots. Während die Resultate für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas in der historischen Betrachtung zwischen -200 €/kW und 0 €/kW schwanken, bewegen sich die Profite in der theoretischen Betrachtung in 50% der Fälle zwischen -50 €/kW und +50 €/kW.

Für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff stellt sich die Sache noch volatiler und verlustreicher dar. In zumindest 75% der Fälle ergibt sich ein Verlust von mindestens 100 €/kW. Auf Basis der angenommenen Preise für Wasserstoff von 3 €/kg bzw. 6 €/kg ergibt sich ausschließlich in den Jahren 2021 und 2022 eine positive Auslastung. Aufgrund der äußerst hohen Strompreise in diesen Jahren ergibt sich jedoch ein günstiges Verhältnis zwischen Input- und Outputpreisen, wodurch sich hohe Gewinne ergeben.

Relativ robuste Ergebnisse zeigen sich für Solar PV: Hier ist die Schwankungsbreite äußerst gering, de-facto -50 bis + 50 €/kW in 90% der Fälle. 

Für die Interpretation an dieser Stelle ist jedoch erwähnenswert, dass die Bewertung auf Grundlage von geschätzten Investitionskosten im Jahr 2024 gegen historische Preise zwischen 2015 und 2024 erfolgt. Aufgrund der stark gefallenen Investitionskosten von Photovoltaik im vergangenen Jahrzehnt kann demnach nicht die Schlussfolgerung gezogen werden, dass bestehende Anlagen dieses Typs genau diese Profitabilität aufweisen.

Äußerst volatil stellt sich auch die Laufwasserkraft dar, da sie nicht nur preislichen Schwankungen sondern auch Schwankungen im Dargebot unterliegt. In den mittleren 50% der Fälle ergeben sich hier Gewinne bzw. Verluste zwischen -200 und +100 €/kW. Bei der Interpretation ist jedoch Vorsicht geboten, da auch hier historische Preise mit Investitionskosten aus dem Jahr 2024 gegenübergestellt werden. 

![Verteilung der Profite über alle Jahre und Szenarien in beiden Betrachtungsweisen](/images/missing_money_quantitativ_historische_analyse/verteilung_der_profite_uber_alle_jahre_und_szenarien_in_beiden_betrachtungsweisen.png)
*Abb. 9: Verteilung der Profite über alle Jahre und Szenarien in beiden Betrachtungsweisen*

Abbildung 10 stellt noch einmal die volle Schwankungsbreite und Größenordnung von Deckungsbeitrag und Fixkosten für alle Kraftwerkstypen und Kraftwerkseinsatzmodalitäten dar. Augenscheinlich ist dabei, dass der Deckungsbeitrag weitaus größeren Schwankungsbreiten ausgesetzt ist als die Kostenseite. Trotz Variation der Investitions- und Betriebskosten, <abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr> und Lebensdauer ergeben sich bei weitem nicht so hohe Schwankungsbreiten wie auf der Erlösseite. Dies spiegelt die hohe Volatilität im Strommarkt wider.

![Schwankungsbreite der Deckungsbeiträge und Fixkosten über alle Jahre, Szenarien und Betrachtungsweisen](/images/missing_money_quantitativ_historische_analyse/schwankungsbreite_der_deckungsbeitrage_und_fixkosten_uber_alle_jahre_szenarien_und_betrachtungsweisen.png)
*Abb. 10: Schwankungsbreite der Deckungsbeiträge und Fixkosten über alle Jahre, Szenarien und Betrachtungsweisen*

In Bezug auf ‚Missing Money‘ können daher folgende Schlussfolgerungen abgeleitet werden:
-	Ein erdgasbasiertes Gas- und Dampfkraftwerk kann auf Basis der letzten 10 Jahre unter idealen Bedingungen annähernd kostendeckend betrieben werden. Die Aussagekraft hängt jedoch stark an der betrachteten Zeitperiode (2015-2024) und den zugrundeliegenden Annahmen über vollständig flexiblen Kraftwerkseinsatz. Auf Basis der historischen Erzeugungsprofile kann diese Aussage nicht gestützt werden
-	Ein Kohlekraftwerk wäre wirtschaftlich darstellbar, die Fixkosten könnten rein auf Basis der Markterlöse abgedeckt werden
-	Der Betrieb einer Gasturbine ist auf Basis der Markterlöse nicht finanzierbar, es ergeben sich zu wenig Einsatzzeiten um ausreichend Deckungsbeitrag zu erwirtschaften

Mit einem Blick auf den zeitlichen Verlauf der Erlöse (Abbildung 6) relativieren sich daher die zuvor getroffenen Aussagen bezüglich der Rentabilität von Kraftwerkstypen stark. Unter Ausschluss der Jahre 2021 und 2022 wird auch für das Kohlekraftwerk ein wirtschaftlicher marktbasierter Betrieb unmöglich und das ‚Missing Money‘ für die gasbasierten Technologien deutlich größer.

## 4. Schlussfolgerungen

Zusammenfassend lassen sich folgende Kernaussagen treffen
- Auf Basis der historischen Preisentwicklung ergeben sich keine starken Investitionsanreize in <abbr title="Gas- und Dampfkraftwerk">GuD</abbr>, Kohle oder <abbr title="Gasturbine">GT</abbr>
- Der zentrale <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Kraftwerkstyp kann im betrachteten Zeitraum ausreichend Deckungsbeitrag zur Deckung der Fixkosten erwirtschaften. Diese Erkenntnis steht und fällt jedoch mit der Inklusion des Jahres 2022 und gilt nur unter einer idealen Kraftwerksflexibilität, die in der Realität tatsächlich nicht gegeben ist

### Limitationen

Zunächst muss festgehalten werden, dass sämtliche Aussagen nur auf Basis des hier (relativ eng) gesetzten Analyserahmens gelten und keinen Anspruch auf allgemeine Gültigkeit haben. Vor allem der begrenzte Analysezeitraum (10 Jahre) ist vor dem Hintergrund einer typischen Kraftwerkslebensdauer (25+ Jahre) relativ kurz gewählt und beinhaltet darüber hinaus eine signifikante Volatilität innerhalb des Zeitraums.

Darüber hinaus sind zumindest folgende Limitationen zu bedenken:

-	**Keine Liefergebühren**: für die Berechnung der Grenzkosten auf Basis der Brennstoffkosten wurde keine Gebühr für die Lieferung von Gas/Kohle zum Kraftwerk berücksichtigt
-	**Gaspreise auf Basis von TTF**: Annahmen zum Gaspreis wurden auf Basis des Preises an der Niederländischen Börse genommen. Diese sind nicht 1:1 anwendbar auf den österreichischen Markt, stellen aber eine ausreichende Approximation dar
-	**Annahme von günstigen Technologieparameter**: Technologiekosten entsprechen den Werten zum Zeitpunkt der Analyse (2024). Bei Gegenüberstellung mit historischen Preisen ergibt sich somit eine optimistische Einschätzung
-	**Volle Flexibilität des Kraftwerkseinsatzes**: Alle Kraftwerkstypen können mit voller Flexibilität am Markt agieren, das ist unter Berücksichtigung von technischen Restriktionen unrealistisch
-	**Effizienz bei optimaler Auslastung**: zur Berechnung der Grenzkosten wurde die maximale Effizienz bei voller Auslastung angenommen
-	**Nur Spotmärkte berücksichtigt**: Verkauf des Stroms erfolgt nur zu [Day-ahead]({{< ref "wissen/markt-day-ahead/index.md" >}}) Preisen, Forward Märkte werden nicht berücksichtigt. Damit ergeben sich mehr Preisspitzen.

Sämtlichen hier genannten Limitationen sprechen tendenziell für eine <u>Über</u>schätzung der Erlöse. Darüber hinaus gibt es aber auch noch Argumente, die für eine <u>Unter</u>schätzung sprechen.
-	Keine Erlöse aus [Regelenergie]({{< ref "wissen/regelreserve/index.md" >}}) berücksichtigt
-	Keine Erlöse aus [Redispatch]({{< ref "wissen/redispatch/index.md" >}})  berücksichtigt
-	Keine Erlöse aus Wärmeauskopplung (für <abbr title="Kraft-Wärme-Kopplung">KWK</abbr>)

<!-- Fußnoten -->

[^1]: [ENTSO-E Transparency Platform<br>(transparency.entsoe.eu)](https://transparency.entsoe.eu)

[^2]: [Trading Economics Gas<br>(tradingeconomics.com)](https://tradingeconomics.com/commodity/eu-natural-gas)

[^3]: [Trading Economics Coal<br>(tradingeconomics)](https://tradingeconomics.com/commodity/coal)

[^4]: [Trading Economics EU-ETS<br>(tradingeconomics.com)](https://tradingeconomics.com/commodity/carbon)

[^5]: [Stromgestehungskosten erneuerbare Energien<br>(ise.fraunhofer.de)](https://www.ise.fraunhofer.de/de/veroeffentlichungen/studien/studie-stromgestehungskosten-erneuerbare-energien.html)

[^6]: [Current and prospective costs of electricity generation until 2050<br>(Deutsches Institut für Wirtschaftsforschung)](https://www.econstor.eu/bitstream/10419/80348/1/757528015.pdf)

[^7]: [Harmonised index of consumer prices (HICP)<br>(ec.europa.eu/eurostat/)](https://doi.org/10.2908/PRC_HICP_AIND)

[^8]: [Clean Energy Technology Observatory: Hydropower and Pumped Storage Hydropower in the European Union - 2024 Status Report 
on Technology Development, Trends, Value Chains and Markets<br>(Europäische Kommission)](https://publications.jrc.ec.europa.eu/repository/handle/JRC139225)

[^9]: [ENTSO-E & ENTSOG TYNDP 2024 Scenarios Report<br>(2024.entsos-tyndp-scenarios.eu)](https://2024.entsos-tyndp-scenarios.eu/download/)