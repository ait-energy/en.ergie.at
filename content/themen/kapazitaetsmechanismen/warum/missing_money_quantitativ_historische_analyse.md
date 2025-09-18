---
title: "Missing Money - Quantitativ-Historische Analyse"
topics: []
authors: ["portmann", "afischer", "dkrainer"]
---

## 1. Kernfragestellung und methodischer Ansatz

Der folgende Abschnitt beschäftigt sich mit der Frage, ob bestehende und neue Kraftwerkskapazitäten im Setting eines [Energy-Only-Marktes]({{< ref "wissen/markt-energy-only/index.md" >}}) ausreichend finanziert werden können. Ziel der Analyse ist somit ein "quantitativer Nachweis" des Missing Money Problems auf Basis historischer Jahre für Österreich. Dazu wurden folgende Kraftwerkstechnologien untersucht:

- Gas- und Dampfkraftwerk Wasserstoff (GuD Wasserstoff)
- Gas- und Dampfkraftwerk Erdgas (GuD Erdgas)
- Gasturbine Wasserstoff (GT Wasserstoff)
- Gasturbine Erdgas (GT Erdgas)
- Laufwasserkraft (klein)
- Photovoltaik
- Windkraft (Onshore)

Zur Beurteilung der Wirtschaftlichkeit wurden die gesamten Kosten (variable und fixe Kosten der Erzeugung auf Basis historischer Marktdaten und Kostenannahmen) den Erlösen (Kraftwerkseinsatz zu Marktpreisen) gegenübergestellt. Um die Unsicherheit 
in den Annahmen zu berücksichtigen, wurde eine Monte Carlo Simulation durchgeführt, der eine Normalverteilung zugrunde 
gelegt wurde. Mittels der normalverteilten Monte Carlo Simulation wurde die Höhe der gewählten Parameter (OPEX, CPAEX, FOM,
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
aufweisen. Tabelle 1 gibt einen Überblick welche Technologien in der historischen und theoretischen Analyse betrachtet wurden.



| Historischer Ansatz | Theoretischer Ansatz |
|---------------------|----------------------|
| Erdgas              | GuD Wasserstoff      |
| PV                  | GuD Erdgas           |
| Windkraft           | GT Wasserstoff       |
| Laufwasserkraft (klein)    | GT Erdgas            |

  <caption style="caption-side: bottom; text-align: left;">
    <em>Tabelle 1: Aufteilung der Technologien in historische und theoretische Betrachtungsweise</em>
  </caption>

Die Technologie "Erdgas" entspricht hierbei dem historischen Einsatz der aggregierten, thermischen Erzeugungsanlagen in Österreich.
Als Inputparameter werden im Weiteren die gleichen Werte wie für GuD Erdgas verwendet.

Die Grenzkosten setzten sich zusammen
aus der Summe von variablen Betriebs- und Instandhaltungskosten 
<abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr>, variablen
Brennstoffkosten und variablen Emissionskosten:

Grenzkosten = Variable <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> Kosten + Variable Brennstoffkosten + Variable Emissionskosten

Die variablen Brennstoffkosten ergeben sich auf Basis von Effizienz und Preis des Brennstoffes:

<p>
  Variable Brennstoffkosten =
  <span style="display: inline-block; vertical-align: middle;">
    <span style="display: block; text-align: center;">
      Brennstoffpreis 
    </span>
    <span style="display: block; border-top: 1px solid #000; text-align: center;">
      Effizienz
    </span>
  </span>
</p>

Die variablen Emissionskosten ergeben sich auf Basis von Effizienz, CO<sub>2</sub>-Intensität und Preis für CO<sub>2</sub>-Zertifikate:

<p>
  Variable Emissionskosten =
  <span style="display: inline-block; vertical-align: middle;">
    <span style="display: block; text-align: center;">
     CO₂ Preis × CO₂ Intensität
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

![Preisentwicklung Commodities und Strom](/images/missing_money_quantitativ_historische_analyse/Preisentwicklung_commodities_strom_täglich_2.png)
*Abb. 1: Preisentwicklung Erdgas, CO2 Emissionszertifikate und Strom*
<!-- 
Abbildung 2 stellt den Zusammenhang zwischen Strompreisen und Grenzkosten auf monatlicher Basis dar. Es zeigt sich, dass der Strommarkt die Grenzkosten der Stromerzeugung auf Basis der Preise für Gas und Kohle sehr deutlich widerspiegelt. Der Strompreis folgt über weite Strecken den Grenzkosten und pendelt zwischen denen eines Gas- und Dampfkraftwerks und eines Kohlekraftwerks. Je nach Marktsituation (Verhältnis der Brennstoffpreise) bzw. Stromnachfrage entspricht der Strompreis tendenziell dem Minimum der Grenzkosten eines Gas- bzw. Kohlekraftwerks. Während im Jahr 2015 tendenziell Kohlekraftwerke den Preis setzen, entspricht der Strompreis seit Beginn 2019 tendenziell den Grenzkosten eines Gas- und Dampfkraftwerks.

![Zusammenhang Strompreis und Grenzkosten: monatlich](/images/missing_money_quantitativ_historische_analyse/zusammenhang_strompreis_und_grenzkosten_monatlich.png)
*Abb. 2: Zusammenhang Strompreis und Grenzkosten: monatlich* -->
Abbildung 2 stellt zum besseren Vergleich der Strompreise zwischen den Jahren 2019-2024 deren Jahresdauerlinien dar.
![Jahresdauerlinien des Strompreises für die Jahre 2019-2024](/images/missing_money_quantitativ_historische_analyse/jahresdauerlinien_Day_Ahead_Preis_2.png)
*Abb. 2: Jahresdauerlinien des Strompreises für die Jahre 2019-2024*

### Investitions- und Betriebskosten, Inflation und technische Annahmen

Des Weiteren wurden generische Annahmen bezüglich der Investitions- und Betriebskosten der jeweiligen Kraftwerkstechnologie auf Basis der Fraunhofer Studie *Stromgestehungskosten Erneuerbarer Energien* [^5] herangezogen. Für die Laufwasserkraftwerke wurden Annahmen aus dem Statusbericht 2024 der Europäischen Kommission zu *Wasserkraft und Pumpspeicherkraftwerken in der Europäischen Union* herangezogen [^8]. 

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
   <!-- <tr>
      <td>Pumpspeicherkraftwerk</td>
      <td>Europäische Kommission</td>
      <td>WACC von Windkraft übernommen, Mittlerer CAPEX ± 20 % für Werte hoch/niedrig</td>
    </tr> -->
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

Um einen adäquaten Unsicherheitsbereich in die Analyse aufzunehmen, wurden sämtliche CAPEX Werte aus der Fraunhofer Studie [^5] für ‚hoch‘ und ‚niedrig‘ herangezogen. Für Laufwasserkraft wurden die <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> Werte aus dem Status Bericht 2024 der Europäischen Kommission [^8] herangezogen, und die angegebene Spannbreite für ‚hoch‘ und ‚niedrig‘ verwendet. <!--, während für Pumpspeicherkraftwerke der mittlere <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> Wert um &#177; 20% variiert wurde. -->
Die fixen <abbr title="Operations & Maintenance (Betrieb und Instandhaltung)">O&M</abbr> Kosten wurden pro Technolgie als 1-3% der mittleren <abbr title="Capital Expenditures (Investitionskosten)">CAPEX</abbr> angenommen, um Werte für ‚hoch‘ und ‚niedrig‘ zu erhalten.
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
    <!--<tr>
      <td>Pumpspeicher</td><td>3.0</td><td>2.0</td><td>6.9 %</td><td>2.9 %</td>
    </tr> -->
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
   <!-- <tr>
      <td>Pumpspeicher</td><td>0.5</td><td>0.0</td><td>75.0</td><td>25.0</td>
    </tr> -->
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
   <!-- <tr>
      <td>Pumpspeicher</td><td>100 %</td><td>100 %</td><td>50</td><td>42</td>
    </tr> -->
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

Für Erdgas und CO<sub>2</sub> wurden die Preise auf Basis der historischen Zeitreihen (Abbildung 1) herangezogen. Für Wasserstoff wurden für alle Szenarien Werte zwischen 3 - 9 €/kg<sub>H2</sub> angenommen, wobei diese Preise wiederum im Rahmen einer normalverteilten Monte Carlo Simulation variiert wurden. Um die Kreuzpreiselastizität der unterschiedlichen Brennstoffe in den Jahren der hohen Strompreise zu berücksichtigen, wurde der gezogene Wasserstoffpreis in jedem Szenario als untere Schranke herangezogen. Überstieg der stündliche Erdgaspreis den Wasserstoffpreis, so wurde in dieser Stunde der Erdgaspreis als Näherung für den Wasserstoffpreis angenommen.
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



<!--Abbildung 3 zeigt den Kraftwerkseinsatz auf Jahresbasis für den theoretischen/historischen Ansatz. Zunächst ist evident, dass der theoretische Ansatz nicht mit den historischen Daten korrespondiert und zu deutlich abweichenden Ergebnissen führt. Während der theoretische Ansatz zu einer Auslastung von 30-40% für Gas und 40-80% für Kohle führt, ergibt sich im historischen Ansatz ein Einsatz von etwa 20-30%.

Das ist eine direkte Folge der impliziten idealen Flexibilität, die das modellierte Kraftwerk besitzt. In der theoretischen Betrachtung besteht keinerlei Einschränkung bezüglich Anfahrtsrampen. Das Kraftwerk kann somit voll flexibel agieren und den Deckungsbeitrag maximieren. In der Realität ist die Flexibilität stärker eingeschränkt, zumindest aufgrund technischer Limitationen bzgl. Startrampen (vor allem bei Kohle), aber auch aufgrund von Wärmelieferungsverpflichtungen.

![Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/jahrliche_kraftwerksauslastung_fur_kohlegud_fur_historischentheoretischen_kraftwerkseinsatz.png)
*Abb. 3: Jährliche Kraftwerksauslastung für alle Technologien im historischen/theoretischen Kraftwerkseinsatz*

Abbildung 5 stellt noch einmal den Kraftwerkseinsatz der beiden Ansätze auf stündlicher Ebene gegenüber. Daraus wird der Unterschied klar ersichtlich: das modellierte Kraftwerk agiert deutlich flexibler (und profitmaximierend) und kann somit einen deutlich höheren Deckungsbeitrag erwirtschaften. Die historischen Profile korrelieren durchaus mit der theoretisch optimalen Version, der Kraftwerkseinsatz fällt jedoch deutlich träger aus.

![Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/jahrliche_kraftwerksauslastung_fur_kohle_gud_fur_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 4: Jährliche Kraftwerksauslastung für Kohle/<abbr title="Gas- und Dampfkraftwerk">GuD</abbr> für historischen und theoretischen Kraftwerkseinsatz*

![Stündliche Kraftwerksauslastung für GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/stundliche_kraftwerksauslastung_fur_gud_fur_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 5: Stündliche Kraftwerksauslastung für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> für historischen/theoretischen Kraftwerkseinsatz* -->

### Wirtschaftlichkeit
#### Ergebnisse aller Simulationsläufe

In Abbildung 3 sind basierend auf dem historischen (historische Erzeugungsprofile) und dem theoretischen Kraftwerkseinsatz (Einsatz
basierend auf Grenzkosten) die Ergebnisse aller 20.000 Simulationsläufe für die betrachteten Technologien als Boxplots dargestellt.
Die Darstellung als Boxplot ermöglicht es, die Verteilung der 20.000 Simulationsergebnisse zu visualisieren und somit einen guten Überblick sowohl über die Medianwerte als auch die Spannweite zu erhalten.
Die Profite, Deckungsbeiträge, Abschöpfungen im Rahmen des Energiekrisenbeitrags-Strom (EKB-S) und Fixkosten (FOM und CAPEX) wurden
pro Technologie als eigener Boxplot visualisiert. Dadurch wird eine Gegenüberstellung der Deckungsbeiträge und des EKB-S - welche aus der Teilnahme am Day-Ahead Markt resultieren - mit den Fixkosten ermöglicht. Diese Ergebnisse ergeben zusammen den Profit pro Technologie. Der Deckungsbeitrag beinhaltet im Normalfall alle Einnahmen minus den variablen Kosten. In dieser Grafik wurde jedoch der Energiekrisenbeitrag-Strom separat herausgezogen und ist somit nicht im Deckungsbeitrag enthalten. Die eigenenständige Darstellung dieses Kostenfaktors wurde gewählt, um eine Abschätzung der Größenordnung der Gewinnabschöpfung und einen Vergleich zwischen den erneuerbaren Erzeugungsanlagen zu ermöglichen.
 

<!--Die Boxplots verdeutlichen die Verteilung der Profite für jede Technologie und zeigen sowohl die Medianwerte als auch die Spannweite der Ergebnisse auf. Insbesondere wird sichtbar, dass die Profite für die meisten Technologien stark variieren und in einigen Fällen sogar negative Werte annehmen.

zeigt die über alle Szenario-Kombinationen gemittelten Profite auf jährlicher Basis und stellt die Ergebnisse des theoretischen und historischen Kraftwerkseinsatzes gegenüber. Zunächst zeigt sich, dass die Profite über die Jahre stark schwanken, wobei das für alle Kraftwerkstypen gilt. Des Weiteren zeigt sich, dass nahezu alle Kraftwerkstypen bis 2021 Geld verloren haben. Mit Beginn der Energiekrise Ende 2021 bis in das Jahr 2024 sind die beobachtbaren Profite von <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas sowohl in der theoretischen als auch historischen Betrachtung merklich angestiegen. Erneuerbare Erzeugungstechnologien (Laufwasserkraft, Speicherwasserkraft, Solar PV und Wind) erlebten 2022 einen sprunghaften Anstieg der Profite bzw. eine Umkehr von Verlusten in Gewinne.

Zum einen ist ersichtlich, dass abseits der Jahre der Energiekrise (2021+2022) für keinen Kraftwerkstyp ausreichend Deckungsbeitrag erwirtschaftet werden konnte, um die laufenden Kosten zu decken. Zum anderen hatten die Jahre der Energiekrise (2021+2022) eine signifikant positive Auswirkung auf die Erlöse aller Kraftwerkstypen.

Abbildung 8 vergleicht direkt die Profite zwischen dem historischen und dem theoretischen Kraftwerkseinsatz für Kohle und <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas. Daraus zeigt, sich, dass die theoretische Betrachtung konsequent optimistischere Resultate liefert als sich aus den historisch beobachtbaren Einsatzzeiten ableiten lassen würde.--> 

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_Wind_MW.png" alt="Boxplot Wind" title="Wind" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">Wind</h6>
  </div>
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_PV_MW.png" alt="Boxplot PV" title="PV" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">PV</h6>
  </div>
</div>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_KWKW_MW.png" alt="Boxplot Laufwasserkraftwerk (klein)" title="KWKW" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">Kleinwasserkraft</h6>
  </div>
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_Erdgas.png" alt="Boxplot Erdgas" title="Erdgas historisch" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">Erdgas</h6>
  </div>
</div>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_Erdgas_OCGT_MW_1.png" alt="Boxplot Erdgas GT" title="Erdgas OCGT" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">Erdgas GT*</h6>
  </div>
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_Erdgas_CCGT_MW_1.png" alt="Boxplot Erdgas GuD" title="Erdgas GuD" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">Erdgas GuD*</h6>
  </div>
</div>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_H_OCGT_MW.png" alt="Boxplot H2 OCGT" title="H2 GT" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">H2 GT*</h6>
  </div>
  <div style="position: relative;">
    <img src="/images/missing_money_quantitativ_historische_analyse/Boxplot_H2_CCGT_MW.png" alt="Boxplot H2 GuD" title="H2 GuD" style="width: 100%; height: auto;">
    <h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">H2 GuD*</h6>
  </div>
</div>


*Abb. 3: Profit, Deckungsbeitrag (DB), Energiekrisenbeitrag-Strom (EKB-S) sowie Fixe Betriebs- und Instandhaltungskosten (FOM) und Investitionskosten (CAPEX) über alle Simulationsläufe. <br>
DB = Einnahmen – Brennstoffkosten – variable Betriebs- und Instandhaltungskosten (VOM).<br> Betrachtete Technologien:  Wind, PV, Erdgas historisch,
Kleinwasserkraft, Erdgas GT\* und Erdgas GuD\*<br>\* theoretischer Kraftwerkseinsatz: Einsatz erfolgt basierend auf wirtschaftlichen Kriterien (Grenzkosten < Strompreis)*

Im Folgenden werden die Ergebnisse für die einzelnen Technologien näher betrachtet.

<u> Erneuerbare Erzeugungsanlagen:</u>

Sowohl Wind, PV als auch Laufwasserkraft (klein) zeigen im Median einen positiven Profit, wodurch ersichtlich wird, dass 
über einen Großteil der Simulationsläufe hinweg ausreichend Deckungsbeiträge durch die alleinige Teilnahme am EOM erwirtschaftet
werden können. Damit können für über 50% der Simulationen alle erneuerbaren Erzeugungsanlagen ihre Fixkosten decken und es tritt kein "Missing-Money-Problem" auf. PV zeigt die geringste Spannweite (-27 bis 101&nbsp;k€/MW/a) im Profit, gefolgt von Wind (-94 bis 137&nbsp;k€/MW/a), während Laufwasserkraft die größte Variation aufweist (2 bis 402&nbsp;€/MW/a). Sowohl PV als auch Wind verzeichnen für etwas mehr als 25% der Simulationsläufe Verluste (negativer Profit), wobei Wind hier potenziell ein größeres Problem hat, nachdem die Spannweite der Verluste (bis -94k€/MW/a) deutlich größer ist als bei PV (bis -27&nbsp;k€/MW/a). Für Laufwasserkraft hingegen ist ersichtlich, dass über alle Simulationsläufe hinweg keine Verluste auftreten, diese Technologie somit in 100% der Simulationen genügend Deckungsbeiträge erwirtschaften kann und daher keinem "Missing-Money-Problem" ausgesetzt ist.

Weitere, interessante Erkenntnisse lassen sich aus der Betrachtung des EKB-S für die einzelnen Technologien ableiten. Insbesondere Laufwasserkraftwerke sind vom EKB-S stark betroffen (~69&nbsp;k€/MW/a), gefolgt von Wind (~36&nbsp;k€/MW/a) und PV (~7&nbsp;k€/MW/a). Auch wenn Laufwasserkraft über alle Simulationen hinweg am stärksten betroffen ist, so ist für Wind die Spannweite der Gewinnabschöpfung am größten (bis 497&nbsp;€/MW/a). Auf PV hat der EKB-S die geringste Auswirkung, erkenntlich an dem geringen Median und der engen Spannweite ( 0 bis 75&nbsp;k€/MW/a). Dies ist darauf zurückzuführen, dass die Erzeugung von PV in Stunden mit Knappheit (begrenzte Verfügbarkeit von Erneuerbaren oder hoher Nachfrage) und daher hohen Strompreisen in der Regel geringer ausfällt. 

Abbildung 4 stellt für die erneuerbaren Technologien die Simulationsergebnisse zusätzlich in Form von Dauerlinien mit Median und Quantilen dar, wobei ebenfalls der EKB-S eingezeichnet ist, wodurch ersichtlich wird in wie vielen Stunden des Jahres ein Gewinnabschöpfung auftritt.
![Jahresdauerlinie_Erneuerbare](/images/missing_money_quantitativ_historische_analyse/Jahresdauerlinie_Erneuerbare.png)
*Abb. 4: Median und Quantile der Jahresdauerlinien der Einnahmen von PV, Wind und Laufwasserkraft über alle Szenarien mit eingezeichneter Schwelle der Gewinnabschöpfung.*

Die Dauerlinien der Einnahmen zeigen, dass PV im Median keiner Gewinnabschöpfung ausgesetzt ist, während Wind in etwa 3% der Stunden und Laufwasserkraft in etwa 5% der Stunden des Jahres eine Gewinnabschöpfung erfährt. Bezieht man alle Simulationsläufe mit ein, so zeigt sich, dass PV in maximal 19% der Stunden, Wind in maximal 33% der Stunden und Laufwasserkraft in bis zu 77% der Stunden des Jahres von einer Gewinnabschöpfung betroffen ist. Diese Darstelltung der Jahresdauerlinien der Einnahmen verdeutlicht die zuvor beschriebenen Ergebnisse der Boxplots und veranschaulicht, dass Laufwasserkraft im größten Umfang von der Gewinnabschöpfung betroffen ist.

<u> Fossile, thermische Erzeugungsanlagen: </u>

Die Betrachtung der Profite von Erdgas (entspricht dem historischen Einsatz) zeigt, dass diese Technologie über einen Großteil der Simulationsläufe Geld verliert (Median der Profite ist negativ). Hier muss jedoch darauf hingewiesen werden, dass Einnahmen aus anderen Märkten und aus der Fernwärmebereitstellung nicht berücksichtigt wurden. Da es sich hierbei um einen historischen Kraftwerkseinsatz handelt und anzunehmen ist, dass dieser nicht stattgefunden hätte, wenn die Wirtschaftlichkeit nicht gegeben gewesen wäre, lässt sich daraus schließen, dass die tatsächlichen Profite durch diese zusätzlichen Einnahmen deutlich höher ausfallen. Die aussagekräftigeren Ergebnisse liefern in diesem Fall die theoretischen Betrachtungen für Erdgas GT* und GuD*, denen eine optimale Flexibilität unterstellt wurde. Durch diese Betrachtung lässt sich eine quantitative Abschätzung treffen, ob diese Technologien durch eine reine Teilnahme am EOM finanzierbar sind. Beide Kraftwerksarten zeigen über alle Simulationsläufe hinweg im Median eine positive Rentabilität, wobei Erdgas GuD* ein deutliches Potential für hohe Gewinne (bis 682k€/MW/a) aufweist.
Eine Deckung der Fixkosten ist für beide Technologien durch Teilnahme am Day-Ahead Markt daher in der Regel gegeben.

<u> Nicht-fossile, thermische Erzeugungsanlagen: </u>

Wasserstoffbetriebene Kraftwerke (GT & GuD) verzeichnen in mehr als 75% der Simulationsläufe Verluste (negativer Profit), wobei sie nur in Ausnahmefällen Gewinne erzielen können. In einzelnen Fällen (in der Form von Ausreißern) verzeichnet diese Technologie Gewinne, ausgelöst durch eine Kombination von niedrigen Kosten in den Inputparametern und besonders hohen Strompreisen in den Krisenjahren. Es ist ersichtlich, dass diese Technologie selbst unter optimistischen Annahmen (niedrige Wasserstoffpreise) in der aktuellen Marktsituation nicht wirtschaftlich betrieben werden kann und somit vor einem signifikanten "Missing-Money-Problem" steht. 

Zur Übersicht und zum Vergleich zwischen den Technologien, sind die Medianwerte der Boxplots in der folgenden Tabelle dargestellt:

<!DOCTYPE html>
<html lang="de">
<table>
    <thead>
    <style>
    th {
        white-space: nowrap; /* Verhindert Umbruch im Spaltentitel */
    }
</style>
        <tr>
            <th>Technologie</th>
            <th>Profit</th>
            <th>Einnahmen</th>
            <th>Brennstoffkosten</th>
            <th>Emissionskosten</th>
            <th>VOM</th>
            <th>EKB-S</th>
            <th>FOM</th>
            <th>CAPEX</th>
            <th>Volllaststunden</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>PV</td>
            <td>13.2</td>
            <td>86.6</td>
            <td>0.0</td>
            <td>0.0</td>
            <td>0.3</td>
            <td>7.5</td>
            <td>16.0</td>
            <td>51.3</td>
            <td>1341</td>
        </tr>
        <tr>
            <td>Laufwasserkraft</td>
            <td>264.4</td>
            <td>492.5</td>
            <td>0.0</td>
            <td>0.0</td>
            <td>1.2</td>
            <td>69.0</td>
            <td>42.0</td>
            <td>115.0</td>
            <td>5021</td>
        </tr>
        <tr>
            <td>Wind</td>
            <td>32.0</td>
            <td>237.0</td>
            <td>0.0</td>
            <td>0.0</td>
            <td>17.2</td>
            <td>36.4</td>
            <td>32.0</td>
            <td>117.3</td>
            <td>2441</td>
        </tr>
        <tr>
            <td>Erdgas</td>
            <td>-56.3</td>
            <td>223.4</td>
            <td>129.1</td>
            <td>46.3</td>
            <td>11.9</td>
            <td>0.0</td>
            <td>22.0</td>
            <td>94.5</td>
            <td>2390</td>
        </tr>
        <tr>
            <td>Erdgas GT*</td>
            <td>25.7</td>
            <td>355.2</td>
            <td>156.4</td>
            <td>74.5</td>
            <td>6.5</td>
            <td>0.0</td>
            <td>11.5</td>
            <td>49.4</td>
            <td>1711</td>
        </tr>
        <tr>
            <td>Erdgas GuD*</td>
            <td>76.2</td>
            <td>600.9</td>
            <td>296.5</td>
            <td>118.9</td>
            <td>27.7</td>
            <td>0.0</td>
            <td>22.0</td>
            <td>94.5</td>
            <td>5644</td>
        </tr>
        <tr>
            <td>Wasserstoff GT*</td>
            <td>-86.1</td>
            <td>4.4</td>
            <td>3.7</td>
            <td>0.0</td>
            <td>0.0</td>
            <td>0.0</td>
            <td>17.5</td>
            <td>78.7</td>
            <td>6</td>
        </tr>
        <tr>
            <td>Wasserstoff GuD*</td>
            <td>-170.1</td>
            <td>11.0</td>
            <td>7.9</td>
            <td>0.0</td>
            <td>0.1</td>
            <td>0.0</td>
            <td>35.0</td>
            <td>157.3</td>
            <td>25</td>
        </tr>
    </tbody>
</table>

</body>
</html>


*Tab. 7: Medianwerte der Boxplots in k€/MW/a für alle Technologien. Einnahmen = Erlöse aus dem Day-Ahead Markt; VOM = variable Betriebskosten; EKB-S = Energiekrisenbeitrag-Strom; \* theoretischer Kraftwerkseinsatz: Einsatz erfolgt basierend auf wirtschaftlichen Kriterien (Grenzkosten < Strompreis)*

<!--
![Mittlere Profite über alle Szenarien auf Basis historischer Erzeugungsprofile](/images/missing_money_quantitativ_historische_analyse/mittlere_profite_uber_alle_szenarien_auf_basis_historischer_erzeugungsprofile.png)
*Abb. 6: Mittlere Profite über alle Szenarien auf Basis historischer Erzeugungsprofile*
![Mittlere Profite über alle Szenarien verglichen zwischen historischem und theoretischem Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/mittlere_profite_uber_alle_szenarien_verglichen_zwischen_historischem_und_theoretischem_kraftwerkseinsatz.png)
*Abb. 7: Mittlere Profite über alle Szenarien verglichen zwischen historischem und theoretischem Kraftwerkseinsatz* -->

#### Ergebnisse für das Jahr 2024

Zusätzlich zur Betrachtung der Simulationsergebnisse über alle Jahre, wurde das Jahr 2024 herausgezogen – vor dem Hintergrund, dass in diesem Jahr die Durchdringung der erneuerbaren Erzeugungsanlagen bereits stärker einem zukünftigen Stromsystem entspricht und dieses Jahr zudem frei von krisenbedingten Preisspitzen war. Die Erlöse, Kosten und der Profit werden als Wasserfall-Grafiken dargestellt, wobei die Durchschnittswerte über alle Simulationsläufe im Jahr 2024 verwendet wurden. Durch diese Betrachtung ergibt sich nun ein leicht verändertes Gesamtbild für alle Technologien. 

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div>
<style>.responsive23-uZI3iggs9718Gc7L-bar-vertical-waterfall_wind { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-uZI3iggs9718Gc7L-bar-vertical-waterfall_wind { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-uZI3iggs9718Gc7L-bar-vertical-waterfall_wind { padding-top: 142.86%; } }</style>
<div id="container23-uZI3iggs9718Gc7L-bar-vertical-waterfall_wind" class="responsive23-uZI3iggs9718Gc7L-bar-vertical-waterfall_wind" style="position: relative;"><iframe title="Waterfall_Wind" src="https://app.23degrees.io/embed/uZI3iggs9718Gc7L-bar-vertical-waterfall_wind" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/uZI3iggs9718Gc7L-bar-vertical-waterfall_wind"></script>
  </div>
  <div>
    <style>.responsive23-ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv { padding-top: 142.86%; } }</style>
<div id="container23-ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv" class="responsive23-ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv" style="position: relative;"><iframe title="Waterfall_PV" src="https://app.23degrees.io/embed/ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/ibeXvvM38w4MeiXJ-bar-vertical-waterfall_pv"></script>
  </div>
</div>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div>
<style>.responsive23-aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv { padding-top: 142.86%; } }</style>
<div id="container23-aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv" class="responsive23-aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv" style="position: relative;"><iframe title="Waterfall_RoR" src="https://app.23degrees.io/embed/aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/aTVdWDUTX1lmhwR6-bar-vertical-waterfall_pv"></script>
  </div>
  <div>
   <style>.responsive23-oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas { padding-top: 142.86%; } }</style>
<div id="container23-oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas" class="responsive23-oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas" style="position: relative;"><iframe title="Waterfall-natural gas" src="https://app.23degrees.io/embed/oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/oEi7m3gQZgTNTzHd-bar-vertical-waterfall-natural-gas"></script>
  </div>
</div>
<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div>
<style>.responsive23-nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt { padding-top: 142.86%; } }</style>
<div id="container23-nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt" class="responsive23-nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt" style="position: relative;"><iframe title="Waterfall-natural gas ocgt" src="https://app.23degrees.io/embed/nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/nXwwxph9MdDZUyBX-bar-vertical-waterfall-natural-gas-ocgt"></script>
  </div>
  <div>
  <style>.responsive23-ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt { padding-top: 142.86%; } }</style>
