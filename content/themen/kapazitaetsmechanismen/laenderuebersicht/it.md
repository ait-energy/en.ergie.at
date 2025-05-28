---
title: "Italien"
topics: []
authors: ["afischer"]
---

<br>
{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
{{< /alert >}}

## Marktweiter Kapazitätsmechanismus mit zentralem Käufer

### Ausschreibung

Der italienische Kapazitätsvergütungsmechanismus basiert auf der Versteigerung von [Zuverlässigkeitsoptionen]({{< ref "themen/kapazitaetsmechanismen/ausgestaltungsfaktoren.md" >}}#zuverlaessigkeitsoptionen), ähnlich dem [irischen]({{< ref "themen/kapazitaetsmechanismen/laenderuebersicht/ie.md" >}}) Markt. Die Zielmenge an [Zuverlässigkeitsoptionen]({{< ref "themen/kapazitaetsmechanismen/ausgestaltungsfaktoren.md" >}}#zuverlaessigkeitsoptionen) wird vom Übertragungsnetzbetreiber festgelegt und entspricht der Zielkapazität des Systems. Die vergebenen Kapazitäten erhalten den Wert der [Zuverlässigkeitsoptionen]({{< ref "themen/kapazitaetsmechanismen/ausgestaltungsfaktoren.md" >}}#zuverlaessigkeitsoptionen) und sind finanziell für deren Abwicklung verantwortlich [^1], [^2]. Der neue italienische <abbr title="Kapazitätsmechanismus">KM</abbr> ist ein mengenbasiertes, marktwirtschaftliches Schema zur Beschaffung von Zuverlässigkeitsoptionsverträgen durch den Systembetreiber. Die Auktion verwendet ein descending-clock Format über 21 Runden, wobei die Gesamtkapazität in jeder Runde gleich bleibt, der Preis jedoch gesenkt werden kann. Gewinnergebote werden zu einem einheitlichen Clearing-Preis bezahlt. Die Auktionsfrequenz umfasst Hauptauktionen, gefolgt von Sekundärauktionen, wobei Sekundärhandel bis zu einem Monat vor Lieferung innerhalb derselben Gebotszone erlaubt ist. Der Preisdeckel wird durch eine obere Schätzung der Kosten für Neueintritt (Cost of New Entry, <abbr title="Open Cycle Gas Turbines">OCGT</abbr>) festgelegt, etwa 90.000 €/MWy. Die Deckel für bestehende Kapazitäten reichen von 25.000 bis 45.000 €/MWy, was den jährlichen festen Betriebskosten von kombinierten Gasturbinen (<abbr title="Combined Cycle Gas Turbine">CCGT</abbr>) entspricht, während die Deckel für neue Kapazitäten mit der <abbr title="Cost of New Entry">CONE</abbr>-Schätzung von 75.000 bis 95.000 €/MWy übereinstimmen [^1]. Die Auktion berücksichtigt Übertragungsbeschränkungen und führt zu unterschiedlichen Kapazitätspreisen für jede italienische Zone, ähnlich dem [Day-Ahead-Markt]({{< ref "wissen/markt-day-ahead/index.md" >}}). Kapazitätsanbieter müssen eine Verfügbarkeit über einem bestimmten Verhältnis, wie beispielsweise 80%, für mindestens einen bestimmten Bruchteil eines Monats, wie 75%, aufrechterhalten. Bei Nichterfüllung dieser Anforderung werden die Kapazitätszahlungen vorübergehend ausgesetzt, und bei systematischer Nichtlieferung kann es zur Rückzahlung der Zahlungen und zum Einzug der Kapazitätsrechte kommen. Obwohl es keine spezifischen Testvorschriften gibt, hat jede Technologie einen zugehörigen Verfügbarkeitsfaktor, um die Zuverlässigkeit zu gewährleisten.

### Teilnahme

Alle bestehenden und neuen Kapazitäten im italienischen System, einschließlich der Nachfrageflexibilität und Speicher, können am Kapazitätsmarkt teilnehmen. Die Teilnahme ist freiwillig, jedoch müssen Ressourcen, die von anderen Unterstützungsmaßnahmen profitieren, diese aufgeben, um anspruchsberechtigt zu sein. Die Teilnahme von grenzüberschreitender Kapazität hängt von der Umsetzung von grenzüberschreitenden Ausgleichsvereinbarungen ab. Für Anbieter von <abbr title="Demand Response">DR</abbr> gibt es eine vereinfachte Abrechnung; wie alle anderen Kapazitätsanbieter sind sie jedoch für Nicht-Erfüllungsgebühren haftbar. Der <abbr title="Übertragungsnetzbetreiber">ÜNB</abbr> kann die Nachfrageflexibilität direkt abschalten, wenn diese während Engpassperioden den Dispatch-Anweisungen nicht folgt. Die Vertragslaufzeiten variieren: In den Anfangsausschreibungen erhalten bestehende Kapazitäten Einjahresverträge, während neue Kapazitäten für 15 Jahre vertraglich gebunden werden. In der vollständigen Implementierungsphase werden bestehende Kapazitäten für 3 Jahre und neue Kapazitäten weiterhin für 15 Jahre vertraglich gebunden. Anpassungsauktionen gelten für einen Einjahreslieferzeitraum.

### Vergütung

Im italienischen Mechanismus erhalten Kapazitätsanbieter Auktionsprämien als Zahlungen. Sie müssen auch eine [Zuverlässigkeitsoptionen]({{< ref "themen/kapazitaetsmechanismen/ausgestaltungsfaktoren.md" >}}#zuverlaessigkeitsoptionen) abwickeln, indem sie die Differenz zwischen einem Referenzpreis, der sich auf die Day-Ahead- und Balancing-Preise stützt, und einem Ausübungspreis (strike price) von 125 €/MWh zahlen, der die Grenzkosten einer Spitzenlast-<abbr title="Open Cycle Gas Turbines">OCGT</abbr>-Einheit widerspiegelt. Für ausländische Kapazitäten ist der Referenzpreis aufgrund der derzeit fehlenden grenzüberschreitenden Ausgleichsvereinbarungen der Day-Ahead-Preis. Die Rückzahlungsverpflichtung für Kapazitätsanbieter erfolgt lastbasiert, was bedeutet, dass sie nur für den Anteil der Kapazität zahlen, der während Engpassperioden benötigt wird. Händler finanzieren den <abbr title="Kapazitätsmechanismus">KM</abbr>, indem sie die Differenz zwischen der Kapazitätsprämie und den Erlösen aus den Zuverlässigkeitsoptionen zahlen, proportional zu ihrem Beitrag zur Spitzenlast.

<!-- Fußnoten -->

[^1]: A. Papavasiliou, “Overview of EU Capacity Remuneration Mechanisms,” 2021.  
[^2]: Terna, “Capacity market - Terna spa.” Accessed: Apr. 11, 2024. [Online]. Available: https://www.terna.it/en/electric-system/capacity-market
