# KINETIK-LAB – Anleitung für LehrerInnen

## Vom beobachteten Phänomen zum Geschwindigkeitsgesetz

Das **KINETIK-LAB** ist eine browserbasierte Lernumgebung zur photometrischen Untersuchung der Reaktion von Kristallviolett mit Hydroxidionen. Es verbindet eine überraschende Beobachtung, präexperimentelle Planung, virtuelle Erprobung, einen realen Versuch bzw. reale Referenzdaten und eine schrittweise kinetische Auswertung.

[**KINETIK-LAB öffnen**](https://ekerzendorfer.github.io/KINETIK_LAB/){ .md-button .md-button--primary }

!!! info "Grundidee"
    Die Anwendung soll den Erkenntnisweg strukturieren, aber nicht vorwegnehmen. Die SchülerInnen sollen möglichst viele fachliche Entscheidungen selbst treffen und diese begründen. Die Lehrkraft moderiert, gibt bei Bedarf Hilfen und entscheidet, wann die nächste Phase freigegeben wird.

---

# 1. Lernziele und didaktische Funktion

Das KINETIK-LAB verbindet mehrere Kompetenzbereiche:

- Beobachtungen von Deutungen unterscheiden,
- aus einem Phänomen eine untersuchbare Forschungsfrage entwickeln,
- eine geeignete Messgröße auswählen,
- Messintervall und Messdauer begründet festlegen,
- eine geeignete Messwellenlänge auswählen,
- reale und virtuelle Messdaten vergleichen,
- Messkurven mathematisch transformieren,
- aus linearen Darstellungen auf Reaktionsordnungen schließen,
- aus mehreren Teilbefunden ein Geschwindigkeitsgesetz formulieren,
- Messunsicherheiten und Modellgrenzen reflektieren.

Im Mittelpunkt steht nicht die Frage, ob eine virtuelle Kurve möglichst exakt eine reale Messung kopiert. Entscheidend ist vielmehr:

**Welche Aussage lässt sich aus einer Messreihe tatsächlich ableiten – und wie sicher ist diese Aussage?**

---

# 2. Fachliches Vorwissen

Das KINETIK-LAB ist nicht als Einführung in die gesamte Reaktionskinetik gedacht.

Vor Beginn sollten die SchülerInnen bereits Grundkenntnisse besitzen zu:

- Reaktionsgeschwindigkeit,
- Reaktionsordnung,
- integrierten Geschwindigkeitsgesetzen,
- Bedeutung einer linearen Darstellung,
- einfacher Regression und R²,
- Absorbanz bzw. Extinktion,
- grundlegendem Zusammenhang zwischen Konzentration und Absorbanz.

Hilfreich ist außerdem, wenn die SchülerInnen bereits einfache photometrische Messungen kennen.

!!! note
    Der Begriff **pseudo-erste Ordnung** kann im Unterricht entweder vorher eingeführt oder im Zuge der Auswertung des Experiments konkretisiert werden.

---

# 3. Zeitbedarf

Je nach Unterrichtsorganisation sind unterschiedliche Varianten möglich.

### Kompakte Variante

- Phase 1 und 2: ca. 20–30 min
- Phase 3: ca. 20–30 min
- Phase 4: reale Daten bereitstellen
- Phase 5: ca. 30–45 min

### Vollständige Variante mit Realexperiment

Sinnvoll ist eine Aufteilung auf mehrere Unterrichtsphasen:

1. Beobachtung und Messplanung
2. virtuelle Erprobung
3. realer Versuch
4. Auswertung und Modellbildung

Das KINETIK-LAB kann damit sowohl als zusammenhängende Unterrichtssequenz als auch als Verbindung zwischen mehreren Unterrichtsstunden eingesetzt werden.

---

# 4. Phase 1 – Beobachten

## Didaktische Funktion

Die SchülerInnen sollen zunächst nur beobachten und Hypothesen bilden. Die Reaktionsgleichung, die Reaktionsordnung und die optimale Wellenlänge werden noch nicht vorgegeben.

Ausgangspunkt sind zwei gleich aussehende Bechergläser mit Kristallviolett-Lösung. In einem Gefäß tritt eine deutlich sichtbare Entfärbung auf.

Die Animation dauert bewusst nur etwa **20 s**. Sie stellt keinen realen vollständigen Reaktionsverlauf dar, sondern dient als didaktisch geraffte Beobachtung.

## Erwartbare Schülerideen

Mögliche Hypothesen sind zum Beispiel:

- Verdünnung,
- Temperaturunterschied,
- Licht- oder Alterungseffekt,
- chemische Reaktion mit einem Rückstand,
- nicht ausreichend gereinigtes Becherglas.

## Rolle der Lehrkraft

Die Lehrkraft sollte zunächst nicht sofort auf Natronlauge hinweisen.

Sinnvoll ist eine kurze gemeinsame Sammlung:

- Was wurde tatsächlich beobachtet?
- Was ist bereits Interpretation?
- Welche Hypothesen sind prinzipiell überprüfbar?

Nach der Besprechung kann die Zusatzinformation freigegeben werden, dass sich im betroffenen Becherglas Rückstände von Natronlauge befanden.

!!! tip
    Die Phase eignet sich gut für eine gemeinsame Projektion. Trotzdem sollten die SchülerInnen ihre eigene Beobachtung und mindestens eine eigene Hypothese dokumentieren.

---

# 5. Phase 2 – Planen

## Didaktische Funktion

Nun soll aus der Beobachtung eine quantitative Forschungsfrage entstehen.

Eine zentrale Frage kann etwa lauten:

**Wie lässt sich das Verschwinden der Farbe quantitativ erfassen und welche Gesetzmäßigkeiten können aus dem zeitlichen Verlauf abgeleitet werden?**

Die App erwartet keine exakt vorgegebene Formulierung.

## Aufgaben der SchülerInnen

Die SchülerInnen sollen:

- eine Forschungsfrage formulieren,
- eine mögliche Messgröße vorschlagen,
- einen erwarteten Kurvenverlauf skizzieren,
- Messintervall und Messdauer abschätzen,
- mögliche Fehler- und Störquellen benennen.

## Rolle der Lehrkraft

Hilfreich ist es, nicht sofort das Photometer als Lösung zu nennen.

Mögliche Impulse:

- Wie könnte man „Farbintensität“ objektiver als mit dem Auge messen?
- Welche Größe müsste sich während der Reaktion ändern?
- Muss wirklich bis zur vollständigen Entfärbung gemessen werden?
- Was ist wichtiger: sehr viele Messpunkte oder ein ausreichend langer Zeitraum?

Die kleine Entfärbungssimulation dient nur dazu, eine Vorstellung vom Zeitmaßstab zu entwickeln.

!!! note
    In dieser Phase wird bewusst noch mit dem Begriff **Farbintensität** gearbeitet. Die genaue photometrische Messgröße wird erst anschließend konkretisiert.

---

# 6. Phase 3 – Virtuell erproben

## 6.1 Phase 3A – Wellenlänge

### Ziel

Die SchülerInnen sollen zuerst aus dem virtuellen Spektrum eine theoretisch günstige Messwellenlänge ableiten und erst danach prüfen, welche Wellenlängen mit einem real verfügbaren Gerät möglich sind.

Beim Start ist daher **kein Messgerät vorausgewählt**.

### Sinnvoller Ablauf

1. Spektralscan ohne Gerätewahl durchführen.
2. Absorptionsmaximum bestimmen.
3. Messgerät auswählen.
4. verfügbare reale Wellenlängen prüfen.
5. geeignete reale Messwellenlänge auswählen und begründen.

Beim verwendeten Vernier-Colorimeter stehen feste Wellenlängen zur Verfügung. Für den realen Referenzversuch wurde **565 nm** verwendet.

Wichtig: Diese Wellenlänge soll nicht von der App automatisch als „richtige Lösung“ vorgegeben werden.

### Rolle der Lehrkraft

Die entscheidende Frage lautet:

**Was ist theoretisch günstig – und was ist experimentell tatsächlich verfügbar?**

Damit entsteht eine realistische Geräteentscheidung statt einer bloßen Abfrage des Absorptionsmaximums.

---

## 6.2 Phase 3B – Messstrategie

### Ziel

Die SchülerInnen testen ihren Messplan, bevor reale Messzeit und Material eingesetzt werden.

Sie variieren:

- Messintervall,
- Messdauer.

Dabei erhalten sie Rückmeldungen zu:

- Anzahl der Messpunkte,
- erfasstem Signalbereich,
- möglicherweise zu kurzem Messzeitraum,
- möglicherweise zu grober zeitlicher Auflösung.

### Didaktischer Kern

Ein kurzer Ausschnitt einer gekrümmten Kurve kann fast geradlinig erscheinen.

Die SchülerInnen sollen daher erkennen:

- viele Messpunkte sind nicht automatisch besser,
- ein zu kurzer Messzeitraum kann zu Fehlinterpretationen führen,
- ein zu grobes Intervall kann relevante Änderungen verdecken.

Die zusätzliche Messdauer von **1000 s** erlaubt bewusst auch einen langen virtuellen Testlauf.

## Rolle der Lehrkraft

Die App bewertet den Messplan nicht einfach als „richtig“ oder „falsch“.

Sinnvolle Rückfragen sind:

- Reicht der erfasste Kurvenabschnitt für eine Aussage?
- Ist das gewählte Messintervall wirklich notwendig?
- Was gewinnt man durch eine längere Messdauer?
- Wie viele Messpunkte sind fachlich sinnvoll?

---

# 7. Phase 4 – Real messen

## Mögliche Datenquellen

Die App unterstützt drei Unterrichtssituationen:

1. **eigener Realversuch**
2. **realer Referenzdatensatz**
3. **synthetischer Entwicklungs-/Testdatensatz**

Für regulären Unterricht ist der reale Versuch oder der reale Referenzdatensatz vorzuziehen.

---

## 7.1 Realexperiment

### Referenzansatz

Der derzeit real kalibrierte Referenzfall verwendet:

- c₀(KV⁺) = 1,20 × 10⁻⁵ mol/L
- c₀(OH⁻) = 0,0300 mol/L
- Vernier Colorimeter
- 565 nm
- Messintervall: 5 s
- Temperatur beim Referenzlauf: ca. 22 °C

### Praktische Durchführung

Bewährt hat sich:

1. eine Lösung im kleinen Becherglas vorlegen,
2. zweite Lösung zupipettieren,
3. mit einer Kolbenhubpipette einmal aufziehen und wieder ausstoßen,
4. Probe rasch in die Küvette überführen,
5. Küvette in das Messgerät einsetzen.

Bei einer Einzelperson entstehen dabei etwa **15 s Startverzögerung** zwischen dem ersten Kontakt der Lösungen und dem ersten registrierten Messwert.

!!! important
    Diese Verzögerung wird dokumentiert, aber **nicht in das virtuelle Reaktionsmodell eingebaut**. Sie ist Teil des realen experimentellen Ablaufs.

### Experimenteller Knackpunkt

Der kritischste praktische Schritt ist eine möglichst schnelle und reproduzierbare Durchmischung.

Typische Fehlerquellen:

- unterschiedliche Mischdauer,
- Luftblasen,
- verzögerte Überführung,
- ungenaue Pipettierung,
- verschmutzte oder unterschiedlich ausgerichtete Küvetten,
- Temperaturunterschiede.

---

## 7.2 CSV-Import

Viele Messgeräte exportieren mehrere Messgrößen gleichzeitig.

Beim Vernier-Export können beispielsweise enthalten sein:

- Zeit,
- Transmission,
- Absorbanz.

Die App lässt daher nach dem Einlesen die Zeit- und Messwertspalte sichtbar auswählen.

Für die weitere kinetische Auswertung soll **Absorbanz/Extinktion** verwendet werden.

!!! tip
    Vor der eigentlichen Auswertung sollte gemeinsam kontrolliert werden, ob die richtige Messwertspalte importiert wurde.

---

# 8. Phase 5 – Auswerten

# 8.1 Phase 5A – Rohdaten

## Ziel

Vor jeder mathematischen Transformation sollen die SchülerInnen zunächst die reale Messkurve beurteilen.

Leitfragen:

- Ist die Kurve grundsätzlich plausibel?
- Gibt es Ausreißer?
- Ist der Anfangsbereich ausreichend erfasst?
- Ist ein Endplateau erkennbar?
- Reicht die Messdauer aus?

---

## A∞

Für die Transformationen wird ein Wert A∞ benötigt.

Der reale Langzeit-Referenzversuch ergab:

**A∞ ≈ 0,01136**

Dieser Wert wurde aus einer etwa 20-minütigen realen Messung bestimmt.

Die App bietet drei Möglichkeiten:

- realen Referenzwert verwenden,
- A∞ aus einem tatsächlich erreichten Endplateau schätzen,
- begründete manuelle Eingabe.

!!! warning
    Die letzten Messpunkte einer kurzen Messung dürfen nicht automatisch als A∞ interpretiert werden. Bei einer 500- oder 600-s-Messung ist die Reaktion noch nicht vollständig beendet.

---

# 8.2 Phase 5B – Realität und Modell

Die reale und die virtuelle Kurve werden miteinander verglichen.

Neben den Rohdaten kann eine normierte Darstellung verwendet werden.

Die Normierung hilft dabei, Unterschiede in der absoluten Signalhöhe von Unterschieden im zeitlichen Verlauf zu trennen.

## Didaktische Botschaft

Das virtuelle Modell wurde an einer realen Schulmessung kalibriert.

Es ist trotzdem **kein digitaler Klon** des Realexperiments.

Abweichungen dürfen und sollen sichtbar bleiben.

Mögliche Ursachen:

- reales Messrauschen,
- Mischvorgang,
- Temperatur,
- Geräteauflösung,
- vereinfachtes Modell,
- Konzentrationsabweichungen.

---

# 8.3 Phase 5C – Reaktionsordnung bezüglich Kristallviolett

Die App zeigt nacheinander:

- A − A∞ gegen t
- ln(A − A∞) gegen t
- 1/(A − A∞) gegen t

Die SchülerInnen sollen selbst beurteilen, welche Darstellung über einen großen Bereich am besten linear verläuft.

## Vorläufige Vermutung

Nach dem Vergleich wird eine Reaktionsordnung ausgewählt:

- 0. Ordnung
- 1. Ordnung
- 2. Ordnung

Die App gibt anschließend eine kurze erklärende Rückmeldung.

Dabei gilt:

- A − A∞ linear gegen t → Hinweis auf 0. Ordnung
- ln(A − A∞) linear gegen t → Hinweis auf 1. Ordnung
- 1/(A − A∞) linear gegen t → Hinweis auf 2. Ordnung

Die Rückmeldung soll nicht als Prüfung, sondern als **Scaffolding** verstanden werden.

---

## Fitbereich nahe A∞

Nahe am Endwert wird A − A∞ sehr klein.

Dadurch verstärken:

- Logarithmus,
- besonders der Kehrwert

kleine Messfehler stark.

Die App verwendet deshalb für die Regression nur einen geeigneten Fitbereich. Späte Messpunkte bleiben in den Rohdaten sichtbar, werden aber nicht mehr für die lineare Regression verwendet.

Beim realen Referenzlauf führt der sinnvolle Fitbereich ungefähr bis 575 s.

Für ln(A − A∞) ergibt sich damit ein nahezu linearer Verlauf und ein k_app in der Größenordnung von:

**k_app ≈ 0,0053 s⁻¹**

---

# 8.4 Phase 5D – Einfluss der Hydroxidkonzentration

## Ziel

Nun wird untersucht, wie sich k_app mit der Hydroxidkonzentration verändert.

Die App macht den Erkenntnisweg bewusst sichtbar:

**[OH⁻] verändern → k_app bestimmen → k_app gegen [OH⁻] auftragen → Reaktionsordnung ableiten**

Für jede Hydroxidkonzentration wird ein eigener virtueller Lauf durchgeführt.

Die SchülerInnen übertragen die wenigen k_app-Werte bewusst manuell in die Tabelle.

## Aktueller Validierungsstand

Der Punkt bei:

**[OH⁻] = 0,0300 mol/L**

ist durch den realen Referenzversuch kalibriert.

Die weiteren Werte bei:

- 0,005 mol/L
- 0,010 mol/L
- 0,020 mol/L

sind derzeit **Modellvorhersagen**.

Sie beruhen auf der Annahme einer linearen Beziehung zwischen k_app und [OH⁻].

Diese Reihe soll später ebenfalls durch Realmessungen überprüft werden.

!!! important
    Im Unterricht sollte klar zwischen **real gemessen**, **aus Messdaten gefittet** und **aus dem Modell vorhergesagt** unterschieden werden.

---

# 8.5 Phase 5E – Einfluss der Wellenlänge

Die SchülerInnen vergleichen:

- eine theoretisch günstige Wellenlänge nahe dem Absorptionsmaximum,
- die tatsächlich verwendete reale Messwellenlänge.

Beim Referenzversuch wurde mit dem Vernier-Colorimeter bei **565 nm** gearbeitet.

Erwartet wird:

- Änderung der absoluten Signalhöhe,
- weitgehend gleicher grundlegender kinetischer Verlauf.

Das KINETIK-LAB erlaubt diesen Vergleich im Modell.

Eine zusätzliche freie Wellenlängenvariation im Kinetikmodul des SpektralLab ist derzeit nicht vorgesehen.

---

# 9. Finale Erkenntnis

Am Ende sollen die SchülerInnen selbst formulieren:

- Reaktionsordnung bezüglich CV⁺,
- Reaktionsordnung bezüglich OH⁻,
- daraus abgeleitetes Geschwindigkeitsgesetz,
- verwendete Evidenz,
- verbleibende Unsicherheiten.

Kleine **Denkhilfe-Schaltflächen** unterstützen bei Bedarf.

Sie erinnern an:

- passende Linearisierung,
- Zusammenhang zwischen k_app und [OH⁻],
- Zusammensetzen der Teilordnungen.

Die vollständige Lösung wird nicht automatisch eingesetzt.

---

# 10. Erwartete fachliche Schlussfolgerung

Für den verwendeten Modellansatz ergibt sich:

- erste Ordnung bezüglich Kristallviolett,
- erste Ordnung bezüglich Hydroxidionen,

und damit:

**v = k · [CV⁺] · [OH⁻]**

Da Hydroxidionen im Experiment in großem Überschuss vorliegen, kann für einen einzelnen Lauf näherungsweise mit einer pseudo-ersten Ordnung bezüglich Kristallviolett gearbeitet werden.

Dabei gilt:

**k_app = k · [OH⁻]**

---

# 11. Real kalibrierter Referenzfall

Der derzeit wichtigste reale Bezugspunkt der Simulation ist:

| Größe | Referenzwert |
|---|---:|
| c₀(CV⁺) | 1,20 × 10⁻⁵ mol/L |
| c₀(OH⁻) | 0,0300 mol/L |
| Messgerät | Vernier Colorimeter |
| Wellenlänge | 565 nm |
| Temperatur | ca. 22 °C |
| A∞ | ca. 0,01136 |
| k_app | ca. 0,00534 s⁻¹ |
| Halbwertszeit | ca. 130 s |
| reale Startverzögerung | ca. 15 s |

Die Startverzögerung wird **nicht** in das virtuelle Modell übernommen.

---

# 12. Modellgrenzen und derzeit offene Punkte

Die virtuelle Kinetik ist real kalibriert, aber bewusst nicht an jeden einzelnen Messwert angepasst.

Noch offen bzw. in weiterer Prüfung:

- Wiederholungsmessungen der niedrigen und hohen Kristallviolett-Konzentration,
- Langzeitmessungen auch für diese Konzentrationen,
- reale Überprüfung der gesamten OH⁻-Reihe,
- möglicher zusätzlicher Vergleich mit einem Spektralphotometer nahe λmax,
- spätere Anpassung des gemeinsamen Kinetik-Kerns im SpektralLab.

Die bisher gemessenen verschiedenen Kristallviolett-Konzentrationen zeigen kleine, aber systematische Unterschiede in den erhaltenen k_app-Werten.

Diese Abweichungen werden nicht in das virtuelle Modell „hineinkalibriert“, solange ihre Ursache nicht ausreichend geklärt ist.

---

# 13. Rolle der KI bei der Entwicklung

Die Messkurven der App sind nicht einfach von einer generativen KI erzeugte Werte.

Die Rollen sind getrennt:

### Reales Experiment

liefert den empirischen Referenzpunkt.

### Fachmodell

beschreibt den Zusammenhang mathematisch und chemisch.

### Generative KI

unterstützt bei:

- Entwicklung der Benutzeroberfläche,
- Programmierung,
- Gestaltung des Lernpfads,
- Formulierung von Hilfen,
- Variation von Aufgaben,
- iterativer Überarbeitung nach Praxistests.

Damit bleibt nachvollziehbar, welche Aussagen auf Messdaten beruhen und welche Teile modelliert sind.

!!! quote
    **Real kalibriert, aber nicht realitätskosmetisiert:**  
    Die Simulation wird an realen Experimenten geprüft. Abweichungen, Modellgrenzen und noch nicht validierte Bereiche bleiben sichtbar.

---

# 14. Ergebnisse zur Besprechung und Protokoll

An mehreren Stellen kann die Gruppe ihre Ergebnisse über **„Ergebnisse zur Besprechung anzeigen“** zusammenfassen.

Diese Funktion eignet sich besonders:

- nach Phase 2,
- nach Phase 3,
- nach Phase 4,
- nach der finalen Auswertung.

Die Anzeige kann in die Zwischenablage kopiert werden.

Zusätzlich kann ein vollständiger Arbeitsstand als Markdown-Datei exportiert werden.

Damit kann die Lehrkraft den Denkweg nachvollziehen, ohne dass die App selbst eine automatische fachliche Bewertung übernimmt.

---

# 15. Hinweise für den Unterrichtseinsatz

Ein sinnvoller Ablauf ist:

1. Phase 1 gemeinsam beginnen.
2. Hypothesen im Plenum diskutieren.
3. Phase 2 in Kleingruppen durchführen.
4. Messplan kurz mit der Lehrkraft besprechen.
5. Phase 3 möglichst selbstständig bearbeiten lassen.
6. realen Versuch durchführen oder Referenzdaten bereitstellen.
7. Phase 5 wieder in Gruppen durchführen.
8. finale Erkenntnisse gemeinsam vergleichen.

Die App eignet sich damit besonders für einen Wechsel aus:

**individueller Arbeit – Gruppenarbeit – gemeinsamer Besprechung**

---

# 16. Sicherheit

Kristallviolett ist als Laborchemikalie entsprechend den schulischen Sicherheitsvorgaben zu behandeln.

Für den Realversuch werden nur sehr geringe und stark verdünnte Mengen benötigt.

Trotzdem sind insbesondere zu beachten:

- Schutzbrille,
- geeignete Schutzhandschuhe entsprechend der schulischen Gefährdungsbeurteilung,
- sorgfältiges Arbeiten beim Herstellen der Lösungen,
- Vermeidung von Haut- und Kleidungskontakt,
- sachgerechte Entsorgung der Versuchslösungen.

Die endgültige Durchführung richtet sich nach den am jeweiligen Schulstandort geltenden Vorschriften und der Gefährdungsbeurteilung der Lehrkraft.

---

# 17. Videos zum Realexperiment

Für den Begleitkurs sind zwei kurze Videos vorgesehen:

### Qualitative Beobachtung der Entfärbung

Zeigt die sichtbare Farbänderung im Realversuch.

**Video-Link:** wird nach Bearbeitung ergänzt.

### Datenerfassung mit dem Vernier Colorimeter

Zeigt die praktische Mischung, Überführung in die Küvette und Messwerterfassung.

**Video-Link:** wird nach Bearbeitung ergänzt.

<!--
Rohfassungen:

Qualitative Beobachtung:
https://youtu.be/hc1YmpWaESE

Datenerfassung:
https://youtu.be/XL6rqaDQCKs
-->

---

## Kurzfassung der didaktischen Leitidee

**Beobachten → Planen → virtuell erproben → real messen → mathematisch auswerten → chemisch interpretieren**

Die virtuelle Lernumgebung soll dabei nicht den Versuch ersetzen, sondern den Weg zwischen Beobachtung, Messung und Erkenntnis sichtbar machen.