<div id="container23-ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt" class="responsive23-ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt" style="position: relative;"><iframe title="Waterfall-natural gas ccgt" src="https://app.23degrees.io/embed/ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/ERyjS7dlg6PLU7Wl-bar-vertical-waterfall-natural-gas-ccgt"></script>
  </div>
</div>


<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 20px; align-items: start;">
  <div>
  <style>.responsive23-ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt { padding-top: 142.86%; } }</style>
<div id="container23-ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt" class="responsive23-ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt" style="position: relative;"><iframe title="Waterfall-hydrogen ocgt" src="https://app.23degrees.io/embed/ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/ZAsBvtU6VikJQKXd-bar-vertical-waterfall-hydrogen-ocgt"></script>
<h6 style="position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255,255,255,0.8); padding: 2px 8px; margin: 0; border-radius: 3px;">H2 GT*</h6>
  </div>
  <div>
    <style>.responsive23-vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt { width: 100%; padding-top: 100%; } @media (max-width: 600px) { .responsive23-vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt { padding-top: 100%; } } @media (max-width: 360px) { .responsive23-vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt { padding-top: 142.86%; } }</style>
<div id="container23-vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt" class="responsive23-vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt" style="position: relative;"><iframe title="Waterfall-hydrogen ccgt" src="https://app.23degrees.io/embed/vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt" allow="fullscreen" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0"></iframe></div>
<script src="https://app.23degrees.io/services/public/embed-code/vjnFvlPlwuwXmY8g-bar-vertical-waterfall-hydrogen-ccgt"></script>
  </div>
