---
title: "Missing Money - Quantitativ-Historische Analyse"
topics: []
authors: ["portmann", "afischer"]
---

## 1. Kernfragestellung und methodischer Ansatz

Der folgende Abschnitt fokussiert auf die Frage, ob bestehende Kraftwerkskapazitäten im Setting eines [Energy-Only-Markts]({{< ref "wissen/markt-energy-only/index.md" >}}) ausreichend finanziert werden können. Ziel der Analyse ist somit ein ‚quantitativer Nachweis‘ des Missing Money auf historischer Basis für Österreich.

Dazu werden für die Kraftwerkstechnologien

- Gas und Dampfkraftwerk (<abbr title="Combined Cycle Gas Turbine">CCGT</abbr>)
- Gas Turbine
- Kohle

werden die historischen Kosten (auf Basis der beobachtbaren Börsenpreise für Gas, Kohle und Co2) und Erlöse (auf Basis der stündlichen [Day-ahead]({{< ref "wissen/markt-energy-only/index.md" >}}) Marktergebnisse) gegenübergestellt und beurteilt, ob die Investitionen (auf Basis <abbr title="Capital Expenditure">CAPEX</abbr>/
<abbr title="Operational Expenditure">OPEX</abbr> Werte der Danish Technology Database) finanzierbar sind.
Zur Determinierung des stündlichen Kraftwerkseinsatzes wurden zwei verschiedene Ansätze verfolgt

- **Theoretisch optimaler Kraftwerkseinsatz**: Voller Einsatz, in Stunden mit positivem Deckungsbeitrag (Erlöse > Grenzkosten)
- **Historisch beobachteter Kraftwerkseinsatz**: historischer Kraftwerkseinsatz laut entso-e [^1] für den gesamten Österreichischen "Gas" Kraftwerkspark
Die Analyse erfolgt auf historischer Basis für die Jahre 2015-2023.

## 2. Annahmen und Eingangsgrößen

### 2.1 Preisentwicklung

Zur Entwicklung der Strompreise wurden die stündlichen Werte der EPEX [Day-ahead]({{< ref "wissen/markt-energy-only/index.md" >}}) 60-Minuten Auktion herangezogen, Zugriff via <https://transparency.entsoe.eu/> [^1]. Für die Ermittlung der Grenzkosten der jeweiligen Kraftwerke wurden die Preise der Rohstoffe näherungsweise bestimmt. Dazu wurden die grafischen Informationen von tradingeconomics.com für Gas, Kohle und Co2 verwertet [^2], [^3], [^4] und die (näherungsweise) tatsächlichen Werte mittels <https://plotdigitizer.com/> extrahiert. Anschließend wurden die Werte auf Tagesbasis interpoliert und in einem weiteren Schritt auf Monatsbasis gemittelt.

![Preisentwicklung Commodities und Strom](/images/missing_money_quantitativ_historische_analyse/preisentwicklung_commodities_und_strom.png)
*Abb. 1: Preisentwicklung Commodities und Strom*

Abbildung 2 stellt den Zusammenhang zwischen Strompreisen und Grenzkosten auf monatlicher Basis dar. Es zeigt sich, dass der Strommarkt die Grenzkosten der Stromerzeugung auf Basis der Preise für Gas und Kohle sehr deutlich widerspiegelt. Der Strompreis folgt über weite Strecken den Grenzkosten und pendelt zwischen denen eines Gas- und Dampfkraftwerks und eines Kohlekraftwerks. Je nach Marktsituation (Verhältnis der Commodity-Preise) bzw. Stromnachfrage entspricht der Strompreis tendenziell dem Minimum der Grenzkosten eines Gas- bzw. Kohlekraftwerks. Während im Jahr 2015 tendenziell Kohlekraftwerke den Preis setzen, entspricht der Strompreis seit Beginn 2019 tendenziell den Grenzkosten eines Gas- und Dampfkraftwerks.

Abbildung 3 zeigt den gleichen Zusammenhang auf einer stündlichen Ebene. Auch hier zeigt sich, dass die Strompreise meistens zwischen den Grenzkosten der beiden Kraftwerkstechnologien auf stündlicher Basis schwanken.

