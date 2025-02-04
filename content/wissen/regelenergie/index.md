---
draft: true

title: "Regelenergie"
description: "Ein Überblick zum Thema Regelenergie."
topics: ["Regelenergie"]
authors:
  - "fackerl"
series: ["Strommärkte"]
series_order: 6
weight: 6
---
<!-- Grafiken -->

## Grundlagen

Um Schwankungen im Stromnetz auszugleichen und die Netzfrequenz stabil bei 50 Hertz zu halten, wird sowohl positive als auch negative Regelenergie eingesetzt. Diese wird häufig auch als Regelleistung, Regelreserve oder Regelkapazität bezeichnet. Positive Regelenergie kommt zum Einsatz, wenn der Strombedarf höher ist, als die ins Netz eingespeiste Menge. In solchen Fällen muss entweder die Stromproduktion erhöht oder der Verbrauch gesenkt werden. Negative Regelenergie hingegen wird verwendet, um einen Überschuss an Energie zu regulieren. Zu einem Überangebot kann es etwa bei Sturmlagen in der Windenergie oder Starkregen in der Wasserkraft kommen. Hierbei wird die Energie im Netz reduziert, indem entweder die Stromproduktion verringert oder der Verbrauch gezielt erhöht wird.[^1] [^4]

Regelenergie kann sowohl von Stromerzeuger:innen als auch von Stromverbraucher:innen bereitgestellt werden. Hierzu zählen beispielsweise KWK-Anlagen, Notstromaggregate, Stromspeicher, Stromwandler sowie Unternehmen, die ihren Stromverbrauch flexibel anpassen können. Für die Bereitstellung dieser Regelenergie erhalten die Anbieter:innen eine finanzielle Entschädigung. Der Markt, auf dem Regelenergie gehandelt wird, wird als Regelenergiemarkt, Regelleistungsmarkt oder Regelreservemarkt bezeichnet.[^1]

## Regelreservearten

Es wird zwischen Primärregelleistung, Sekundärregelleistung und Tertiärregelleistung unterschieden. Diese Arten der Regelenergie variieren hinsichtlich ihrer Organisation, Aktivierungszeit und Reaktionsgeschwindigkeit.[^2]

### Primärregelreserve