</div>

*Abb. 5: Einnahmen, Brennstoff- und Emissionskosten, variable Betriebs- und Instandhaltungskosten (VOM), Energiekrisenbeitrag-Strom (EKB-S) sowie fixe Betriebs- und Instandhaltungskosten (FOM), Investitionskosten (CAPEX) und resultierende Profite über alle Simulationsläufe für das Jahr 2024.
Betrachtete Technologien: Wind, PV, Erdgas historisch, Kleinwasserkraft, Erdgas GT\* und Erdgas GuD\* <br>
\* theoretischer Kraftwerkseinsatz: Einsatz erfolgt basierend auf wirtschaftlichen Kriterien (Grenzkosten < Strompreis)*

Während PV über alle Simulationen noch einen ausreichenden Deckungsbeitrag erwirtschaften konnte, reichen im Jahr 2024 die Erlöse knapp nicht mehr aus um die Fixkosten zu decken. Damit steht PV vor einem Finanzierungsproblem und ist damit einer geringen Menge von "Missing-Money" ausgesetzt.  Wind und Laufwasserkraft können weiterhin ausreichend Deckungsbeiträge erwirtschaften, während die generierten Erlöse für die fossilen, thermischen Technologien nicht mehr ausreichen um die gesamten Kosten zu decken. Besonders überraschend ist dies bei den erdgasbetriebenen GuDs, da sie über alle Simulationsläufe hinweg ein erhebliches Potenzial für hohe Gewinne aufweisen. Wenig überraschend sind hingegen die Ergebnisse für die wasserstoffbetriebenen Kraftwerke, die auch im Jahr 2024 vor einem erheblichen "Missing-Money-Problem" stehen.