![Zusammenhang Strompreis und Grenzkosten: monatlich](/images/missing_money_quantitativ_historische_analyse/zusammenhang_strompreis_und_grenzkosten_monatlich.png)
*Abb. 2: Zusammenhang Strompreis und Grenzkosten: monatlich*

![Zusammenhang Strompreis und Grenzkosten: stündlich](/images/missing_money_quantitativ_historische_analyse/zusammenhang_strompreis_und_grenzkosten_stündlich.png)
*Abb. 3: Zusammenhang Strompreis und Grenzkosten: monatlich*

### 2.2 CAPEX, OPEX, Inflation und technische Annahmen

Des Weiteren wurden generische Annahmen bezüglich der Investitions- und Betriebskosten der jeweiligen Kraftwerkstechnologie auf Basis des "Technology Catalogues" der Dänischen Energieagentur herangezogen [^5]. Eine Zusammenfassung der Werte ist in der nachfolgenden Tabelle dargestellt:

|                          | GT     | CCGT   | Coal   |
|--------------------------|--------|--------|--------|
| **Efficiency**           | 0.45   | 0.61   | 0.52   |
| **Lifetime**             | 25     | 25     | 25     |
| **Investment (€m/MW)**   | 0.56   | 0.83   | 1.86   |
| **Fixed O&M (€/MW/y)**   | 18600  | 27800  | 30355  |
| **Variable O&M (€/MWh)** | 4.2    | 4.2    | 2.8    |

Für die Analyse wurden Werte für das Jahr 2030 herangezogen um bewusst optimistische Werte auszuwählen.
Darüber hinaus wurden Annahmen zur Co2-Intensität der jeweiligen Energieträger getroffen. Diese sind in der
nachfolgenden Tabelle zusammengefasst:

|                             | Gas  | Coal |
|-----------------------------|------|------|
| **Co2-Intensität (kg CO₂/GJ)** | 50.3 | 88.3 |

Die nominalen Geldwerte hinsichtlich der Strom- und Commoditypreise wurden auf reale Werte 2015 angepasst, basierend auf den Inflationsdaten für Österreich laut des Harmonisierten Verbraucherpreisindex (HICP) von Eurostat [^6], um den Geldwerteinheiten der Dänischen Energieagentur zu entsprechen:

| Year   | 2015 | 2016 | 2017 | 2018 | 2019 | 2020 | 2021 | 2022 | 2023 |
|--------|------|------|------|------|------|------|------|------|------|
| Index  | 1.00 | 1.01 | 1.03 | 1.05 | 1.07 | 1.08 | 1.11 | 1.21 | 1.30 |

## 3. Resultate

### 3.1 Auslastung

Abbildung 4 zeigt den Kraftwerkseinsatz auf Jahresbasis für den theoretischen/historischen Ansatz. Zunächst ist evident, dass der theoretische Ansatz nicht mit den historischen Daten korrespondiert und zu deutlich abweichenden Ergebnissen führt. Während der ‚theoretische‘ Ansatz zu einer Auslastung von 30-40% für Gas und 40-80% für Kohle führt, ergibt sich im historischen Ansatz ein Einsatz von etwa 20-30%.
Das ist eine direkte Folge der impliziten idealen Flexibilität, die das modellierte Kraftwerk besitzt. In der theoretischen Betrachtung besteht keinerlei Einschränkung bezüglich Anfahrtsrampen. Das Kraftwerk kann somit voll flexibel agieren und den Deckungsbeitrag maximieren. In der Realität ist die Flexibilität stärker eingeschränkt, zumindest aufgrund technischer Limitationen bzgl. Startrampen (vor allem bei Kohle), aber auch aufgrund von Wärmelieferungsverpflichtungen.

![Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/jährliche_kraftwerksauslastung_für_kohle_gud_für_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 4: Jährliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz*

![Stündliche Kraftwerksauslastung für Kohle/GuD für historischen/theoretischen Kraftwerkseinsatz](/images/missing_money_quantitativ_historische_analyse/stündliche_kraftwerksauslastung_für_kohle_gud_für_historischen_theoretischen_kraftwerkseinsatz.png)
*Abb. 5: Stündliche Kraftwerksauslastung für Kohle/<abbr title="Gas- und Dampfkraftwerk">GuD</abbr> für historischen/theoretischen Kraftwerkseinsatz*

### 3.2 Deckungsbeiträge

Abbildung 6 stellt den auf Basis des Kraftwerkseinsatzes (theoretisch/historisch) ermittelten Deckungsbeitrag mit den Fixkosten gegenüber. Die Fixkosten setzen sich zusammen aus 1) den einsatzunabhängigen <abbr title="Operations and Maintenance">O&M</abbr>-Kosten auf jährlicher Basis sowie 2) den Kosten für die Abschreibung des Kapitaleinsatzes. Wie zu erwarten ergeben sich im ‚theoretischen‘ Ansatz deutlich höhere Deckungsbeiträge.

![Deckungsbeitrag im Vergleich zu den Fixkosten im theoretischen bzw. historischen Ansatz](/images/missing_money_quantitativ_historische_analyse/deckungsbeitrag_im_vergleich_zu_den_fixkosten_im_theoretischen_bzw._historischen_ansatz.png)
*Abb. 6: Deckungsbeitrag im Vergleich zu den Fixkosten im theoretischen bzw. historischen Ansatz*

Abbildung 7 illustriert das Missing Money explizit. Daraus ergibt sich ein differenziertes Bild. In der ‚theoretischen‘ Betrachtung ergeben sich Verluste von rund 5€k/MW/a für ein idealtypisches <abbr title="Gas- und Dampfkraftwerk">GuD</abbr>-Kraftwerk, Überschüsse von etwa 25 €k/MW/a für ein idealtypisches Kohlekraftwerk und Verluste von 40 €k/MW/a für eine idealtypische Gasturbine.

![Missing money in der theoretischen Betrachtung (positive Werte = Verluste)](/images/missing_money_quantitativ_historische_analyse/missing_money_in_der_theoretischen_betrachtung_positive_werte_verluste.png)
*Abb. 7: Deckungsbeitrag im Vergleich zu den Fixkosten im theoretischen bzw. historischen Ansatz*

Demzufolge fallen die Aussagen für die drei Technologien sehr unterschiedlich aus :

- <u>Ein Gas- und Dampfkraftwerk kann annähernd kostendeckend betrieben werden</u>, der Fehlbetrag von 5 €k/MW pro Jahr liegt durchaus im Unsicherheitsbereich von
- <u>Ein Kohlekraftwerk ist wirtschaftlich darstellbar</u>, die Fixkosten können rein auf Basis der Markterlöse abgedeckt werden
- <u>Der Betrieb einer Gasturbine ist auf Basis der Markterlöse nicht finanzierbar</u>, es ergeben sich zu wenig Einsatzzeiten um ausreichend Deckungsbeitrag zu erwirtschaften

Um die Bedeutung der Ergebnisse besser einordnen zu können, gibt Abbildung 10 einen Eindruck über den zeitlichen Verlauf der Erlöse. Es zeigt sich, dass die Erlöse über die Jahre hinweg sehr stark schwanken. Zum einen ist ersichtlich, dass abseits der Jahre der Energiekrise (2021+2022) für keinen Kraftwerkstyp ausreichend Deckungsbeitrag erwirtschaftet werden konnte, um die laufenden Kosten zu decken. Zum anderen hatten die Jahre der Energiekrise (2021+2022) eine signifikant positive Auswirkung auf die Erlöse aller Kraftwerkstypen.

![Gegenüberstellung von Deckungsbeitrag (CM) und Fixkosten im zeitlichen Verlauf](/images/missing_money_quantitativ_historische_analyse/gegenüberstellung_von_deckungsbeitrag_cm_und_fixkosten_im_zeitlichen_verlauf.png)
*Abb. 8: Gegenüberstellung von Deckungsbeitrag (CM) und Fixkosten im zeitlichen Verlauf*

Mit einem Blick auf den zeitlichen Verlauf der Erlöse relativieren sich daher die zuvor getroffenen Aussagen bezüglich der Rentabilität von Kraftwerkstypen stark. Unter Ausschluss der Jahre 2021+2022 wird auch für das Kohlekraftwerk ein wirtschaftlicher marktbasierter Betrieb unmöglich und das ‚missing money‘ für die gasbasierten Technologien deutlich größer.

