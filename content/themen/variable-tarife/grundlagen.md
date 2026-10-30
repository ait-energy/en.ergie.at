---
title: "Begriffs- und Systemrahmen"
topics: []
authors: [afischer]
showSummary: true
summary: "Begriffe, Bestandteile des Strompreises und Gestaltungsdimensionen von Tarif- und Entgeltkomponenten."
---

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Betrachtungsfokus {#betrachtungsfokus}

Das Projekt [DyTEG](https://projekte.ffg.at/projekt/008a523e-f36b-1410-864f-00d3c07d99bb) untersucht, wie sich dynamische Tarif- und Preiskomponenten auf [Energiegemeinschaften]({{< ref "wissen/energiegemeinschaften/index.md" >}}) (EGs) und ihre Teilnehmer:innen auswirken. Daraus leitet sich der Betrachtungsfokus dieser Seiten ab: Im Vordergrund stehen Endkund:innen, die an das [Niederspannungsnetz (Netzebene 7)]({{< ref "wissen/stromnetz/index.md" >}}) angeschlossen sind, und hier insbesondere Haushalte. Ausdrücklich eingeschlossen sind Prosumer mit PV-Anlage sowie Haushalte mit flexiblen Verbrauchseinrichtungen oder Speichern (z. B. Wärmepumpe, Elektrofahrzeug, Heimspeicher), da gerade diese Gruppe im Kontext der variablen Preissignale relevant ist. Darüber hinaus werden kleinere Gewerbebetriebe und Gemeinden berücksichtigt, die ebenfalls typische EG-Teilnehmende sind. Da EG-Teilnehmende häufig sowohl Strom beziehen als auch einspeisen, werden Bezugs- und Einspeiseseite gleichermaßen betrachtet.

## Begriffsdefinitionen {#begriffe}

### Zeitliche Differenzierung (Dynamisch vs. Variabel) {#zeitliche-differenzierung}

Die Begriffe „dynamisch“, „variabel“ und „zeitvariabel“ werden in der öffentlichen Diskussion und teilweise auch in der wissenschaftlichen Literatur häufig synonym oder ohne klare Abgrenzung voneinander verwendet. Um eine einheitliche und präzise Terminologie sicherzustellen, werden im Folgenden die nachstehenden Begriffe definiert:

- <mark>Statisch-zeitvariabel (kurz „zeitvariabel“)</mark> sind Komponenten, deren Arbeits- (ggf. auch Leistungs-)preis nach vorab festgelegten, in der Regel langfristig (saisonal, jährlich) bekannt gegebenen Zeitfenstern differenziert wird (z. B. Hoch-/Niedertarifzeiten nach Tageszeit, Wochentag oder Saison), innerhalb dieser Zeitfenster jedoch konstant bleibt. Die Zeitfenster und Preisniveaus orientieren sich an antizipierten, typischen Mustern der (z.B. der Netzauslastung bzw. -einspeisung im Falle der Netzentgelte oder durchschnittlichen Großhandelspreisen im Falle der Energiekomponente) und werden nicht kurzfristig an die tatsächliche Systemsituation angepasst. Diese Definition erfolgt in Analogie zur Verwendung der BNetzA im AgNes Prozess.[^bnetza_agnes_dynamisierung]

- <mark>Dynamisch-zeitvariabel (kurz „dynamisch“)</mark> sind Komponenten, deren Preisverlauf kurzfristig, mit einem Vorlauf von höchstens wenigen Tagen bis hin zu untertägiger bzw. echtzeitnaher Anpassung, auf Basis der tatsächlichen oder unmittelbar bevorstehenden Situation (z.B. lokalen bzw. regionalen Netzauslastung oder Großhandelspreise) festgelegt wird. Anders als bei (statisch-)zeitvariablen Komponenten ist der Zeit und / oder Preisverlauf nicht langfristig im Voraus fixiert, sondern reagiert zeitnah auf das konkrete Geschehen (z. B. Auslastung von Transformatoren oder Leitungsabschnitten in einem bestimmten Netzbereich).

In einer DENA[^dena_dynamische_tarife] Studie werden dynamische Tarife ergänzend als Teilmenge zeitvariabler Tarife beschrieben (ein dynamischer Tarif ist demnach stets auch zeitvariabel, wobei „dynamisch“ lediglich eine präzisere Charakterisierung darstellt). Diese Definition ist zwar formal korrekt, dennoch sollen die beiden Begriffe hier klar voneinander abgegrenzt verwendet werden, um Missverständnisse zu vermeiden: Wie oben beschrieben liegt das eigentliche Abgrenzungskriterium darin, wann bzw. wie kurzfristig vor dem tatsächlichen Verbrauch der Preis festgelegt wird, weshalb hier sowohl „zeitvariabel“ als auch „dynamisch“ ausschließlich die oben definierten, eigenständigen Bedeutungen tragen.

Zudem ist zu erwähnen, dass neben der zeitlichen Differenzierung auch eine örtliche (geographische) Differenzierung möglich ist. Diese kann entweder als strukturelle, kostenbasierte regionale Differenzierung (z. B. unterschiedliche Netzentgelthöhen aufgrund unterschiedlicher Kosten in den jeweiligen Bundesländern Österreichs) oder als gezielte, anreizorientierte örtliche Differenzierung als Steuerungsinstrument (wie vorgeschlagen im AgNes Prozess in DE, siehe Abschnitt „[AgNes Diskussionsvorschlag]({{< ref "themen/variable-tarife/international/de.md#agnes" >}})“) ausgestaltet werden, bei der durch unterschiedliche Tarifhöhen ein gewünschtes Verhalten der Nutzer:innen erreicht werden soll. Für den Kontext der Wechselwirkung von variablen Tarifen mit Energiegemeinschaften ist jedoch insbesondere die zeitliche Differenzierung relevant, weshalb sich die folgenden Betrachtungen im Wesentlichen auf diese fokussieren.

### Tarife vs. Preise {#tarife-vs-preise}

Wie in Abschnitt „[Zeitliche Differenzierung](#zeitliche-differenzierung)“ beschrieben, ist die zeitliche Differenzierung sowohl auf der Netz- als auch auf der Energieseite ein zentrales Thema. Bereits die Gesetzessprache selbst verwendet für beide Seiten unterschiedliche, aber ähnlich klingende Begriffe: Während das ElWG auf der Netzseite von „zeitvariablen Netznutzungsentgelten“ spricht (§ 128 Abs. 3 und 4 ElWG), definiert es auf der Energieseite den „Liefervertrag mit dynamischen Energiepreisen“. Im allgemeinen Sprachgebrauch werden beide Konstrukte jedoch häufig unter dem Sammelbegriff „(dynamischer) Tarif“ zusammengefasst.

Bei einer Gegenüberstellung beider Seiten entsteht daraus ein reales Missverständnisrisiko: Ohne weitere Kennzeichnung lässt sich aus der Formulierung „Tarif“ oder „Preis“ allein nicht erkennen, ob die Netz- oder die Energiekomponente gemeint ist. Das liegt auch an der allgemeinen Wortbedeutung selbst: Ein „Tarif“ bezeichnet üblicherweise die, meist aus mehreren Komponenten wie Grund-, Arbeits- und/oder Leistungspreis bestehende, übergeordnete Entgeltstruktur eines Angebots, während ein „Preis“ den konkreten Betrag einer einzelnen dieser Komponenten bezeichnet. Diese allgemeine Bedeutung lässt eine Verwendung in beiden Kontexten zu und schafft damit keine Klarheit von selbst.

Um dieses Risiko auszuschließen, wird hier durchgängig zwischen beiden Begriffen unterschieden:

- <mark>(Netz)tarif</mark> wird auf diesen Seiten vornehmlich im Netzkontext verwendet und bezeichnet die Entgeltstruktur für das Netz. „Netztarif“ wird dabei synonym zum in § 127 Abs. 2 ElWG verwendeten Begriff „Netzentgelt“ gebraucht.

- <mark>(Energie)preis</mark> wird auf diesen Seiten vornehmlich im Kontext von Energiepreisen auf der Energieseite verwendet. Die Verwendung des Begriffs „Tarif“ auf der Energieseite wird vermieden um Missverständnisse zu vermeiden. Mehrere solcher Preiskomponenten bilden gemeinsam das Preismodell des jeweiligen Liefervertrags.

Diese Konvention dient ausschließlich der Eindeutigkeit innerhalb dieser Seiten und dem Ziel Klarheit zu schaffen und Missverständnisse zu vermeiden.

## Überblick allgemeine Bestandteile des Strompreises {#bestandteile}

Der von Endkund:innen gezahlte Strompreis setzt sich aus mehreren regulatorisch und ökonomisch unterschiedlich determinierten Komponenten zusammen, die sich in Preisbildung, Beeinflussbarkeit und regulatorischer Zuständigkeit grundlegend unterscheiden:

| Block | Preisbildung | Zuständigkeit | Beeinflussbar durch Kund:in? |
|----|----|----|----|
| Energiepreis | Markt (Wettbewerb) | Lieferant | Ja - durch Anbieter- und Preismodellwahl |
| Netzentgelte | Reguliert (SNE-VO nach ElWOG, künftig SNE-G-V und SNE-T-V nach ElWG) | [Netzbetreiber]({{< ref "wissen/akteure/index.md" >}}) (standortgebunden) | Nein - keine freie Netzbetreiberwahl (natürliches Monopol) |
| Steuern & Abgaben | Hoheitlich festgelegt | Bund / Gemeinde | Nein |

Strukturell entfiel in der Vergangenheit (insb. vor 2022) näherungsweise je rund ein Drittel des Gesamtpreises auf jeden Block, dieses Verhältnis schwankt dabei deutlich mit dem Großhandelspreisniveau der Energiekomponente, welche gerade in den Energiekrisenjahren 2022/2023, bedingt durch die hohen Großhandelspreise, einen höheren Anteil hatte. Eine typische Verteilung für einen Haushalt in Österreich ist in [Abbildung 1](#abb-1) dargestellt.

![Abbildung 1 Überblick über die prozentuale Aufteilung des Endkundenpreises für einen Haushalt in Österreich 2026](/images/variable-tarife/grundlagen/abb-01.jpeg)

<span id="abb-1"></span>*Abbildung 1 Überblick über die prozentuale Aufteilung des Endkundenpreises für einen Haushalt in Österreich 2026[^econtrol_preise]*

Für die Analyse von Dynamisierungen ist diese Dreiteilung ein zentraler Ausgangspunkt, weil sie gerade auf Energie und Netzseite jeweils anderen Logiken und Akteur:innen unterliegt.

## Grundlegende Ausgestaltungsoptionen von Tarifkomponenten {#tarifkomponenten}

Die in Abschnitt „[Überblick allgemeine Bestandteile des Strompreises](#bestandteile)“ beschriebenen Preisblöcke Energiepreis, Netzentgelte und staatliche Abgaben sind ihrerseits keine monolithischen Größen, sondern bestehen aus Tarifkomponenten mit unterschiedlichen Bemessungsgrundlagen und Abrechnungslogiken. Für die Analyse von Dynamisierungsoptionen ist das Verständnis dieser Grundkomponenten eine notwendige Voraussetzung, denn nicht jede Komponente lässt sich gleich gut dynamisieren (oder soll überhaupt dynamisiert werden), und die Art der Bemessungsgrundlage bestimmt maßgeblich, welche Anreize ein Tarif erzeugt und erzeugen soll.

Grundsätzlich lassen sich Typen von Tarifkomponenten unterscheiden, die sich nach ihrer Bemessungsgrundlage, der Abrechnungslogik und den erzeugten Verhaltenswirkungen voneinander abgrenzen

| Preisart | Bemessungs-grundlage | Einheit | Abrechnungslogik |
|----|----|----|----|
| Arbeitspreis | Entnommene / eingespeiste Energiemenge | ct/kWh | Abrechnung auf Basis der tatsächlich verbrauchten oder eingespeisten Energiemenge (mengenbasiert) |
| Leistungspreis | Tatsächlich gemessene Leistung (z. B. Spitzenleistung) | €/kW | Abrechnung anhand definierter Leistungswerte (z. B. Tages-, Monats-/ Jahreshöchstleistung, durchschnittliche Spitzenwerte oder Spitzenlasten in leistungsstarken Zeiträumen) |
| Kapazitätspreis | Vorab vertraglich vereinbarte Leistung | €/kW | Leistungsbasierte Abrechnung im Buchungszeitraum; Überschreitungen führen zu Pönalen oder Anpassung; ggf. stufenbasierte oder anschlussbezogene Kapazität |
| Grundpreis | Pauschaler Fixbetrag (nutzungs-unabhängig) | €/a (bei Jahres-abrechnung) | Täglich, monatlich oder jährlich erhoben; unabhängig von Netzinanspruchnahme |

Quelle: AIT-BMWET Speicherstudie[^bmwet_stromspeicher]

<mark>Verbrauchsbasierte Komponenten (Arbeitspreis)</mark> bemessen sich an der tatsächlich entnommenen oder eingespeisten Energiemenge in kWh. Sie erzeugen direkte Mengenanreize: Wer weniger oder zu günstigeren Zeiten verbraucht, zahlt weniger. Damit eignen sie sich grundsätzlich gut als Träger dynamischer Preissignale. Eine zeitliche Variation des Arbeitspreises setzt unmittelbar finanzielle Anreize zur Lastverschiebung oder Verbrauchsreduktion.

<mark>Leistungs- und kapazitätsbasierte Komponenten (Leistungspreis, Kapazitätspreis)</mark> bemessen sich dagegen nicht an der konsumierten Menge, sondern an der beanspruchten oder vorab kontrahierten Leistung in kW. Ihre systemökonomische Berechtigung ergibt sich daraus, dass die Netzinfrastruktur auf die maximal gleichzeitig auftretende Last ausgelegt sein muss. Kapazitätsvorhaltung verursacht Fixkosten unabhängig von der tatsächlichen Nutzungsdauer. Leistungsbasierte Entgelte internalisieren diesen Zusammenhang direkt und setzen im Vergleich zu einem leistungsunabhängigen Grundpreis einen Anreiz zur [Spitzenlastreduktion]({{< ref "wissen/peakshaving/index.md" >}}). Eine Dynamisierung dieser Komponenten, etwa durch zeitlich variable Leistungspreise oder durch die Auswahl des abrechnungsrelevanten Leistungswertes in einem Zeitraum ist in der Praxis wenig verbreitet, kann jedoch strukturell präzise und wirksame Anreize zur Spitzenlastreduzierung setzen.

<mark>Fixe Grundentgelte</mark> decken administrativen und anschlussgebundenen Grundaufwand und dienen der stabilen Kostendeckung unabhängig vom Nutzungsverhalten. Sie entfalten keine verbrauchs- oder leistungsbezogenen Verhaltensanreize, sondern sichern eine angemessene Grundbeteiligung der Netznutzenden.Gerade im Haushaltsbereich und in Ländern in denen noch kein flächendeckender Smart Meter Ausbau erreicht wurde, sind Grundentgelte einen verbreitete Komponente.

In der Praxis werden diese Komponenten nicht isoliert eingesetzt, sondern in Kombinationen, die je nach regulatorischer Zielsetzung, Verbrauchersegment und verfügbarer Messtechnologie variieren. Für die nachfolgende Analyse ist entscheidend: Jede der beschriebenen Grundkomponenten kann im Prinzip einer zeitlichen oder räumlichen Variation unterzogen werden und unterscheidet sich in Anforderungen an Messtechnik, regulatorischen Rahmen und erzeugten Anreizwirkungen.

## Zusammenfassung: Gestaltungsdimensionen von Tarif- und Entgeltkomponenten {#gestaltungsdimensionen}

Aus den vorangegangenen Abschnitten ergibt sich ein mehrdimensionaler Gestaltungsraum, der sich entlang von fünf grundlegenden Dimensionen beschreiben lässt, welcher im folgenden zusammenfassend dargestellt ist:

1.  <mark>Art der Differenzierung</mark>: Die in Abschnitt „[Zeitliche Differenzierung](#zeitliche-differenzierung)“ eingeführte Unterscheidung zwischen zeitlicher und örtlicher sowie zwischen statischer und dynamischer Ausgestaltung. Im Ergebnis vier mögliche Grundformen (statisch- bzw. dynamisch-zeitvariabel, statisch- bzw. dynamisch-ortsvariabel).

2.  <mark>Preisblock und die Flussrichtung</mark>: Wie in Abschnitt „[Überblick allgemeine Bestandteile des Strompreises](#bestandteile)“ dargestellt, gliedert sich der Endkundenpreis in Energiepreis, Netzentgelte und Steuern & Abgaben. Jeder dieser Blöcke kann theoretisch sowohl auf der Bezugs- als auch auf der Einspeiseseite anfallen, wobei in der Praxis bisher überwiegend die Bezugsseite betroffen ist.

3.  <mark>Tarifkomponente</mark>: Die in Abschnitt „[Grundlegende Ausgestaltungsoptionen von Tarifkomponenten](#tarifkomponenten)“ beschriebenen Komponenten: Arbeits-, Leistungs- und Kapazitätspreis, Grundpreis sowie Anschlussentgelt, wobei Arbeits- und Leistungspreis zusätzlich eine Mengenschwellenlogik (Preisänderung ab einem definierten Verbrauchs- bzw. Leistungswert) enthalten können.

4.  <mark>Primäre Wirkung</mark> einer Komponente: Sie kann auf Spitzenlastreduktion oder Lastverschiebung zielen, einen längerfristigen Investitionsanreiz setzen oder, wie insbesondere bei klassischen Grundpreisen, primär der Kostendeckung dienen und damit anreizfrei sein.

5.  <mark>Zugang aus Nutzer:innensicht</mark>: verpflichtend, freiwillig wählbar (Opt-in) oder optional im Austausch gegen eine Gegenleistung, wie etwa bei § 14a EnWG.

Die fünf Dimensionen sind nicht vollständig unabhängig voneinander, und nicht jede theoretische mögliche Kombination ist praktisch relevant oder überhaupt sinnvoll (ein einmaliges Anschlussentgelt etwa kann nicht dynamisch-zeitvariabel ausgestaltet sein).

Die Beschriebene Kodierung wird in Abschnitt „[Zusammenfassung und Vergleich der Praxisbeispiele]({{< ref "themen/variable-tarife/international/vergleich.md" >}})“ benutzt um die im folgenden Abschnitt „[Internationale Beispiele variabler Netzentgelte]({{< ref "themen/variable-tarife/international.md" >}})“ gesammelten Tarife strukturiert und übersichtlich zusammenzufassen. Diese Übersicht macht sie sichtbar, welche Dimensionskombinationen in der internationalen Praxis vorwiegend verwendet werden oder bislang nicht oder kaum vorkommen und bilden die Grundlage für die Analyse von wahrscheinlichen Dynamisierungen in Österreich.

[^bnetza_agnes_dynamisierung]: [AgNes – Orientierungspunkte Dynamisierung (Kap. 5.1)<br>(bundesnetzagentur.de)](https://www.bundesnetzagentur.de/DE/Beschlusskammern/GBK/GBK_Termine/Downloads/2026/01_2026/14_01/AgNes_Orientierungspunkte_Dynamisierung.pdf?__blob=publicationFile&v=4)
[^dena_dynamische_tarife]: [Was sind dynamische Stromtarife?<br>(dena.de)](https://www.dena.de/fileadmin/dena/Publikationen/PDFs/2024/Was_sind_dynamische_Stromtarife.pdf)
[^econtrol_preise]: [Strom- und Gaspreise<br>(e-control.at)](https://www.e-control.at/konsumenten/strom-gas-preise)
[^bmwet_stromspeicher]: [Stromspeicher<br>(bmwet.gv.at)](https://www.bmwet.gv.at/Services/Publikationen/publikationen-energie/stromspeicher.html)