<!-- 
Abbildung 9 illustriert die Schwankungsbreite hinter den Durchschnittsergebnissen in Form von Boxplots. Während die Resultate für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Erdgas in der historischen Betrachtung zwischen -200 €/kW und 0 €/kW schwanken, bewegen sich die Profite in der theoretischen Betrachtung in 50% der Fälle zwischen -50 €/kW und +50 €/kW.

Für <abbr title="Gas- und Dampfkraftwerk">GuD</abbr> Wasserstoff stellt sich die Sache noch volatiler und verlustreicher dar. In zumindest 75% der Fälle ergibt sich ein Verlust von mindestens 100 €/kW. Auf Basis der angenommenen Preise für Wasserstoff von 3 €/kg bzw. 6 €/kg ergibt sich ausschließlich in den Jahren 2021 und 2022 eine positive Auslastung. Aufgrund der äußerst hohen Strompreise in diesen Jahren ergibt sich jedoch ein günstiges Verhältnis zwischen Input- und Outputpreisen, wodurch sich hohe Gewinne ergeben.

Relativ robuste Ergebnisse zeigen sich für Solar PV: Hier ist die Schwankungsbreite äußerst gering, de-facto -50 bis + 50 €/kW in 90% der Fälle. 

Für die Interpretation an dieser Stelle ist jedoch erwähnenswert, dass die Bewertung auf Grundlage von geschätzten Investitionskosten im Jahr 2024 gegen historische Preise zwischen 2015 und 2024 erfolgt. Aufgrund der stark gefallenen Investitionskosten von Photovoltaik im vergangenen Jahrzehnt kann demnach nicht die Schlussfolgerung gezogen werden, dass bestehende Anlagen dieses Typs genau diese Profitabilität aufweisen.


