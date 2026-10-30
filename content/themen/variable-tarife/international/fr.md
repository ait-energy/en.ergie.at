---
title: "Frankreich"
topics: []
authors: [afischer]
showSummary: true
weight: 2
series: ["Variable Tarife – International"]
series_order: 2
summary: "Der französische Netztarif TURPE 7 mit saisonalen Haupt- und Schwachlastzeiten sowie optionalen zeit- und ortsabhängigen Netzentgelten für Speicher."
---

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## TURPE 7 {#turpe-7}

### Komponenten {#komponenten}

Der Netztarif TURPE 7 trat am 1. August 2025 für einen Zeitraum von vier Jahren in Kraft und wurde durch die CRE-Deliberation Nr. 2025-13 vom 30. Januar 2025 validiert. Er regelt die Netztarife zur Kompensation der Kosten der Übertragungs- & Verteilernetzbetreiber. Der Tarif setzt sich aus vier Komponenten zusammen, welche in [Tabelle 4](#tab-4) am Beispiel einer:eines typischen privaten Kund:in dargestellt sind[^fournisseurs_turpe]. Die variable Komponente (CSV) wird im weiteren Verlauf dieser Seite noch detaillierter ausgeführt.

<span id="tab-4"></span>*Tabelle 4 Übersicht über Komponenten des TURPE7 Netztarifs und beispielhafte Höhe für eine:einen typischen Privatkund:in[^fournisseurs_turpe]*

| Komponente | Höhe |
|----|----|
| Verwaltungsgebühr (Composante de Gestion, CG) | 16,80 €/Jahr |
| Messgebühr (Composante de Comptage, CC) | 22,00 €/Jahr |
| Fixe Bezugskomponente (Composante de Soutirage Fixe, CSF) | 10,11 €/kVA/Jahr (Tarifkundengruppe CU4) |
| Variable Bezugskomponente (Composante de Soutirage Variable, CSV) | Abh. von Verbrauch in Zeitfenstern (siehe [Tabelle 6](#tab-6)) |

### Zeitfenster und Preiskoeffizienten {#zeitfenster}

Seit dem 1. August 2024 wird die variable Bezugskomponente auf vier Zeitfenster aufgeteilt, die sich aus der Kombination von zwei Saisons und jeweils zwei Lastzeiten (Peak/Off-Peak) ergeben. Die nachfolgende [Tabelle 5](#tab-5) stellt diese Struktur dar.

<span id="tab-5"></span>*Tabelle 5 Übersicht der Tariffenster in TURPE7*

|  | Hochsaison / Saison Haute (H)<br>01.11. - 31.03. | Niedrigsaison / Saison Basse (B)<br>01.04. - 31.10. |
|----|:--:|:--:|
| Hauptlastzeiten / Heures Pleines (HP) | HPH | HPB |
| Schwachlastzeiten / Heures Creuses (HC) | HCH | HCB |

Vom lokalen Verteilernetzbetreiber werden entsprechend der dargestellten Aufteilung zwei Hoch und Niederfenster ausgewiesen, welche in der Tarifhöhe saisonal unterschiedlich sind, jedoch bezogen auf die Uhrzeiten konstant bleiben. Pro Tag gibt es 8 Niederstunden (wovon 5 in der Nacht liegen müssen) und 16 Hochstunden, welche auf Definition der französischen Regulierungsbehörde CRE in den in [Abbildung 12](#abb-12) dargestellten Zeiträumen verteilt werden können.

![Abbildung 12 Übersicht über mögliche Zeitfenster für Niedrigtariffenster für Netzentgelte in Frankreich (übersetzt aus )](/images/variable-tarife/international/abb-12.png)

<span id="abb-12"></span>*Abbildung 12 Übersicht über mögliche Zeitfenster für Niedrigtariffenster für Netzentgelte in Frankreich (übersetzt aus [^cre_faq_hp_hc])*

Die Höhe der Netzentgelte in den entsprechenden Zeiträumen wird zentral von der Regulierungsbehörde festgelegt. [Tabelle 6](#tab-6) zeigt die jeweiligen Preiskoeffizienten.

<span id="tab-6"></span>*Tabelle 6 Übersicht der TURPE7-Koeffizienten je Tarifkundengruppel (FTA) (übersetzt und adaptiert aus[^fournisseurs_turpe] )*

| FTA[^fta] | Beschreibung | CSF (€/<br>kVA/a) | HPH<br>Hoch Winter<br>\[ct/kWh\] | HCH<br>Niedrig Winter<br>\[ct/kWh\] | HPB<br>Hoch Sommer<br>\[ct/kWh\] | HCB<br>Niedrig Sommer<br>\[ct/kWh\] |
|----|----|:--:|:--:|:--:|:--:|:--:|
| CU4 | Kurznutzung (≤ 36 kVA) | 10,11 | 7,49 | 3,97 | 1,66 | 1,16 |
| MU4 | Mittlere Nutzung (≤ 36 kVA) | 12,12 | 7,00 | 3,73 | 1,61 | 1,11 |
| LU | Langzeitnutzung (Großverbraucher) | 93,13 | 1,25 | 1,25 | 1,25 | 1,25 |

Kund:innen im Hoch- und Höchstspannungsnetz (HTA/HTB) unterliegen einem zusätzlichen Spitzenlastzeitfenster namens „Pointe Fixe/mobil“ - von Anfang Dezember bis Ende Februar-, ergänzend und verschärfend zum HPH- und HCH-Tarif.[^bet_netzentgelte_europa]

## Optionale zeitvariable Netzentgelte für Speicher in Frankreich {#speicher}

Ein anschauliches Beispiel für die gezielte Beanreizung von Speichern in einem Netzentgeltsystem liefert Frankreich mit der Reform seines Entgeltregimes „TURPE 7“[^cre_turpe7_deliberation], die im August 2026 wirksam wird[^modo_turpe7]. Neu eingeführt wird dabei eine optionale, orts- und zeitabhängige Tarifkomponente, über die Batteriespeicher für ein netzdienliches Verhalten belohnt werden. Grundlage dieser regulatorischen Logik ist die Identifikation jener Netzgebiete, die strukturell von Einspeise- oder Verbrauchsspitzen betroffen sind. Eine Übersicht der kategorisierten Netzknoten ist in [Abbildung 13](#abb-13) dargestellt. So werden etwa in Regionen mit hoher Solarerzeugung Anreize gesetzt, damit Speicher rund um die Mittagszeit Energie aufnehmen, während in nachfragestarken Regionen umgekehrt Anreize zur Einspeisung während winterlicher Lastspitzen bestehen. Da für die Speicher somit sowohl bei der Einspeisung als auch beim Verbrauch Netzentgelte anfallen, entsteht ein entsprechendes Lenkungssignal. Über diese zeit- und standortabhängigen Entgeltsignale sollen Batteriespeicher gezielt zum Abbau lokaler Netzengpässe beitragen und die Integration erneuerbarer Energien erleichtern[^modo_turpe7]. Zunächst betroffen sind Speicher auf den Netzebenen HTA, HTB1 und HTB2. Dabei handelt es sich bei HTA um die Mittelspannungs-Verteilnetzebene mit rund 20 kV, bei HTB1 um die Hochspannungs-Subtransmissionsebene mit 63/90 kV und bei HTB2 um die regionale Hochspannungs-Übertragungsebene mit 150/225 kV.[^energy_storage_news_fr]

![Abbildung 13 Übersicht Einspeise- oder Konsumgeprägter Netzknoten im Rahmen der TURPE7 Netzentgelte für Speicher in Frankreich](/images/variable-tarife/international/abb-13.png)

<span id="abb-13"></span>*Abbildung 13 Übersicht Einspeise- oder Konsumgeprägter Netzknoten im Rahmen der TURPE7 Netzentgelte für Speicher in Frankreich*

[^fournisseurs_turpe]: [TURPE : tout savoir sur le tarif d'utilisation des réseaux<br>(fournisseurs-electricite.com)](https://www.fournisseurs-electricite.com/contrat-electricite/prix/turpe)
[^cre_faq_hp_hc]: [FAQ Heures pleines / Heures creuses<br>(cre.fr)](https://www.cre.fr/fileadmin/Documents/Communiques_de_presse/2025/250206_FAQ_HP-HC.pdf)
[^fta]: FTA: „Formule Tarifaire d'Acheminement“ ist eine vom Netzbetreiber zugeordnete Tarifkundengruppe
[^bet_netzentgelte_europa]: [Vergleich der Netzentgelte und Netzentgeltsystematiken in Europa für Strom<br>(bet-consulting.de)](https://www.bet-consulting.de/fileadmin/redaktion/PDF/Studien_und_Gutachten/Gutachten_Vergleich_der_Netzentgelte_und_Netzentgeltsystematiken_in_Europa_f%C3%BCr_Strom.pdf)
[^cre_turpe7_deliberation]: [Délibération n° 2025-78 – TURPE 7 HTA-BT<br>(cre.fr)](https://www.cre.fr/fileadmin/Documents/Deliberations/2025/250313_2025-78_Post-CSE_TURPE_7_HTA-BT.pdf)
[^modo_turpe7]: [France grid tariff fee for batteries (TURPE 7)<br>(modoenergy.com)](https://modoenergy.com/research/en/france-grid-tariff-fee-battery-turpe)
[^energy_storage_news_fr]: [France introduces grid tariff reforms for energy storage<br>(energy-storage.news)](https://www.energy-storage.news/france-introduces-grid-tariff-reforms-for-energy-storage/)
