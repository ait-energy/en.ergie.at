---
title: "Deutschland"
topics: []
authors: [afischer]
showSummary: true
weight: 4
series: ["Variable Tarife – International"]
series_order: 4
summary: "Zeitvariable Netzentgelte nach § 14a EnWG Modul 3 und der AgNes-Diskussionsvorschlag der Bundesnetzagentur."
---

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Variable Netzentgelte in Modul 3 §14a EnWG {#modul-3}

### Steuerbare Verbrauchseinrichtungen und Wahlmodule {#steuve}

Die Integration steuerbarer Verbrauchseinrichtungen (SteuVE) ist in Deutschland durch § 14a EnWG rechtlich verankert[^enwg_14a] und wurde durch die Festlegung BK6-22-300 der Bundesnetzagentur vom 27. November 2023 konkretisiert, welche seit dem 1. Januar 2024 gilt.[^bnetza_steuve] Als SteuVE gelten insbesondere Wärmepumpen einschließlich Zusatz- oder Notheizung, nicht öffentlich zugängliche Ladepunkte für Elektrofahrzeuge, Anlagen zur Raumkühlung sowie, hinsichtlich des Netzbezugs, Batteriespeicher, sofern ihre Anschlussleistung 4,2 kW übersteigt und sie im Niederspannungsnetz angeschlossen sind.

Die Regelung folgt einer regulatorischen Tauschlogik: Netzbetreiber dürfen den Netzanschluss solcher Anlagen nicht mehr unter Verweis auf eine mögliche lokale Überlastung verzögern oder ablehnen. Im Gegenzug dürfen sie bei einer konkret drohenden Netzüberlastung den Strombezug der betroffenen Anlagen vorübergehend „dimmen“. Eine Mindestleistung von 4,2 kW bleibt dabei stets gewährleistet, sodass etwa Wärmepumpen weiterbetrieben und Elektrofahrzeuge weitergeladen werden können, während der reguläre Haushaltsverbrauch von der Steuerung vollständig unberührt bleibt.[^bnetza_steuve] Als Ausgleich für die Duldung dieser Steuerung erhalten die Betreiber:innen der SteuVE ein reduziertes Netzentgelt, für dessen Ausgestaltung drei Module zur Wahl stehen, wobei sich Modul 1 und Modul 2 entschieden werden muss und Modul 3, das zeitvariable Netzentgelt, eine optionale Ergänzung zu Modul 1 darstellt.

<span id="tab-8"></span>*Tabelle 8 Übersicht der drei Wahlmodule zur Netzentgeltreduzierung nach § 14a EnWG*

| Modul 1 - Pauschale Reduzierung | Modul 2 - Prozentuale Reduzierung | Modul 3 - Zeitvariables Netzentgelt |
|----|----|----|
| Bundeseinheitlich bestimmte Pauschale je Netzbetreiber: 110–190 €/Jahr (Stand 2023); verbrauchsunabhängig. | Absenkung des Netzentgelt-Arbeitspreises (ct/kWh) für den Bezug am seperaten Zählpunkt der SteuVE auf 40 % des Standardwerts in der Niederspannung ohne Leistungsmessung. Zudem kein Netzentgelt Grundpreis für den Verbrauch am separaten Zähler. | Mehrere Zeitfenster mit drei Preisstufen (HT/NT/ST) des örtlichen Netzentgelts. Zeitfenster und Preisstufen werden kalenderjährlich festgelegt und müssen in mind. zwei Quartalen pro Jahr abgerechnet werden. Verfügbar seit April 2025. |
| Kein separater Zähler erforderlich. | Separater Zählpunkt für die SteuVE erforderlich. | Intelligentes Messsystem erforderlich |
| Wechsel zu Modul 2 möglich, jedoch nicht rückwirkend. | Wechsel zu Modul 1 möglich, jedoch nicht rückwirkend. | Nur in Kombination mit Modul 1 wählbar. Kombination mit Modul 2 ist nicht möglich. |

### Zeitvariables Netzentgelt (Modul 3) {#zeitvariables-netzentgelt}

Seit April 2025 sind Netzbetreiber verpflichtet, ein zeitvariables Netzentgelt im Sinne von Modul 3 anzubieten, das ausschließlich in Kombination mit Modul 1 gewählt werden kann.[^bnetza_steuve] Vorgesehen sind mehrere Zeitfenster mit drei Preisstufen (Hochtarif HT, Standardtarif ST, Niedertarif NT), die kalenderjährlich festgelegt werden, netzgebietsweit einheitlich gelten und in mindestens zwei Quartalen eines Jahres abgerechnet werden müssen. Ziel ist es, ohne verpflichtende Steuerungseingriffe einen ökonomischen Anreiz zur Verlagerung verschiebbarer Verbräuche in schwach ausgelastete Netzzeiten zu setzen, ohne Kund:innen mit nicht verschiebbaren Verbräuchen zu benachteiligen.

### Ausgestaltung durch die Verteilnetzbetreiber {#ausgestaltung-vnb}

Wie Verteilnetzbetreiber diesen Rahmen in der Praxis ausgestalten, wurde in einer Analyse von der Forschungsstelle für Energiewirtschaft e.V. (FfE) untersucht[^ffe_14a]. [Abbildung 14](#abb-14) visualisiert dabei die gewählten Zeitfenster von ausgewählten VNBs, die ein breites Spektrum an Netzgebieten, sowie städtische und ländliche Netzgebiete abdecken.

![Abbildung 14 Übersicht über VNB gewählte Zeiträume für Tariffenster nach §14 EnWG Modul 3 aus dem Jahr 2025](/images/variable-tarife/international/abb-14.png)

<span id="abb-14"></span>*Abbildung 14 Übersicht über VNB gewählte Zeiträume für Tariffenster nach §14 EnWG Modul 3 aus dem Jahr 2025[^ffe_14a]*

Zudem sind in [Abbildung 15](#abb-15) die Preislevels der untersuchten VNBs dargestellt.

![Abbildung 15 Übersicht über Preislevels der Tariffenster der VNB im Rahmen von §14 EnWG Modul](/images/variable-tarife/international/abb-15.png)

<span id="abb-15"></span>*Abbildung 15 Übersicht über Preislevels der Tariffenster der VNB im Rahmen von §14 EnWG Modul[^ffe_14a_tarifstufen]*

Die FfE-Analyse der Modul-3-Tarife von 12 VNB zeigt im Mittel einen Standardtarif von 7,83 ct/kWh, einen Hochtarif von 11,82 ct/kWh und einen Niedertarif von 2,19 ct/kWh, wobei die Preisspreizungen zwischen den VNB erheblich variieren (am größten bei MitNetz mit +7,52/-6,69 ct/kWh, am günstigsten der Niedertarif bei EWE Netz mit 0,49 ct/kWh) und keinem erkennbaren Muster nach Netzgebietstyp oder Region folgen. Zeitlich liegt das Hochtarif-Fenster bei den meisten VNB abends (überwiegend zwischen 17 und 21 Uhr) und das Niedertarif-Fenster nachts. Einzelne VNB legen zusätzlich ein Niedertarif-Fenster über Mittag, um den PV-Eigenverbrauch zu incentivieren. Bei Preisspreizungen über 10 ct/kWh (6 der 12 VNB) lässt sich laut FfE etwa durch verschobenes Laden eines E-Autos (60 kWh) eine Ersparnis von rund 6 € gegenüber dem Standardtarif erzielen. Voraussetzung ist stets ein intelligentes Messsystem. Die FfE verweist zudem auf mögliches Überschneidungspotenzial mit dynamischen Energiepreisen sowie zusätzliche Optimierung durch Heimenergiemanagementsysteme (HEMS). Eine Analyse von itemsnet.de[^itemsnet_zeitvariabel] zu den vorläufigen Preisblättern der 12 größten VNB (rund 45 % Marktanteil) für das Abrechnungsjahr 2026 stellt geringfügige Abweichungen zum Vorjahr fest: Die Tarifniveaus für den Hochtarif fallen 2026 insgesamt niedriger, im Quartalsvergleich sank die Hochtarif-Spanne von rund 10-17 ct/kWh (2025) auf rund 8-13 ct/kWh (2026), und nahezu alle VNB bieten die drei Tarifstufen inzwischen ganzjährig an (2025 nur ein VNB), während die gewählten Zeitfenster weiterhin stark uneinheitlich bleiben.[^itemsnet_zeitvariabel]

### Beispiele für 2026 {#beispiele-2026}

Ergänzend zu den dargestellten Informationen aus 2025, stellt [Tabelle 9](#tab-9) ein paar zufällig ausgewählten Beispiele für das Jahr 2026 dar.

<span id="tab-9"></span>*Tabelle 9 Übersicht dynamischer Netzentgelte nach §14a EnWG Modul 3 für das Jahr 2026*

| Verteilernetzbetreiber | HT & NT Zeitraum | HT-Zeitfenster | NT-Zeitfenster | ST (ct/kWh) | HT (ct/kWh) | NT (ct/kWh) |
|----|:--:|:--:|:--:|:--:|:--:|:--:|
| Westnetz[^westnetz_2026] | Q1–Q4 (ganzjährig) | 15–20 Uhr | 00–07 Uhr | 9,53 | 15,65 | 0,95 |
| Netze BW[^netze_bw_2026] | Q1–Q4 (ganzjährig) | 17–22 Uhr | 10–14 Uhr | 7,57 | 11,06 | 3,03 |
| WEMAG Netz[^wemag_2026] | nur Q1 & Q4 (Winter) | 07:00 - 11:00<br>17:00 - 20:00 | 00:00 - 06:00<br>21:00 - 00:00 | 5,13 | 7,70 | 1,95 |
| Stadtwerke Böblingen Netz[^sw_boeblingen_2026] | nur Q1 & Q4 (Winter) | 17:00 – 22:00 | 0:00 – 6:00 | 5,64 | 7,27 | 1,41 |
| Elektrizitätswerke Bad Hindelang[^ew_hindelang_2026] | Q1–Q4 (ganzjährig) | 17-20 | 23-5 | 9,83 | 14,75 | 3,69 |

<mark>Legende:</mark> ST = Standardtarif · HT = Hochtarif · NT = Niedertarif · Modul 3 = zeitvariabler Netztarif nach §14a EnWG

## AgNes Diskussionsvorschlag {#agnes}

Im Verfahren „Allgemeine Netzentgeltsystematik Strom" (AgNes) überarbeitet die deutsche Bundesnetzagentur die Netzentgeltsystematik, nachdem ein EuGH-Urteil vom 2. September 2021 eine unabhängigere Entgeltregulierung verlangte und StromNEV sowie ARegV Ende 2028 auslaufen. Die Rahmenfestlegung soll Ende 2026 abgeschlossen werden, die Anwendung erfolgt ab 1.1.2029. Da der Prozess aktuell noch nicht abgeschlossen ist, beziehen sich die folgenden Informationen auf den veröffentlichten Zwischenstand aus dem Mai 2026[^bnetza_agnes_mai_2026], welcher als fortgeschrittener Diskussionsstand, jedoch nicht als final, interpretiert werden kann. Ein wesentliches Kernelement ist die Trennung in zwei komplementäre, potenziell parallel erhobene Komponenten:

- <mark>Netzentgelte mit Finanzierungsfunktion:</mark> Sollen stabile und planbare Kostendeckung sicherstellen und dabei möglichst geringe Fehlanreize setzen. Ihr Design variiert nach Kundengruppe und unterscheidet sich im vorgeschlagenen Fall für Haushalte & Prosumer, Verbraucher:innen ab Mittelspannung, Einspeisende, Speicher, Elektrolyseure & evtl. stromintensive Industrie.

- <mark>Netzentgelte mit Anreizfunktion:</mark> Sollen gezielt netzdienliches Verhalten fördern und nicht primär der Generierung von Einnahmen dienen. Ihre genaue Ausgestaltung steht aktuell noch nicht fest; zeitlich, sowie örtlich variable Ausgestaltungen wurden aber im Prozess vorgeschlagen und das Konzept soll 2027 detailliert werden. Sie sind frühestens ab 2029 und zunächst auf höheren Netzebenen geplant.

### Örtliche Differenzierung {#oertliche-differenzierung}

Bei der örtlichen Differenzierung von Netzentgelten zeichnet sich in Deutschland damit ein Wechsel ab: weg von regionalen Unterschieden als Folge der Kostenverteilung, hin zu örtlichen Preissignalen als gezieltem Anreizinstrument. Bis Ende 2024 führte die netzgebietsbezogene Ermittlung der Netzentgelte dazu, dass Regionen mit starkem Erneuerbaren-Ausbau erhöhte Netzentgelte aufwiesen. So entfielen auf Mecklenburg-Vorpommern, Brandenburg und Schleswig-Holstein, die zusammen rund 9 % der Bevölkerung Deutschlands stellen, rund 33 % des Ausbaus von Windenergie- und Freiflächen-PV-Anlagen. Die Kosten des Netzausbaus für den Abtransport des dort erzeugten Stroms lagen damit bei den Verbraucher:innen vor Ort, was in einer Studie im Auftrag des Umweltbundesamts als ungerechte Kostenverteilung bewertet wurde.[^uba_netzkosten] Seit 1. Jänner 2025 werden diese Mehrkosten daher über einen bundesweiten Aufschlag auf alle Stromverbraucher:innen verteilt, wodurch die durch den Erneuerbaren-Ausbau bedingten regionalen Unterschiede verringert wurden.[^bnetza_netzkosten]

Die in AgNes vorgeschlagene örtliche Differenzierung folgt dagegen einer grundlegend anderen Logik. Sie soll als eigenständige Anreizkomponente, getrennt von der Finanzierungsfunktion, netzdienliches Verhalten vor und hinter Netzengpässen gezielt beeinflussen. Maßgeblich für örtliche Unterschiede wäre damit nicht mehr die Kostenstruktur eines Netzgebiets, sondern die konkrete Netzsituation, mit dem Ziel, Systemkosten wie den [Redispatchbedarf]({{< ref "wissen/redispatch/index.md" >}}) zu senken.

### Status Quo Netzentgelte mit Anreizfunktion {#anreizfunktion}

Übergeordnetes Ziel der Anreizkomponente ist es, Marktteilnehmenden in für das Netz kritischen Situationen finanzielle Signale zu geben, damit sie das Netz durch ihr Verhalten nicht zusätzlich belasten bzw. entlasten. Hintergrund ist aus Sicht der Bundesnetzagentur insb. die notwendige Reduktion des Redispatchbedarfs (die Kosten für Redispatch- und andere Engpassmaßnahmen der Übertragungsnetzbetreiber beliefen sich 2025 bereits auf 3,06 Mrd. € inkl. Vorhaltekosten für Reservekraftwerke), sowie die mit steigender Volatilität und wachsenden Preisspreads zunehmend attraktive Nutzung niedriger bzw. negativer Preise (z. B. zur Einspeicherung), obwohl das Netz den entsprechenden Strom nicht immer an den benötigten Ort transportieren kann (z.B. erhöhter Redispatchbedarf wenn aufgrund von Strommarktsignalen bei einem Netzengpass zwischen Erzeugung und Verbrauch auf der für das Netz nachteiligen Seite ein-/ausgespeist wird).

Der Vorschlag zur Ausgestaltung der Netzentgelte mit Anreizfunktion entwickelt sich im Laufe des AgNes Prozesses dynamisch, d.h. er variiert vergleichsweise stark zwischen den veröffentlichten Zwischenständen. Während im Orientierungspapier vom Dez. 2025 noch ein recht konkretes Design vorgeschlagen wurde, verweist der aktuelle Zwischenstand aus dem Mai 2026 auf einen hohen Analysebedarf, insbesondere hinsichtlich der Rückwirkungen auf den Stromgroßhandelsmarkt und den Redispatch, möglicher Umverteilungswirkungen zwischen Marktakteur:innen sowie der praktischen Umsetzbarkeit. Ein konkretes Konzept soll daher erst im Jahr 2027 entwickelt und in seinen Wirkungen untersucht werden. Als Ausgangspunkt für die Diskussion könnte dabei der Vorschlag aus dem Orientierungspapier im Dezember 2025 dienen, welcher folgende Kernelemente enthielt:

- Zeitlich (15-minütig) und räumlich variables Netzentgelt mit untersch. Preissignalen vor und hinter einem Engpass

- Symmetrisch vorzeichengerechte Anreize: z.B. positive Preise für Bezug, negative Preise (Auszahlungen) für Einspeisung

- Veröffentlichung d. Preissignale täglich vor Day-Ahead-Closure; falls kurzfristiges situatives Signal noch nicht umsetzbar ggf. Übergangslösung mit zeitvariablen Signalen & mehr Vorlaufzeit

Wie bereits beschrieben finden sich diese Konkretisierungen im aktuellen Entwurf nicht mehr wieder und diese sollen nach vertiefter Analyse in 2027 erarbeitet werden. Dennoch beschreibt die BNetzA für die Einführung bereits einen recht konkreten Zeitrahmen um den betroffenen Akteur:innen Planungssicherheit zu geben:

- Dynamische Netzentgelte für Speicher sollen frühestens 2030, möglichst aber bis 2033 eingeführt werden.

- Für Einspeisende ist eine Einführung frühestens ab 2032, möglichst aber bis 2035 vorgesehen; eine Ausnahme gilt für Offshore-Windenergieanlagen.

- Im Bereich der Niederspannung soll zügig und kontinuierlich an der Weiterentwicklung des zeitvariablen Netzentgelts für Heimspeicherbetreiber und Elektroautos weitergearbeitet werden; denkbar ist die Einbeziehung von Verbraucher:innen in der Niederspannung im Rahmen eines Opt-in, das so früh wie technisch möglich eingeführt werden soll.

- Dynamische Netzentgelte für Elektrolyseure bleiben nach einer erfolgreichen Einführung bei Speichern vorstellbar, da diese Verbraucher:innen über ein hohes Flexibilitätspotenzial verfügen und neu entstehende Elektrolyseure bei passender Standortwahl davon profitieren könnten; vor einer Einführung sollte jedoch Klarheit über die erforderlichen rechtlichen Anpassungen auf europäischer Ebene bestehen.

- Bei großen Stromverbrauchenden sind ihre Potenziale für das Netz in die Diskussion um Sondernetzentgelte für die Industrie eingebettet.

- Ab 2027 soll zudem an einem Regelwerk für Baukostenzuschüsse für Einspeisende sowie für die Implementierung von Flexible Connection Agreements (FCA) gearbeitet werden – beide Maßnahmen flankieren die mit AgNes verfolgten Ziele und sind daher bei der Abwägung zu berücksichtigen.

### Status Quo Netzentgelte mit Finanzierungsfunktion für Niederspannungskund:innen unter 100.000 kWh {#finanzierungsfunktion}

Eine weitere relevante Kundengruppe sind Niederspannungskund:innen mit einem Verbrauch von unter 100.000 kWh (typischerweise Haushalte).

Der Diskussionsstand vom Mai 2026 sieht für diese Kundengruppe im Rahmen der Netzentgelte mit Finanzierungsfunktion folgende Eckpunkte vor:

- Verpflichtender Grundpreis (€/a) und Arbeitspreis (€/kWh) als grundlegende Entgeltkomponenten.

- Prosumer zahlen zusätzlich einen Aufschlag auf den Grundpreis i. H. v. 70–90 % des regulären Grundpreises. Begründung: Die Eigenerzeugung verringert den Netzbezug und damit die über den Arbeitspreis geleisteten Finanzierungsbeiträge, senkt jedoch häufig nicht im gleichen Maße die tatsächlichen Netzkosten.

- Der Grundpreis inkl. Prosumer-Aufschlag soll 20–40 % der Erlöse des Netzbetreibers aus dieser Kundengruppe decken (gilt nicht für Balkonkraftwerke).

- Sonderentgelte für steuerbare Verbrauchseinrichtungen (§ 14a EnWG, siehe Abschnitt „[Variable Netzentgelte in Modul 3 §14a EnWG](#modul-3)“) bleiben bestehen und werden weiterentwickelt.

[^enwg_14a]: [§ 14a EnWG<br>(gesetze-im-internet.de)](https://www.gesetze-im-internet.de/enwg_2005/__14a.html)
[^bnetza_steuve]: [Steuerbare Verbrauchseinrichtungen<br>(bundesnetzagentur.de)](https://www.bundesnetzagentur.de/DE/Vportal/Energie/SteuerbareVBE/start.html)
[^ffe_14a]: [Variable Netzentgelte als Option für steuerbare Verbrauchseinrichtungen nach §14a<br>(ffe.de)](https://www.ffe.de/veroeffentlichungen/variable-netzentgelte-als-option-fuer-steuerbare-verbrauchseinrichtungen-nach-%c2%a714a/)
[^ffe_14a_tarifstufen]: [Variable Netzentgelte als Option für steuerbare Verbrauchseinrichtungen nach §14a<br>(ffe.de)](https://www.ffe.de/veroeffentlichungen/variable-netzentgelte-als-option-fuer-steuerbare-verbrauchseinrichtungen-nach-%c2%a714a/), Konkrete Preislevels sind hier tabellarisch aufgezeigt: [Übersicht der Tarifstufen<br>(ffe.de)](https://www.ffe.de/wp-content/uploads/2024/10/Uebersicht-der-Tarifstufen.pdf)
[^itemsnet_zeitvariabel]: [Zeitvariable Netzentgelte etablieren sich am Markt<br>(itemsnet.de)](https://itemsnet.de/itemsblogging/zeitvariable-netzentgelte-etablieren-sich-am-markt/)
[^westnetz_2026]: [Preisblätter Westnetz Strom 01.01.2026<br>(westnetz.de)](https://www.westnetz.de/content/dam/revu-global/westnetz/documents/ueber-westnetz/unser-netz/netzentgelte-strom/preisblaetter-westnetz-strom-01-01-2026.pdf)
[^netze_bw_2026]: [Netzentgelte Strom Netze BW GmbH 2026<br>(netze-bw.de)](https://assets.cdn.netze-bw.de/xytfb1vrn7of/7eQvxehZzn3ECbR9rALmyD/ecc795b9dcd666ce1f53d9d04362a321/netzentgelte-strom-netze-bw-gmbh-2026.pdf)
[^wemag_2026]: [Preisblatt Netzentgelte 2026<br>(wemag-netz.de)](https://www.wemag-netz.de/sites/default/files/2025-12/251208_wemag-netz-gmbh-preisblatt-netzentgelte-2026_0.pdf)
[^sw_boeblingen_2026]: [Preisblatt Strom 2026<br>(stadtwerke-boeblingen.de)](https://www.stadtwerke-boeblingen.de/files/public/133_Netze/Strom-Gasnetz/nnv_SW_B%C3%B6blingen_Preisblatt_Strom_2026_V2.pdf)
[^ew_hindelang_2026]: [Vorläufiges Preisblatt Netznutzung 2026<br>(ewhindelang.de)](https://www.ewhindelang.de/download/2026_nn-vorlaeufiges-preisblatt_hindelang_20251014.pdf)
[^bnetza_agnes_mai_2026]: [AgNes-Papier, Stand Mai 2026<br>(bundesnetzagentur.de)](https://www.bundesnetzagentur.de/SharedDocs/Pressemitteilungen/20260527_AgnesPapier.pdf?__blob=publicationFile&v=1)
[^uba_netzkosten]: [Studie im Auftrag des Umweltbundesamts<br>(openumwelt.de)](https://openumwelt.de/entities/publication/cfc01fb3-f549-4dec-99a3-6dbf84ed92fc)
[^bnetza_netzkosten]: [Verteilung von Netzkosten<br>(bundesnetzagentur.de)](https://www.bundesnetzagentur.de/DE/Fachthemen/ElektrizitaetundGas/Aktuelles/VerteilungNetzkosten/start.html)