Die Primärregelung, auch als Primärregelleistung, Primärreserveleistung (<abbr title="Primärreserveleistung">PRL</abbr>) oder Primärregelreserve (<abbr title="Primärregelreserve">PRR</abbr>) bezeichnet, wird als erste Maßnahme eingesetzt, um die Netzfrequenz zu jeder Zeit in einem Toleranzbereich zwischen 49,99 und 50,01 Hertz zu halten. Dieser Bereich wird auch als "Totband" bezeichnet. Wird der Toleranzbereich aufgrund eines Ungleichgewichts zwischen Erzeugung und Verbrauch über- oder unterschritten, wird die Abweichung automatisch durch entsprechende Regelung von Anlagen kompensiert. Die Primärregelleistung muss innerhalb von 30 Sekunden verfügbar sein, um die unvorhergesehenen Schwankungen auszugleichen und für mindestens 15 Minuten zur Verfügung stehen. Der Markt für Primärregelreserve hat nur eine Leistungsausschreibung (siehe [Regelenergiemarkt](#regelenergiemarkt)), da Frequenzabweichungen schnell ausgeglichen werden müssen und sich die positiven und negativen Mengen oft im Durchschnitt ausgleichen. Daher ist der Aufwand für eine separate Abrechnung im Vergleich zum Nutzen zu hoch.[^5] [^6] <!--evtl unten in Kapitel Unterschiede zwischen Regelenergiearten-->
<!-- 15 oder 30 Minuten?? -->
<!-- Details zum Markteintritt für jede Reserveart..? -->

### Sekundärregelreserve

Dauert die Störung länger als 30 Sekunden, wird die Sekundärregelreserve (<abbr title="Sekundärregelreserve">SRR</abbr>) bzw. Sekundärregelleistung oder Sekundärreserveleistung (<abbr title="Sekundärreserveleistung">SRL</abbr>) aktiviert. Diese ist der <abbr title="Primärregelreserve">PRR</abbr> nachgeordnet und soll diese entlasten und dafür sorgen, dass die <abbr title="Primärregelreserve">PRR</abbr> wieder frei wird, um ihre Funktion zu erbringen. Sie muss innerhalb von 5 Minuten aktiviert werden, wobei die Aktivierung automatisch erfolgt.[^1]

### Tertiärregelreserve

Überschreitet die Störung eine Dauer von 15 Minuten oder ist die <abbr title="Sekundärreserveleistung">SRL</abbr> zu gering, um das Gleichgewicht im Netz wiederherzustellen, wird diese durch die Tertiärregelleistung (TRL), auch als Minutenreserveleistung (MRL) bezeichnet, abgelöst. Diese ist die langsamste Form der Regelenergie, sie wird entweder automatisch oder manuell aktiviert und muss erst 15 Minuten nach Abruf zur Verfügung stehen.[^3] [^9] [^10]
<!-- Next Kraftwerke->Tertiärreserve schreibt sowohl 10 als auch 15 Minuten (Überschreitungsdauer der Störung)?? -->

## Regelenergiemarkt

Die Beschaffung von Sekundär- und Tertiärregelleistung erfolgt auf nationaler Ebene. Der [Übertragungsnetzbetreiber](./wissen/akteure/index.md) und [Regelzonenführer](./wissen/akteure/index.md) <abbr title="Austrian Power Grid">APG</abbr>, als verantwortliche Instanz für die Netzregelung und den Zukauf von Regelreserven innerhalb der Regelzone Österreich, beschafft seinen Bedarf an Sekundär- und Tertiärregelenergie auf dem Regelenergiemarkt. Dieser Prozess erfolgt durch wöchentliche Ausschreibungen, die über die Plattform „RRAP – Regelreserveausschreibungsplattform der Austrian Power Grid AG“ abgewickelt werden.[^3] Die <abbr title="Austrian Power Grid">APG</abbr> schreibt ihre benötigte Regelenergie aus und Anbieter:innen können Gebote abgeben. Die Preise werden in einer [Merit-Order-Liste](./wissen/merit-order/index.md) (<abbr title="Merit-Order-Liste">MOL</abbr>) in aufsteigender Reihenfolge angeordnet.

### Arbeits- und Leistungspreis

Dabei werden Gebote für zwei voneinander unabhängige Preise abgegeben: den Leistungspreis und den Arbeitspreis. Der Leistungspreis stellt die Vergütung für die reine Bereitstellung von Regelenergie dar. Die Erzeugungs- oder Verbrauchsanlage verpflichtet sich, die angebotene Regelenergie während der vereinbarten Zeitscheibe jederzeit abrufbereit zu halten. Für diese garantierte Verfügbarkeit wird ein fester Preis pro Megawatt (Leistungspreis) entrichtet. Die Vergütung für die im Bedarfsfall tatsächlich abgerufene Energie wird als Arbeitspreis bezeichnet und pro bereitgestellter Megawattstunde gezahlt.[^1] [^3] Beide Preise werden im Rahmen eines [Pay-as-Bid-Verfahrens](./wissen/pay-as-bid/index.md) festgelegt, bei welchem Anbieter:innen genau den von ihnen gebotenen Preis erhalten.[^7] Seit Oktober 2018 wird dem Leistungsfaktor ein sogenannter zusätzlicher Gewichtungsfaktor aufgerechnet, der miteinbezieht, wie wahrscheinlich es ist, dass die Energie tatsächlich eingesetzt wird. Dies wird als Mischpreisverfahren bezeichnet. [^4]
<!-- Mehr Details? Noch gültig? -->

Im Rahmen der Ausschreibungen erhalten die Anbieter:innen mit den niedrigsten Gebotspreisen für den Leistungspreis den Zuschlag für die Bereitstellung der Regelenergie. Wird die Regelenergie tatsächlich in Anspruch genommen, werden aus dem Pool der zugeschlagenen Anbieter:innen diejenigen mit den niedrigsten gebotenen Arbeitspreisen zur Erbringung der Regelenergie ausgewählt.[^1] [^4]

### Unterschiede zwischen den Regelreservearten

Im Falle der Sekundärregelleistung findet die Beschaffung über Ausschreibungen zwar national innerhalb der Regelzone Österreich statt, der eigentliche Abruf passiert jedoch über eine Kooperation mit dem deutschen Regelenergiemarkt. Die bezuschlagten Angebote werden zu einer gemeinsamen Merit Order Liste zusammengeführt, welche als Common Merit-Order-List (<abbr title="Common Merit-Order-List">C-MOL</abbr>) bezeichnet wird. Diese beinhaltet die entsprechenden Zuschläge sowohl für den österreichischen als auch für den deutschen Bedarf an SRL.[^7]
<!-- C-MOL nur für Sekundär, oder? (doublecheck), noch aktuell, dass TRL rein national ist? ... Unterschied C-MOL zu Imbalance Netting... -->

Die Tertiärregelung wird vollständig auf nationaler Ebene durchgeführt.[^8] Die Primärregelung hingegen erfolgt zentralisiert über den zentraleuropäischen Übertragungsnetzbetreiber [ENTSO-E](./wissen/akteure/index.md) (European Network of Transmission System Operators for Electricity) in Zusammenarbeit mit anderen [Übertragungsnetzbetreibern](./wissen/akteure/index.md).[^5]

<!-- evtl. Erlöse & geeignete Bereitsteller -->

### Weitere Informationen

- Kapitel 3 und 10 der [Sonstigen Marktregeln Strom](https://www.e-control.at/bereich-recht/soma-strom)
- [Marktbasierte Beschaffung Regelreserve](https://www.e-control.at/industrie/strom/strommarkt/marktbasierte-beschaffung-regelreserve)
- Die Verordnung zur [Festlegung einer Leitlinie über den Systemausgleich im Elektrizitätsversorgungssystem (EB Guideline)](https://www.e-control.at/marktteilnehmer/strom/network-codes-und-guidelines) der Europäischen Kommission gibt den Rahmen für die nationale Beschaffung und Abrechnung sowie internationale Kooperationsprojekte vor

<!-- evtl. andere Seiten vom Kompendium verlinken -->

[^1] [A1 Energy Solutions: Regelenergie kurz erklärt](https://www.a1energysolutions.at/regelenergie-pool/)
[^2] [APCS: Regelenergie](https://www.apcs.at/de/regelenergie)
[^3] [APG: Netzregelung](https://markt.apg.at/netz/netzregelung/)
[^4] [Next Kraftwerke: Regelenergie in Österreich](https://www.next-kraftwerke.at/wissen/regelenergie#vorhaltung-und-einsatz-der-regelleistung)
[^5] [Next Kraftwerke: Was ist Primärreserveleistung?](https://www.next-kraftwerke.at/wissen/primaerregelung-prl)
[^6] [APG: Primärregelung (PRR)](https://markt.apg.at/netz/netzregelung/primaerregelung/)
[^7] [Next Kraftwerke: Sekundärregelung (SRL)](https://www.next-kraftwerke.at/wissen/sekundaerregelung-srl)
[^8] [Regelleistung.net: FAQ Regelleistung](https://www.regelleistung.net/xspproxy/api/staticfiles/regelleistung/regelleistung_files/faqregelleistung.pdf)
[^9] [Next Kraftwerke: Tertiärregelung](https://www.next-kraftwerke.at/wissen/tertiaerregelung-trl)
[10] [E-Control: Regelreserve und Ausgleichsenergie](https://www.e-control.at/marktteilnehmer/strom/strommarkt/regelreserve-und-ausgleichsenergie)