Abbildung 10 stellt noch einmal die volle Schwankungsbreite und Größenordnung von Deckungsbeitrag und Fixkosten für alle Kraftwerkstypen und Kraftwerkseinsatzmodalitäten dar. Augenscheinlich ist dabei, dass der Deckungsbeitrag weitaus größeren Schwankungsbreiten ausgesetzt ist als die Kostenseite. Trotz Variation der Investitions- und Betriebskosten, <abbr title="Weighted Average Cost of Capital (gewichtete durchschnittliche Kapitalkosten)">WACC</abbr> und Lebensdauer ergeben sich bei weitem nicht so hohe Schwankungsbreiten wie auf der Erlösseite. Dies spiegelt die hohe Volatilität im Strommarkt wider. -->

## 4. Schlussfolgerungen

In Bezug auf "Missing-Money" können daher folgende Schlussfolgerungen abgeleitet werden:
-	Erdgasbasiertes Gas- und Dampfkraftwerke sowie Spitzenlastkraftwerke können auf Basis der letzten 6 Jahre unter idealen Bedingungen gewinnbringend betrieben werden. Die Aussagekraft hängt jedoch stark von der betrachteten Zeitperiode (2019-2024) und den zugrundeliegenden Annahmen über vollständig flexiblen Kraftwerkseinsatz ab. 
-	In der aktuellen Markt- und Systemlage (Jahr 2024) lässt sich ein bestehendes Missing-Money-Problem für einzelne Marktteilnehmer:innen im österreichischen Energy-Only-Markt identifizieren. 
- Das Missing-Money-Problem ergibt sich in der aktuellen Markt- und Systemlage für fossile Technologien durch zu wenig Einsatzzeiten, um ausreichend Deckungsbeiträge zu erwirtschaften. Auch PV ist in der aktuellen Markt- und Systemlage vom Missing-Money-Problem betroffen. Die Ursachen hierfür liegen in den hohen Investitionskosten und den niedrigen Strompreisen zu Zeiten von PV-Einspeisung, die durch die bereits hohe Durchdringung von PV im Stromsystem bedingt sind.
- Wasserstoffbetriebene Kraftwerke sehen sich selbst unter optimistischen Annahmen mit einem erheblichen Missing-Money-Problem konfrontiert. Um Investitionen zu ermöglichen, sind Förderungen erforderlich, da der Markt keine ausreichenden Anreize für Investitionen bietet.

