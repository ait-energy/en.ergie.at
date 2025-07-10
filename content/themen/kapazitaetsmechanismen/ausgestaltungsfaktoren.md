---
title: "Ausgestaltungsfaktoren von Kapazitätsmärkten"
topics: []
authors: ["afischer", "sfanta"]
---
Kapazitätsmechanismen sind komplexe Instrumente zur Gewährleistung der Versorgungssicherheit in Strommärkten. Sie bestehen aus einer Vielzahl ineinandergreifender Elemente, deren Ausgestaltung erheblich variiert. Diese Seite bietet einen systematischen Überblick über zentrale Gestaltungsaspekte wie das [Auktionsdesign](#auktionsdesign), die [Definition und Zertifizierung von Kapazität](#kapazitätsdefinition), [Derating-Faktoren](#derating) sowie [vertragliche Rahmenbedingungen](#vertragsparameter). Darüber hinaus werden Fragen der [Vergütungsstruktur](#verguetungsstruktur), [Kostenallokation](#kostenallokation) und [institutionellen Zuständigkeiten](#governance) beleuchtet. Anhand konkreter Beispiele aus europäischen Ländern werden unterschiedliche Mechanismendesigns dargestellt, um ein besseres Verständnis für deren Aufbau, Funktionen und praktische Umsetzung zu ermöglichen.

{{< timeline >}}

<a id="auktionsdesign"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Auktionsdesign ====================== -->
{{< timelineItem icon="scale-balanced" header="Auktionsdesign" subheader="Preisfindung, Teilnahme, Zuteilung" >}}

<ul>
  <li><strong>Preisfindung:</strong> Einheitspreisauktionen („uniform pricing“) zahlen allen erfolgreichen Bietern den Clearing-Preis des letzten akzeptierten Gebots (z. B. Irland, UK). Im Gegensatz dazu erhalten Bieter im Pay-as-bid-Verfahren (z. B. Schwedens strategische Reserve) die individuell gebotenen Preise – dies fördert strategisches Bietverhalten, reduziert aber Mitnahmeeffekte.</li>

  <li><strong>Teilnahmebedingungen:</strong> Auktionen sind oft formal technologieneutral, werden jedoch durch Kriterien wie De-rating-Faktoren oder Umweltanforderungen (z. B. CO₂-Grenzwerte in Polen, Belgien) faktisch differenziert.</li>

  <li><strong>Auktionsfrequenz:</strong> Häufig werden Hauptauktionen Jahre (z.B. T-4) vor dem Lieferzeitraum abgehalten (z. B. UK, Irland), ergänzt durch T-1-Zusatzauktionen zur kurzfristigen Nachsteuerung.</li>

  <li><strong>Zuteilung:</strong> Erfolgt über zentrale Clearing-Mechanismen auf Basis von Preis, Standort oder Systemdienlichkeit. Verwendet werden entweder Nachfragekurven (z. B. Irland) oder kombinatorische Constraints zur Berücksichtigung von Netzrestriktionen (z. B. Belgien).</li>
</ul>

{{< /timelineItem >}}

<a id="kapazitätsdefinition"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Kapazitätsdefinition & Zertifizierung ====================== -->
{{< timelineItem icon="graduation-cap" header="Kapazitätsdefinition & Zertifizierung" subheader="Technologieneutralität & Kriterien" >}}

<ul>
  <li><strong>Technologieneutraler Zugang:</strong> Ziel, alle Technologien – von konventionellen Kraftwerken über Speicher bis Demand Response (DR) – einzuschließen, praktisch aber oft eingeschränkt.</li>
  <li><strong>Technische Anforderungen:</strong> Anfahrtszeiten, Mindestverfügbarkeiten (z. B. ≤ 12 h in Deutschlands strategischer Reserve) oder Anschluss an Spannungsebenen ≥ 110 kV (strategische Reserve Deutschland).</li>
  <li><strong>Neuheitsanforderung:</strong> Neuheit der Kapazität oder erhöhung der installierten Leistung (z.B. um ≥ 20 % oder Wechsel des Energieträgers bei Ausschreibungen in Frankreich).</li>
  <li><strong>Umweltkriterien:</strong> CO₂-Grenzwerte für teilnahmeberechtigte Einheiten (z. B. 550 g CO₂/kWh in Belgien).</li>
  <li><strong>Systemdienliche Eigenschaften:</strong> Speicherfähigkeit, Hybridisierbarkeit, netzstützende Funktionen (z. B. im Netzanschluss-Auktionskriteriensystem in Spanien).</li>
  Die konkrete Ausgestaltung entscheidet, ob die angestrebte Technologieneutralität praktisch gewährleistet oder durch implizite Anforderungen eingeschränkt ist.
</ul>

{{< /timelineItem >}}

<a id="derating"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Derating-Faktoren ====================== -->
{{< timelineItem icon="triangle-exclamation" header="Derating-Faktoren" subheader="Verfügbarkeitsbewertung & Normierung" >}}

<ul>
  <li><strong>Zweck:</strong> Abbildung der erwartbaren Verfügbarkeit einer Kapazitätseinheit in systemkritischen Stunden zur technologieübergreifenden Vergleichbarkeit.</li>
  <li><strong>Herleitung:</strong> Empirisch auf Basis historischer Verfügbarkeitsdaten oder simulationsgestützten Szenarien.</li>
  <li><strong>Technologie-Unterschiede:</strong> Hohe Derating-Werte für regelbare Kraftwerke (z. B. CCGT); deutlich geringere Werte für PV/Wind; Demand Response teils mit pauschalen Faktoren oder Zusatzanforderungen (z. B. Italien).</li>
  <li><strong>Einsatz in Auktionen:</strong> Normierung von Angebotsmengen und Aggregation des zu beschaffenden Kapazitätsvolumens (z. B. Irland, UK, Belgien).</li>
  <li><strong>Differenzierung & Aktualisierung:</strong> Technologie- oder anlagenspezifische Faktoren, meist jährlich oder vor jeder Auktionsrunde angepasst, um Technologiefortschritte und Systembedarfe zu berücksichtigen.</li>
</ul>

{{< /timelineItem >}}

<a id="vertragsparameter"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Vertragsparameter ====================== -->
{{< timelineItem icon="edit" header="Vertragsparameter" subheader="Laufzeit, Verfügbarkeit, Aktivierung & Integration" >}}

<ul>
  <li><strong>Laufzeit:</strong> Neue Kapazitäten erhalten teils langfristige Verträge (bis zu 15 Jahre in Italien, 10 Jahre in Irland), während bestehende Anlagen meist kürzer gebunden sind (z. B. 3 Jahre in Italien, 1 Jahr in Irland). Diese Differenzierung soll neue Investitionen fördern, kann aber zu Ungleichbehandlung führen.</li>

  <a id="zuverlaessigkeitsoptionen"
   style="display:block; position:relative; top:-4rem; visibility:hidden;">
  </a>
  <li><strong>Zuverlässigkeitsoptionen (Reliability Options):</strong> Ein Mechanismus, bei dem Kapazitätsanbieter regelmäßige Zahlungen erhalten – im Gegenzug verpflichten sie sich, in Zeiten von Stromknappheit Energie bereitzustellen oder eine finanzielle Ausgleichszahlung zu leisten, wenn ein vorher definierter Preis (Strike-Preis) überschritten wird. Das Modell sichert Anbieter stabile Einnahmen, schützt Verbraucher vor extremen Preisspitzen und stärkt die Versorgungssicherheit, ohne in die Strompreisbildung des Spotmarkts direkt einzugreifen.

  </li> <li><strong>Verfügbarkeitsverpflichtungen & Sanktionen:</strong> Je nach Markt unterscheiden sich die Ansätze: In Belgien oder Schweden gelten konkrete technische Anforderungen an die Verfügbarkeit als vertraglich fixierte Bedingung. In anderen Ländern wie Irland oder dem Vereinigten Königreich kommen überwiegend finanzielle Steuerungsinstrumente zum Einsatz – etwa Sanktionen bei Nichtverfügbarkeit oder verpflichtende Ausgleichszahlungen bei Systemstress, unabhängig vom Mechanismus selbst.</li>

  <li><strong>Marktintegration:</strong> Marktweite Mechanismen binden Kapazitäten eng an den Strommarkt, während strategische Reserven bewusst vom Markt isoliert werden – was Marktverzerrungen vermeiden, aber die effiziente Ressourcennutzung einschränken kann.</li>
</ul>

{{< /timelineItem >}}

<a id="verguetungsstruktur"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Vergütungsstruktur ====================== -->
{{< timelineItem icon="paypal" header="Vergütungsstruktur" subheader="Verfügbarkeit & Leistung" >}}
<ul>
  <li><strong>Pay-for-availability-Logik:</strong> Kapazitätsanbieter erhalten eine fixe Vergütung für die zugesicherte Verfügbarkeit – unabhängig von tatsächlicher Stromlieferung. Typisch für strategische Reserven (z. B. Schweden, Finnland), bei denen Einheiten vom Markt getrennt und nur in Ausnahmesituationen eingesetzt werden.</li>

  <li><strong>Pay-for-performance-Komponente:</strong> In marktweiten Mechanismen (z. B. Irland, Italien) wird die Verfügbarkeitsvergütung mit einer Leistungspflicht kombiniert: Anbieter erhalten Grundvergütung, müssen aber bei Knappheit Energie liefern, andernfalls drohen finanzielle Sanktionen.</li>

  <li><strong>Contracts for Difference (CfD):</strong> Rückzahlungsregelungen, bei denen Anbieter die Differenz zwischen festgelegtem Strike Price und tatsächlichem Marktpreis erstatten, wenn Letzterer überschritten wird (z. B. Belgien, Irland).</li>

  Diese Struktur hilft, Mitnahmeeffekte zu begrenzen und stellt sicher, dass Kapazitätsanbieter auch bei hohen Marktpreisen zur Systemstabilisierung beitragen.
</ul>
{{< /timelineItem >}}

<a id="kostenallokation"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Kostenallokation ====================== -->
{{< timelineItem icon="tag" header="Kostenallokation" subheader="Finanzierung & Verursacherprinzip" >}}

<ul>
  <li><strong>Finanzierung:</strong> Über drei Kanäle – Netzentgelte, allgemeine Steuern oder direkte Umlagen auf Stromkunden; die konkrete Ausgestaltung variiert je nach nationalem Kontext.</li>
  <li><strong>Beispiele:</strong>  
    <ul>
      <li>Deutschland: Kosten der strategischen Reserve werden über Netzentgelte weitergegeben (z. B. Kapazitätsreserve).</li>
      <li>Belgien: Finanzierung erfolgt über öffentliche Dienstverpflichtungen im Rahmen der Tarife des Übertragungsnetzbetreibers Elia.</li>
    </ul>
  </li>
  <li><strong>Herausforderung:</strong> Gewährleistung von Transparenz über Verteilung und Höhe der Kosten – insbesondere für Endkunden – und gleichzeitige Vermeidung von Marktverzerrungen.</li>
  <li><strong>Direkte Umlagen vs. Steuern:</strong>  
    <ul>
      <li>Direkte Umlagen auf Stromkunden können zu regressiven Verteilungseffekten führen.</li>
      <li>Steuerfinanzierte Ansätze können die Verbindung zwischen Verursachern und Kostenträgern abschwächen.</li>
    </ul>
  </li>
  <li><strong>Verursacherprinzip:</strong> Marktweite Mechanismen weisen eine Allokation nach Verursacherprinzip auf – Lastversorgungsunternehmen tragen Kosten proportional zu ihrem Beitrag während Stressperioden (z. B. Irland, UK), was als marktverträglich gilt und Anreize zur Lastreduktion setzt.</li>
</ul>
{{< /timelineItem >}}

<a id="governance"
   style="display:block; position:relative; top:-3rem; visibility:hidden;">
</a>
<!-- ====================== Governance & Institutionelle Zuständigkeiten ====================== -->
{{< timelineItem icon="shield" header="Governance & Institutionelle Zuständigkeiten" subheader="ÜNB, Regulierungsbehörden & dezentrale Modelle" >}}

<ul>
  <li><strong>Zentrale Rolle der ÜNB:</strong> Übertragungsnetzbetreiber agieren insb. bei zentralen organisierten KMs als Beschaffungsstellen, koordinieren Ausschreibungen (z. B. Belgien, Polen) und überwachen die Vertragserfüllung der Kapazitätsanbieter.</li>
  <li><strong>Aufgabe der Regulierungsbehörden:</strong> Genehmigung von Auktionsparametern, Festlegung von Preisobergrenzen und Bewertungsverfahren (z. B. Irland) – für Transparenz, Nichtdiskriminierung und Kostenkontrolle.</li>
  <li><strong>Dezentrale Modelle:</strong> Verantwortung liegt bei Marktakteuren (Stromlieferanten, Großverbraucher, Verteilnetzbetreiber), die Kapazitätszertifikate nach ihrem Spitzenlastanteil erwerben müssen (z. B. Frankreich). Dezentrale Strukturen ermöglichen regionale Nachfrageabbildung, sind aber administrativ aufwendiger und verursachen höhere Transaktionskosten.</li>
  <li><strong>Einfluss auf Effizienz & Integration:</strong> Die institutionelle Zuständigkeit bestimmt maßgeblich Effizienz, Steuerbarkeit und Integration des Kapazitätsmechanismus in bestehende Marktstrukturen.</li>
</ul>

{{< /timelineItem >}}
{{< /timeline >}}

{{< backtotop >}}
