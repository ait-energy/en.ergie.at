---
title: "Einspeiseentgelte"
topics: []
authors: [afischer]
showSummary: true
weight: 6
series: ["Variable Tarife – International"]
series_order: 6
summary: "Standortabhängige Einspeisenetzentgelte in Irland, Großbritannien und Rumänien."
---

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Irland {#irland}

In Irland existiert ein Einspeisenetzentgelt für Erzeugungsanlagen \>5MW im Übertragungs- und Verteilernetz. Der sogenannte GTUoS-Tarif (Generator Transmission Use of System Tarif) besteht aus zwei Komponenten: einem pauschalen „Postage Stamp“-Anteil (mind. 70 %) und einem standortabhängigen Anteil (max. 30 %). Der pauschale Anteil wird gleichmäßig auf alle Erzeuger verteilt, während der standortabhängige Teil auf Faktoren wie Stromflüsse, Netzkonfigurationen, Erzeugungsniveaus, geplante Netzinvestitionen und Interkonnektorflüssen basiert, die sich jährlich ändern. Die GTUoS-Tarife fallen tendenziell höher in Regionen aus, die weit von großen Verbrauchsschwerpunkten entfernt liegen, sowie in Netzgebieten, in denen bereits eine hohe Anzahl von Erzeugungsanlagen errichtet wurde oder sich in Planung befindet. Dies betrifft insbesondere den Nordwesten und Südwesten Irlands.[^soni_gtuos]

In Irland sind Erzeugungsanlagen mit einer installierten Leistung von weniger als 5 MW von Netzentgelten für die Einspeisung befreit. Um eine Diskriminierung zwischen Erzeugern unterschiedlicher Größe zu vermeiden, wird dieser Freibetrag von 5 MW grundsätzlich allen Erzeugungsanlagen gewährt. Netzentgelte werden daher lediglich auf den Teil der installierten Leistung erhoben, der 5 MW übersteigt. Eine Erzeugungsanlage mit einer installierten Leistung von 7 MW wird beispielsweise nur für 2 MW (7 MW − 5 MW) veranlagt.[^acer_price_signals]

Die Einführung des standortbezogenen Elements geht auf das Ziel zurück, Erzeuger an den Kosten der von ihnen verursachten Netzverstärkungen zu beteiligen. Das Ziel ist es, effizientere Investitionsentscheidungen bei der Standortwahl zu fördern. Aktuell ist nicht geplant den variablen Anteil zu erhöhen, da andere Instrumente wie Anschlussentgelte weiterhin als Hauptquelle für standortbezogene Signale gesehen werden.[^acer_price_signals]

Eine Übersicht über die anlagenspezifischen GTUoS-Charges wird veröffentlicht, zuletzt die für das Jahr 2025/2026.[^eirgrid_gtuos]

## Großbritannien {#grossbritannien}

### Übertragungsnetzentgelte für Einspeiser (TNUoS) {#tnuos}

In Großbritannien existiert ein Einspeisentgeld für Erzeuger im Übertragungsnetz. Die sogenannten Transmission Network Use of System Charges (TNUoS) dienen der Finanzierung der Kosten für Bau, Betrieb und Instandhaltung des Übertragungsnetzes. Die Entgelte werden durch den National Energy System Operator (NESO) erhoben und unterscheiden sich je nach Standort und Netznutzung der Erzeugungsanlage.

TNUoS-Entgelte werden nicht pauschal von allen Einspeisern erhoben, sondern hängen von der Anschlussart sowie der vertraglich vereinbarten Einspeisekapazität (Transmission Entry Capacity, TEC) ab. Direkt an das Übertragungsnetz angeschlossene Erzeugungsanlagen mit einem Bilateral Connection Agreement (BCA) sind grundsätzlich entgeltpflichtig. Bei dezentral angeschlossenen („embedded“) Erzeugungsanlagen mit Bilateral Embedded Generation Agreement (BEGA) gilt eine Freigrenze von 100 MW TEC. Anlagen unterhalb dieser Schwelle entrichten keine TNUoS-Entgelte. Erzeugungsanlagen mit BELLA-Vertrag (Bilateral Embedded Licence Exempt Agreement) oder ohne direkten Vertrag mit NESO zahlen ebenfalls keine TNUoS-Gebühren.[^neso_tnuos] Damit richtet sich das britische Einspeisentgeltsystem primär an große Erzeugungsanlagen. Kleine und mittlere dezentrale Anlagen, insbesondere typische PV-Dachanlagen von Haushalten, fallen nicht unter die TNUoS-Entgeltpflicht.

Die eigentlichen Einspeiseentgelte im britischen TNUoS-System bestehen aus einer Kombination aus einer geografisch differenzierten Hauptkomponente („Wider Tariff“) und zusätzlichen lokalen Netzkostenkomponenten. Die Wider-Tarif-Komponente bildet die netzseitigen Auswirkungen des Anlagenstandorts ab. Hierfür wird Großbritannien in 27 Erzeugungszonen unterteilt, denen unterschiedliche Tarife zugeordnet sind. Die Höhe des Entgelts hängt insbesondere vom Standort der Anlage, der vertraglich vereinbarten Einspeisekapazität (TEC) sowie teilweise von der Erzeugungstechnologie ab. Ziel ist es, langfristige Standortsignale zu setzen und die Kosten des Übertragungsnetzes verursachungsgerecht auf Erzeugungsanlagen zu verteilen. Ergänzend werden lokale Netzkosten über Local Circuit Tariffs und Local Substation Tariffs verrechnet, welche die Nutzung der konkret in Anspruch genommenen Leitungs- und Umspannwerksinfrastruktur widerspiegeln. Sämtliche Tarifkomponenten werden auf Basis der vertraglich vereinbarten Einspeisekapazität (TEC) in £/kW berechnet und gemeinsam als jährliches Einspeisenetzentgelt erhoben.[^neso_tnuos] Die finalen Tarife werden anschließend veröffentlicht.[^neso_tnuos_final]

### Verteilernetzentgelte für Einspeiser (DNUoS) {#dnuos}

Für die Verteilernetzentgelte in Großbritanien wird unterschieden zwischen CDCM (LV/HV-Anschlüsse) und EDCM (EHV-Anschlüsse). Diese gelten sowohl für Bezug als auch für Einspeisung, auf dieser Seite werden jedoch lediglich die Einspeiseentgelte fokussiert. Die Berechnungslogik wird festgelegt im Distribution Connection and Use of System Agreement (DCUSA)

#### CDCM (LV/HV-Anschlüsse) {#cdcm}

CDCM (Schedule 16 DCUSA): Das CDCM-Modell ordnet Kunden bestimmten Kundengruppen (Customer Categories, ca. 30) zu. Jede dieser Gruppen erhält einen eigenen Netztarif. Die Zuordnung erfolgt anhand gemeinsamer Merkmale wie Größe des Anschlusses, Messkonzept (Metering), Spannungsebene und weiterer technischer Eigenschaften. Ein Netztarif kann aus bis zu sieben verschiedenen Entgeltbestandteilen bestehen, wobei nicht jeder Kunde alle Bestandteile zahlt. Zu diesen Entgelten gehören bis zu drei Arbeitspreise (Unit Rate 1, 2 und 3) in Pence pro Kilowattstunde (p/kWh), eine feste tägliche Grundgebühr (Fixed Charge), ein Kapazitätsentgelt auf Basis der vereinbarten Anschlussleistung (Capacity Charge), ein Entgelt für die Überschreitung der vereinbarten Kapazität (Exceeded Capacity Charge), sowie ein Blindleistungsentgelt (Reactive Power Charge) in Pence pro kVArh. Die drei Arbeitspreise entsprechen unterschiedlichen Zeitfenstern des Verteilnetzbetriebs (Timebands), nicht jeder Tarif enthält alle möglichen Bestandteile.[^dcusa_cdcm] Da die in DCUSA Schedule 16, Paragraph 71[^dcusa_schedule16] festgelegte Berechnungsformel für die Arbeitspreis-Komponente (Unit Rate, p/kWh) von Erzeugungstarifen einen negativen Faktor enthält, ist dieser Tarifbestandteil bei jeder CDCM-Erzeugungstarifierung strukturell als Gutschrift (negativer Wert) ausgestaltet. Dies betrifft jedoch nur die Arbeitspreis-Komponente – etwaige Fixed-Charge- oder Blindleistungs-Komponenten der Erzeugungstarife können davon unabhängig positive (belastende) Werte annehmen. Beispiele für die höhe der Gutschrift für verschiedene DSOs und mit Gültigkeit ab 01.04.2025 sind in [Tabelle 10](#tab-10) aufgezeigt, wobei angenommen wird, dass die Einspeisung in der Customer Category „LV Generation Aggregated“ stattfindet. In dieser Kundengruppe werden über alle dargestellten DSOs auch keine weiteren Tarifbestandteile erhoben, das heißt es fällt rein der negative Arbeitspreis an, welcher statisch-zeitvariabel in 3 Zeitfenstern aufgegliedert ist.

<span id="tab-10"></span>*Tabelle 10 Übersicht der CDCM Tarifhöhen verschiedener DSOs aus dem UK*

| DSO | Tariflevel AP |
|----|----|
| Northern Powergrid[^npg_charging] | Weekdays:<br>-6.763 p/kWh (16:00 - 19:30 Uhr)<br>-1.124 p/kWh (08:00 - 16:00 und 19:30 - 22:00)<br>- 0.220 p/kWh (00:00 - 08:00 und 22:00 - 24:00)<br>Saturdays & Sundays:<br>- 0.220 p/kWh |
| Eastern Power Networks[^epn_charging]; Scottish & Southern Electricity Networks[^ssen_charging] | Weekdays:<br>-8.615 p/kWh (16:00 - 19:00 Uhr)<br>-0.982 p/kWh (07:00 - 16:00 und 19:00 - 23:00)<br>-0.165 p/kWh (00:00 - 07:00 und 23:00 - 24:00)<br>Saturdays & Sundays:<br>-0.165 p/kWh |
| National Grid (South West)[^nged_charging] | Weekdays:<br>-16.000 p/kWh (17:00 - 19:00 Uhr)<br>-1.048 p/kWh (07:30 - 17:00 und 19:00 - 21:30)<br>- 0.130 p/kWh (00:00 - 07:30 und 21:30 - 24:00)<br>Saturdays & Sundays:<br>-0.165 p/kWh |
| Electricity North West[^enwl_charging] | Weekdays:<br>- 11.359 p/kWh (16:00 - 19:00 Uhr)<br>- 2.024 p/kWh (09:00 - 16:00 und 19:00 - 20:30)<br>- 0.088 p/kWh (00:00 - 09:00 und 20:30 - 24:00)<br>Saturdays & Sundays:<br>- 2.024 p/kWh (16:00 - 19:00)<br>- 0.088 p/kWh (00.00 - 16.00 und 19.00 - 24.00) |

#### EDCM (EHV-Anschlüsse) {#edcm}

EDCM: Anders als das CDCM bildet das EDCM keine Kundengruppen, sondern berechnet für jeden einzelnen an das EHV-Netz (Spannungen ≥22 kV bzw. innerhalb der Grenze einer HV-Umspannstation) angeschlossenen Kunden ein individuelles ("bespoke") Tarifpaket aus bis zu vier Entgeltkomponenten: je ein Fixentgelt (p/Tag), ein Kapazitätsentgelt (p/kVA/Tag), ein Überschreitungsentgelt (p/kVA/Tag) und ein "Super-Red"-Arbeitspreis (p/kWh, in bestimmten Stunden, meist Abends zwischen Nov und Feb) jeweils getrennt für Bezug ("Import") und Einspeisung ("Export"). Zur Ermittlung des kostenreflektiven, standortspezifischen Entgeltanteils ("Charge 1") existieren zwei alternative, in Schedule 17[^edcm_fcp] (Forward Cost Pricing, FCP) bzw. Schedule 18[^edcm_lric] (Long Run Incremental Cost) geregelte Berechnungsmethoden, die sich ausschließlich in einen Berechnungsschritt unterscheiden, während alle übrigen Tarifelemente identisch ermittelt werden. Analog zum CDCM-Erzeugungstarife ist auch im EDCM der Arbeitspreis ("Super-Red") in allen in [Tabelle 10](#tab-10) dargestellten DSOs 0 oder negativ, es werden aber zudem die anderen Bestandteile mit positiven Kosten erhoben. Die genauen Ausprägungen lassen sich den verlinkten Dokumenten in den Fußnoten aus [Tabelle 10](#tab-10) entnehmen.

## Rumänien {#rumaenien}

Seit dem Jahr 2025 erhebt Rumänien ein Einspeisenetzentgelt für Erzeugungsanlagen mit einer installierten Leistung von mehr als 5 MW, die an das Verteilnetz angeschlossen sind. Hintergrund ist, dass in einzelnen Regionen mit hoher Erzeugungskonzentration erhebliche Stromflüsse in andere Netzgebiete auftreten, wodurch zusätzliche Verluste im 110-kV-Verteilnetz entstehen. Die betroffenen Kosten wurden zuvor ausschließlich über die Entnahmeentgelte der jeweiligen Netzgebiete finanziert.

Die rumänische Regulierungsbehörde ANRE entwickelte gemeinsam mit den Verteilnetzbetreibern (DSO), dem Übertragungsnetzbetreiber (TSO) sowie einem externen Berater eine Methodik zur Ermittlung jener Netzverluste, die durch regionale Einspeiseüberschüsse verursacht werden. Grundlage bildet eine Unterteilung des Landes in acht geografische Netzregionen, die unabhängig von den Konzessionsgebieten der Verteilnetzbetreiber definiert wurden. Das Einspeisenetgelt wird ausschließlich in jenen Regionen erhoben, in denen ein signifikanter Überschuss an Erzeugung gegenüber dem lokalen Verbrauch festgestellt wird. Zum Zeitpunkt der Einführung im Jahr 2025 waren zwei der acht Netzregionen betroffen. Die dort geltenden Einspeiseentgelte entsprachen 6 % bzw. 17 % der jeweiligen Entnahmeentgelte für die Netznutzung. Nach Angaben von ANRE wurde die Maßnahme nach einem längeren Konsultationsprozess mit den betroffenen Erzeugern umgesetzt und von den Marktakteuren grundsätzlich akzeptiert.[^erra_anre]

[^soni_gtuos]: [2025/26 Proposed GTUoS Tariffs NI<br>(soni.ltd.uk)](https://cms.soni.ltd.uk/sites/default/files/publications/2526%20Proposed%20GTUoS%20Tariffs%20NI%20Final.pdf)
[^acer_price_signals]: [Getting price signals right: fair and cost-reflective electricity network tariffs<br>(acer.europa.eu)](https://www.acer.europa.eu/news/getting-price-signals-right-fair-and-cost-reflective-electricity-network-tariffs)
[^eirgrid_gtuos]: [2025/26 Approved GTUoS Tariffs IE<br>(eirgrid.ie)](https://cms.eirgrid.ie/sites/default/files/publications/2526_Approved_GTUoS_Tariffs_IE_v1.0.pdf)
[^neso_tnuos]: [TNUoS Charges – Guidance<br>(neso.energy)](https://www.neso.energy/document/138046/download)
[^neso_tnuos_final]: [Final TNUoS Tariffs<br>(neso.energy)](https://www.neso.energy/document/353086/download)
[^dcusa_cdcm]: [CDCM Annual Review Pack v6 (Kapitel 2.3ff)<br>(dcusa.co.uk)](https://dcusa-cdn-1.s3.eu-west-2.amazonaws.com/wp-content/uploads/2024/10/25150956/CDCM-ARP_v6_20241025.pdf)
[^dcusa_schedule16]: [DCUSA Schedule 16<br>(dcusa.co.uk)](https://document.dcusa.co.uk/dcusa-document/150/635258?)
[^npg_charging]: [Northern Powergrid (Northeast) 2025-26 LC14 Charging Statement<br>(northernpowergrid.com)](https://www.northernpowergrid.com/sites/default/files/assets/Northern%20Powergrid%20(Northeast)%20-%20%202025-26%20LC14%20Charging%20Statement%20-%20v0.2.pdf)
[^epn_charging]: [Eastern Power Networks LC14 Statement 2025<br>(ukpowernetworks.co.uk)](https://media.umbraco.io/ukpn-cms/gqufhepd/eastern-power-networks-lc14-statement-2025-v1-7.pdf)
[^ssen_charging]: [SEPD Embedded Networks DUoS Charges 2025-2026<br>(ssen.co.uk)](https://www.ssen.co.uk/globalassets/library/charging-statements-sepd/202526/sepd-embedded-networks-duos-charges-2025-2026_v0.2.pdf)
[^nged_charging]: [National Grid (South West) Charging Statement<br>(nationalgrid.co.uk)](https://commercial.nationalgrid.co.uk/downloads-view-reciteme/687752)
[^enwl_charging]: [ENWL LC14 Statement 2025<br>(enwl.co.uk)](https://www.enwl.co.uk/globalassets/about-us/regulatory-information/documents/current-charging-information/25-26/enwl-lc14-statement-2025_v1.0-final.pdf)
[^edcm_fcp]: [EDCM FCP v9 (Schedule 17)<br>(dcusa.co.uk)](https://dcusa-cdn-1.s3.eu-west-2.amazonaws.com/wp-content/uploads/2025/11/06124046/EDCM-FCP_v9_20251106.pdf)
[^edcm_lric]: [EDCM LRIC v9 (Schedule 18)<br>(dcusa.co.uk)](https://dcusa-cdn-1.s3.eu-west-2.amazonaws.com/wp-content/uploads/2025/11/06124039/EDCM-LRIC_v9_20251106.pdf)
[^erra_anre]: [Case study from ANRE Romania on injection charge for producers connected to distribution networks<br>(erranet.org)](https://erranet.org/case-study-from-anre-romania-on-injection-charge-for-producers-connected-to-distribution-networks-featured-in-erra-spring-newsletter-2025/)