Bei diesen Schlussfolgerungen ist jedoch zu berücksichtigen, dass keine Förderungen miteinbezogen und ausschließlich die im Day-Ahead-Markt erzielbaren Erlöse betrachtet wurden. Eine Teilnahme an zusätzlichen Märkten kann das Gesamtbild erheblich verändern und die Wirtschaftlichkeit der Marktteilnehmer:innen maßgeblich beeinflussen.


### Limitationen

Zunächst muss festgehalten werden, dass sämtliche Aussagen nur auf Basis des hier gesetzten Analyserahmens gelten und keinen Anspruch auf allgemeine Gültigkeit haben. Vor allem der begrenzte Analysezeitraum (6 Jahre) ist vor dem Hintergrund einer typischen Kraftwerkslebensdauer (25+ Jahre) relativ kurz gewählt und beinhaltet darüber hinaus eine signifikante Volatilität innerhalb des Zeitraums.

Darüber hinaus sind zumindest folgende Limitationen zu bedenken:

-	**Keine Liefergebühren**: für die Berechnung der Grenzkosten auf Basis der Brennstoffkosten wurde keine Gebühr für die Lieferung von Gas zum Kraftwerk berücksichtigt
-	**Gaspreise auf Basis von TTF**: Annahmen zum Gaspreis wurden auf Basis des Preises an der niederländischen Börse genommen. Diese sind nicht 1:1 anwendbar auf den österreichischen Markt, stellen aber eine ausreichende Approximation dar
-	**Annahme von günstigen Technologieparameter**: Technologiekosten entsprechen den Werten zum Zeitpunkt der Analyse (2024). Bei Gegenüberstellung mit historischen Preisen ergibt sich somit eine optimistische Einschätzung
-	**Volle Flexibilität des Kraftwerkseinsatzes**: Alle Kraftwerkstypen können mit voller Flexibilität am Markt agieren, das ist unter Berücksichtigung von technischen Restriktionen unrealistisch
-	**Effizienz bei optimaler Auslastung**: zur Berechnung der Grenzkosten wurde die maximale Effizienz bei voller Auslastung angenommen
-	**Nur Spotmärkte berücksichtigt**: Verkauf des Stroms erfolgt nur zu [Day-ahead]({{< ref "wissen/markt-day-ahead/index.md" >}}) Preisen, Forward Märkte werden nicht berücksichtigt. 

Sämtlichen hier genannten Limitationen sprechen tendenziell für eine <u>Über</u>schätzung der Erlöse. Darüber hinaus gibt es aber auch noch Argumente, die für eine <u>Unter</u>schätzung sprechen.
-	Keine Erlöse aus [Regelenergie]({{< ref "wissen/regelreserve/index.md" >}}) berücksichtigt
-	Keine Erlöse aus [Redispatch]({{< ref "wissen/redispatch/index.md" >}})  berücksichtigt
-	Keine Förderungen (wie zum Beispiel Marktprämie) für erneuerbare Erzeugungsanlagen berücksichtigt
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