## 4 Schlussfolgerung, Einordnung und Limitation

### 4.1 Kernaussagen

- Auf Basis der historischen Preisentwicklung ergeben sich keine starken Investitionsanreize in <abbr title="Gas- und Dampfkraftwerk">GuD</abbr>, Kohle oder <abbr title="Gas Turbine">GT</abbr>
- Die genannten Technologien können im betrachteten Zeitraum ausreichend Deckungsbeitrag zur Deckung der Fixkosten erwirtschaften.
- Diese Erkenntnis steht und fällt jedoch mit dem Auftreten des Jahres 2022 und ist äußerst sensitiv auf die Ex/Inklusion dieses Jahres

### 4.2 Limitationen

Zunächst muss festgehalten werden, dass sämtliche Aussagen nur auf Basis des hier (relativ eng) gesetzten Analyserahmens gelten und keinen Anspruch auf allgemeine Gültigkeit haben. Vor allem der begrenzte Analysezeitraum (9 Jahre) ist vor dem Hintergrund einer typischen Kraftwerkslebensdauer (25+ Jahre) relativ kurz gewählt und beinhaltet darüber hinaus eine signifikante Volatilität innerhalb des Zeitraums.

Darüber hinaus sind zumindest folgende Limitationen zu bedenken:

- **Keine Delivery Charges**: für die Berechnung der Grenzkosten auf Basis der Brennstoffkosten wurde keine Gebühr für die Lieferung von Gas/Kohle zum Kraftwerk berücksichtigt
- **Gas Preise auf Basis von TTF**
- **Annahme von günstigen Technologieparameter**: Technologiekosten entsprechen zukünftigen Werten (2030). Bei Gegenüberstellung mit historischen Preisen ergibt sich somit eine optimistische Einschätzung
- **Volle Flexibilität des Kraftwerkseinsatzes**: Alle Kraftwerkstypen können mit voller Flexibilität am Markt agieren, das ist unter Berücksichtigung von technischen Restriktionen unrealistisch
- **Effizienz bei optimaler Auslastung**: zur Berechnung der Grenzkosten wurde die maximale Effizienz bei voller Auslastung angenommen
- **Nur Spotmärkte berücksichtigt** Verkauf (Strom) nur gegen Day-ahead Preise, Forward Märkte nicht berücksichtigt. Damit ergeben sich mehr Preisspitzen
- **Berücksichtigung Jahr 2022 wurde mit 1/9 Gewicht** spricht für optimistische Betrachtung

Sämtlichen hier genannten Limitationen sprechen tendenziell für eine <u>Über</u>schätzung der Erlöse. Darüber hinaus gibt es aber auch noch Argumente, die für eine <u>Unter</u>schätzung sprechen.

- Keine Erlöse aus Regelenergie berücksichtigt
- Keine Erlöse aus Redispatch  berücksichtigt
- Keine Erlöse aus Wärmeauskopplung (für KWK)

<!-- Fußnoten -->

[^1]: [ENTSO-E Transparency Platform (Accessed: Aug. 03, 2024)  
(ENTSO-E)](https://transparency.entsoe.eu)

[^2]: [Trading Economics Gas (Accessed: Aug. 03, 2024)  
(Trading Economics)](https://tradingeconomics.com/commodity/eu-natural-gas)

[^3]: [Trading Economics Coal (Accessed: Aug. 03, 2024)  
(Trading Economics)](https://tradingeconomics.com/commodity/coal)

[^4]: [Trading Economics EU-ETS (Accessed: Aug. 03, 2024)  
(Trading Economics)](https://tradingeconomics.com/commodity/carbon)

[^5]: [Technology Data for Power and Heat Production Plants  
(Danish Energy Agency)](https://ens.dk/en/analyses-and-statistics/technology-data-individual-heating-plants)

[^6]: [Harmonised index of consumer prices (HICP)  
(Eurostat)](https://doi.org/10.2908/PRC_HICP_AIND)
