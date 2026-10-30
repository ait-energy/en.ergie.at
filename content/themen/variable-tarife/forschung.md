---
title: "Tarifbeispiele aus der Forschung"
topics: []
authors: [afischer]
showSummary: true
---

{{< katex >}}

Die wissenschaftliche Literatur sowie zahlreiche nationale und internationale Forschungs- und Demonstrationsprojekte zeigen, dass dynamische Tarifmodelle ohnehin in sehr unterschiedlichen Ausprängungen umgesetzt werden können. Im Rahmen des Projekts [INNOnet]({{< ref "projekte/INNOnet/index.md" >}}) wurde bereits eine umfangreiche Sammlung und Analyse von Netztarifen aus Forschungsprojekten durchgeführt. Die identifizierten Tarifmodelle und die zugehörigen Forschungsprojekte sind in [Tabelle 11](#tab-11) zusammengefasst. Die Analyse umfasst unter anderem die Projekte EcoGrid EU, LEAFS, E-Energy, FLEXIGRID, GridWise, InovGrid sowie weitere europäische und internationale Demonstrationsprojekte. Die Ergebnisse zeigen, dass sich die untersuchten Tarifmodelle trotz ihrer Vielfalt auf einige grundlegende Dynamisierungsansätze zurückführen lassen.

<!-- more -->

{{< alert >}}
Wir arbeiten gerade an diesem Artikel. Informationen können unvollständig oder teilweise inkorrekt sein. Fehler oder
fehlende Details kannst Du direkt per [GitHub Issue melden](https://github.com/ait-energy/en.ergie.at/issues).
Inhaltlicher Stand: Oktober 2026.
{{< /alert >}}

## Tarife aus Forschungsprojekten im Überblick {#uebersicht}

<span id="tab-11"></span>*Tabelle 11: Clustering of the grid tariffs Investigated in research projects (aus dem Projekt INNOnet)*

{{< accordion >}}
{{< accordionItem title="Tabelle 11 aufklappen" md=false >}}
<div style="overflow-x: auto;">
<table>
<colgroup>
<col style="width: 18%" />
<col style="width: 3%" />
<col style="width: 1%" />
<col style="width: 1%" />
<col style="width: 2%" />
<col style="width: 2%" />
<col style="width: 1%" />
<col style="width: 1%" />
<col style="width: 1%" />
<col style="width: 1%" />
<col style="width: 3%" />
<col style="width: 4%" />
<col style="width: 6%" />
<col style="width: 2%" />
<col style="width: 2%" />
<col style="width: 3%" />
<col style="width: 4%" />
<col style="width: 4%" />
<col style="width: 3%" />
<col style="width: 3%" />
<col style="width: 3%" />
<col style="width: 3%" />
<col style="width: 2%" />
<col style="width: 3%" />
<col style="width: 2%" />
<col style="width: 2%" />
<col style="width: 2%" />
<col style="width: 3%" />
</colgroup>
<thead>
<tr>
<th rowspan="4"><p><strong>Project</strong></p></th>
<th rowspan="4"><p><strong>Tariff</strong></p></th>
<th colspan="13" style="text-align: center;"><p><strong>Consumption Charges</strong></p></th>
<th colspan="7" style="text-align: center;"><p><strong>Injection Charges/Yields</strong></p></th>
<th colspan="3" style="text-align: center;"><p><strong>Bonus/Malus</strong></p></th>
<th colspan="3" style="text-align: center;"><p><strong>Investigation Approach</strong></p></th>
</tr>
<tr>
<th colspan="2" style="text-align: center;"><p>Fixed</p>
<p>(\(C_{+ ,x}^{F}\))</p></th>
<th colspan="2" style="text-align: center;"><p>Energy-based</p>
<p>(\(E_{+} \cdot C_{+ ,x}^{E}\))</p></th>
<th colspan="4" style="text-align: center;"><p>ToU - Energy</p>
<p>(\({E_{+ ,t} \cdot C}_{+ ,x,t}^{E}\))</p></th>
<th colspan="2" style="text-align: center;"><p>Capacity-based</p>
<p>(\(P_{+}^{Max}{\cdot C}_{+}^{P}\))</p></th>
<th style="text-align: center;"><p>ToU - Capacity (\({P_{+ ,t}^{Max} \cdot C}_{+ ,t}^{P}\))</p></th>
<th colspan="2" style="text-align: center;"><p>Tariff levels</p></th>
<th style="text-align: center;"><p>Fixed</p>
<p>(\(C_{-}^{F}\))</p></th>
<th colspan="2" style="text-align: center;"><p>Energy-based</p>
<p>(\(E_{-} \cdot C_{- ,x}^{E}\))</p></th>
<th colspan="2" style="text-align: center;"><p>ToU - Energy</p>
<p>(\({E_{- ,t} \cdot C}_{- ,x,t}^{E}\))</p></th>
<th colspan="2" style="text-align: center;"><p>Capacity-based</p>
<p>(\(P_{-}^{Max}{\cdot C}_{-}^{P}\))</p></th>
<th rowspan="3" style="text-align: center;"><blockquote>
<p>Interruptible (\(R^{I}\))</p>
</blockquote></th>
<th style="text-align: center;"><blockquote>
<p>Controllable components</p>
</blockquote></th>
<th rowspan="3" style="text-align: center;"><blockquote>
<p>Event-based (\(R^{E}\))</p>
</blockquote></th>
<th rowspan="3" style="text-align: center;"><blockquote>
<p>Manual</p>
</blockquote></th>
<th rowspan="3" style="text-align: center;"><blockquote>
<p>Automatic</p>
</blockquote></th>
<th rowspan="3" style="text-align: center;"><blockquote>
<p>Simulation</p>
</blockquote></th>
</tr>
<tr>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>E</p></th>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>E</p></th>
<th colspan="2" style="text-align: center;"><p>Dual</p></th>
<th colspan="2" style="text-align: center;"><p>Dyn</p></th>
<th style="text-align: center;"><p>Msrd</p></th>
<th style="text-align: center;"><p>Fixed</p></th>
<th style="text-align: center;"><p>Dual</p></th>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>E</p></th>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>E</p></th>
<th rowspan="2" style="text-align: center;"><p>G</p></th>
<th rowspan="2" style="text-align: center;"><p>E</p></th>
<th style="text-align: center;"><p>Msrd</p></th>
<th style="text-align: center;"><p>Fixed</p></th>
<th rowspan="2" style="text-align: center;"><blockquote>
<p>(\(R^{C}\))</p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>E</p></th>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>E</p></th>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>G</p></th>
<th style="text-align: center;"><p>G</p></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="3"><p>INNOnet</p></td>
<td><p>INN_1</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>INN_2</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>INN_3</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td rowspan="9"><p>EcoGrid EU</p></td>
<td><p>EG_1</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_2</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_3</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_4</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_5</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_6</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_7</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_8</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>EG_9</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td rowspan="6"><p>LEAFS</p></td>
<td><p>LE_1</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>LE_2</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>LE_3</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>LE_4</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>LE_5</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>LE_6</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>HiT</p></td>
<td><p>HiT</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Power-Matching-City</p></td>
<td><p>PMC</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Couperus</p></td>
<td><p>COU</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Your Energy Moment</p></td>
<td><p>YEM</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Smart Grid Gotland</p></td>
<td><p>SGG</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Aggregation of Municipal Plants</p></td>
<td><p>AMP</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>WarmUp</p></td>
<td><p>WUP</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>Tiko – Swisscom Energy Solution</p></td>
<td><p>Tiko</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>AEP Ohio gridSMART</p></td>
<td><p>AEP</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>Pacific Northwest Smart Grid</p></td>
<td><p>PNSG</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td rowspan="4"><p>E-Energy cluster of projects</p></td>
<td><p>EE_1</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>EE_2</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>EE_3</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>EE_4</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td rowspan="2"><p>Linear Project</p></td>
<td><p>LPM</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>LPA</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>InovGrid</p></td>
<td><p>IG</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td rowspan="2"><p>GridWise</p></td>
<td><p>GW_1</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>GW_2</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
</tr>
<tr>
<td><p>FlexiGrid</p></td>
<td><p>FG</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
<tr>
<td><p>ELECON</p></td>
<td><p>EL</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>-</p></td>
<td style="text-align: center;"><p>X</p></td>
</tr>
</tbody>
</table>
</div>
{{< /accordionItem >}}
{{< /accordion >}}

## Time-of-Use- und Real-Time-Pricing-Modelle {#tou-rtp}

Ein großer Teil der Forschungsaktivitäten konzentriert sich auf die Time-of-Use-Tarife. Darüber hinaus gewinnen Real-Time-Pricing-Modelle zunehmend an Bedeutung. Dabei werden Preisänderungen in kurzen zeitlichen Intervallen an Endkund:innen weitergegeben, wodurch Markt- oder Netzsignale unmittelbar wirksam werden können. Solche Ansätze bieten zwar ein hohes Flexibilitätspotenzial, erfordern jedoch eine entsprechende Mess- und Kommunikationsinfrastruktur sowie teilweise automatisierte Energiemanagementsysteme.

## Leistungs- und kapazitätsbasierte Ansätze {#leistungsbasiert}

Neben energiebezogenen Tarifen werden in der Forschung auch leistungs- und kapazitätsbasierte Ansätze untersucht. Hier orientieren sich die Kosten nicht primär an der verbrauchten Energiemenge, sondern an der beanspruchten Leistung oder an reservierten Netzkapazitäten. Solche Modelle sollen insbesondere Anreize zur Reduktion von Lastspitzen schaffen und dadurch die vorhandene Netzinfrastruktur effizienter nutzen. Im Unterschied zu klassischen Arbeitspreisen stehen hier die verursachten Netzkosten und die Inanspruchnahme von Netzkapazitäten stärker im Vordergrund.

## Hüllkurvenkonzepte {#huellkurven}

Neben klassischen energie- und leistungsbasierten Tarifmodellen werden in Forschung und Praxis zunehmend auch sogenannte Hüllkurvenkonzepte diskutiert. Dabei wird nicht direkt ein zeitabhängiger Preis vorgegeben, sondern ein zulässiger Leistungsbereich definiert, innerhalb dessen sich Verbraucher:innen oder EEGs frei bewegen können. Wird die vorgegebene Hüllkurve eingehalten, entstehen keine zusätzlichen Einschränkungen. Überschreitungen können hingegen mit höheren Entgelten, reduzierter Priorisierung oder anderen netzseitigen Maßnahmen verbunden sein. Aus Sicht der Netzbetreibenden bieten Hüllkurven den Vorteil, dass Netzgrenzen direkt berücksichtigt werden können, ohne dass dafür hochdynamische/komplexe Preissignale erforderlich sind. Gleichzeitig behalten Endkund:innen eine hohe Flexibilität hinsichtlich der konkreten Betriebsführung von Anlagen wie Wärmepumpen, Batteriespeichern oder Ladeinfrastruktur für EVs. Hüllkurven stellen somit einen alternativen Ansatz zur Flexibilitätsaktivierung dar. Während dynamische Tarife primär über wirtschaftliche Anreize wirken, definieren Hüllkurven technische Freiheitsgrade. In der Praxis sind auch Kombinationen beider Ansätze denkbar.

## Dynamische Einspeisetarife und steuerbare Lasten {#einspeisung}

Ein weiterer Forschungsschwerpunkt betrifft dynamische Einspeisetarife und netzzustandsabhängige Vergütungsmodelle für dezentrale Erzeugungsanlagen. Ziel ist es, Einspeisung stärker an den tatsächlichen Bedarf des Energiesystems anzupassen und gleichzeitig die Integration erneuerbarer Energien zu unterstützen. Ergänzend dazu werden auch Tarife untersucht, die steuerbare oder unterbrechbare Lasten berücksichtigen und dadurch Flexibilität gezielt für Netz- oder Marktzwecke nutzbar machen. Beispiele hierfür sind steuerbare Wärmepumpen, Batteriespeicher oder Ladeeinrichtungen für Elektrofahrzeuge, die als Reaktion auf Preis- oder Netzsignale ihren Betrieb anpassen.

## Zusammenfassung {#zusammenfassung}

Dynamisierung kann zusammenfassend entlang verschiedener Dimensionen erfolgen. Dazu zählen insbesondere zeitliche, leistungsbezogene, einspeisebezogene sowie netzzustandsabhängige Dynamisierungen. Gleichzeitig wird deutlich, dass unterschiedliche Tarifmodelle unterschiedliche Zielsetzungen verfolgen. Während einige Ansätze primär wirtschaftliche Effizienz adressieren, stehen bei anderen die Reduktion von Netzengpässen, die Integration erneuerbarer Energien oder die Bereitstellung von Flexibilität im Vordergrund. Insbesondere zeigen die bisherigen Forschungsarbeiten, dass zukünftige Tarifstrukturen voraussichtlich nicht auf eine einzelne Form der Dynamisierung beschränkt sein werden, sondern vielmehr unterschiedliche Ansätze miteinander kombinieren werden. Dies betrifft sowohl die Kombination von Energie- und Netztarifen als auch die mögliche Verknüpfung von dynamischen Tarifen mit netzorientierten Steuerungsansätzen wie Hüllkurven. Dadurch entstehen neue Möglichkeiten aber auch potenzielle Zielkonflikte zwischen den verschiedenen Akteur:innen des Energiesystems.
