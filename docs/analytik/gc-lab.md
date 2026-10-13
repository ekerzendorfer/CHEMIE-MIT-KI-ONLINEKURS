# GC-LAB – Gaschromatographie verstehen und Methoden entwickeln

Das **GC-LAB** ist ein browserbasiertes virtuelles Gaschromatographie-Labor für den Chemieunterricht. Es verbindet die Beobachtung eines chromatographischen Trennprozesses mit der Entwicklung geeigneter Messbedingungen, der Beurteilung der Trennqualität und der Identifikation unbekannter Komponenten über Referenzstandards.

[**GC-LAB öffnen**](https://ekerzendorfer.github.io/GC_LAB/){ .md-button .md-button--primary }

[**GC-01 direkt starten**](https://ekerzendorfer.github.io/GC_LAB/?task=GC01){ .md-button }

[**GC-02 direkt starten**](https://ekerzendorfer.github.io/GC_LAB/?task=GC02){ .md-button }

[**Quellcode auf GitHub**](https://github.com/ekerzendorfer/GC_LAB){ .md-button }

<!-- ABBILDUNG GC-01
     DATEI: ../assets/images/analytik/gc-lab/gc01_ueberblick.webp
     MOTIV: Gesamtansicht des GC-LABs mit Methodenauswahl, Chromatogramm und Messwerten.
     PRIORITÄT: A
     EMPFOHLENE BREITE: 1200–1400 px -->

## Warum ein virtuelles GC-Labor?

Die Gaschromatographie verbindet mehrere Ebenen, die im Unterricht leicht getrennt voneinander betrachtet werden:

- Stoffe werden in einer Säule unterschiedlich stark zurückgehalten,
- aus dieser Trennung entstehen zeitlich versetzte Detektorsignale,
- die Wahl der Methode beeinflusst Retentionszeiten und Auflösung,
- ein gut aussehendes Chromatogramm muss fachlich bewertet werden,
- und die Identifikation eines Peaks erfordert zusätzliche Evidenz.

Im GC-LAB können diese Zusammenhänge gezielt untersucht werden. Die Lernenden verändern chromatographische Bedingungen, vergleichen mehrere Läufe und beurteilen selbst, ob eine Trennung analytisch brauchbar ist.

!!! info "Didaktischer Schwerpunkt"
    Im Mittelpunkt steht nicht das Finden einer einzigen „richtigen“ Einstellung. Entscheidend ist die **Methodenentwicklung**: Wie verändern Temperatur, stationäre Phase, Säulenlänge und Gasstrom die Trennung – und welcher Kompromiss aus Auflösung und Laufzeit ist für die jeweilige Fragestellung sinnvoll?

## Vom Trennprozess zum Chromatogramm

Ein GC-Lauf entsteht nicht sofort als fertiges Diagramm. Im Beobachtungsmodus wächst das Chromatogramm entlang der chromatographischen Modellzeit.

Zusätzlich kann ein **schematisches Prinzipmodell** eingeblendet werden. Es zeigt den Weg

**Injektor → Säule → Wechselwirkung mit der stationären Phase → Detektor → elektrisches Signal → A/D → Chromatogramm**

und macht sichtbar, dass die Komponenten die Säule mit unterschiedlichen Retentionszeiten verlassen.

Die Darstellung ist bewusst ein didaktisches Modell. Sie zeigt keine maßstäbliche Molekülbewegung und legt sich nicht auf einen einzigen physikalischen Retentionsmechanismus fest.

<!-- GIF GC-02
     DATEI: ../assets/images/analytik/gc-lab/gc02_trennprozess.gif
     MOTIV: GC-Lauf mit gleichzeitig sichtbarer Prozessanimation und wachsendem Chromatogramm.
     PRIORITÄT: A
     EMPFOHLENE LÄNGE: 10–15 s
     EMPFOHLENE BREITE: 1200–1400 px -->

## Was lässt sich verändern?

Für die Methodenentwicklung stehen vier zentrale Parameter zur Verfügung:

| Parameter | Typische Auswirkung im Modell |
|---|---|
| **Stationäre Phase** | verändert die Selektivität und kann damit auch die Elutionsreihenfolge beeinflussen |
| **Säulenlänge** | längere Säule erhöht meist die Trennleistung, verlängert aber die Laufzeit |
| **Ofentemperatur** | höhere Temperatur verkürzt die Retention, kann jedoch die Trennung verschlechtern |
| **Trägergasstrom** | beeinflusst Totzeit und Effizienz; ein sehr hoher Strom ist nicht automatisch günstiger |

Für jeden Lauf werden Retentionszeiten, Peakflächen, Peakbreiten, Laufzeit und – bei mindestens zwei Peaks – die chromatographische Auflösung \(R_s\) angegeben.

Als Zielwert für eine analytisch brauchbare Trennung verwendet das Lernmodell

\[
R_s \ge 1{,}5
\]

Die Versuchshistorie erlaubt es, mehrere Methoden direkt miteinander zu vergleichen.

## Zwei Lernaufgaben für den Einstieg

Seit Version 0.5 enthält das GC-LAB zwei integrierte Aufgaben. Sie bilden einen kurzen Lernweg vom geführten Parametervergleich bis zur Untersuchung einer unbekannten Probe.

### GC-01 · Wie entsteht eine gute Trennung?

Diese Aufgabe ist als **geführter Einstieg** gedacht.

Untersucht wird ein Gemisch aus Ethylacetat und 1-Butanol. Der erste Lauf startet bewusst mit einer ungünstigen Methode:

- unpolare Säule,
- 15 m Säulenlänge,
- 140 °C,
- hoher Gasstrom.

Die Peaks sind dabei nur unzureichend getrennt.

Danach werden die Methodenparameter schrittweise freigegeben:

1. zunächst nur die Temperatur,
2. anschließend der Gasstrom,
3. danach die Säulenlänge.

Die Lernenden vergleichen jeweils Auflösung und Laufzeit. Am Ende werden die Läufe in der Versuchshistorie gegenübergestellt und eine kurze **Methodenbilanz** formuliert.

[**GC-01 starten – Wie entsteht eine gute Trennung?**](https://ekerzendorfer.github.io/GC_LAB/?task=GC01){ .md-button .md-button--primary }

<!-- GIF GC-03
     DATEI: ../assets/images/analytik/gc-lab/gc03_gc01_gefuehrt.gif
     MOTIV: GC-01 – Startlauf, Schrittwechsel und Freigabe eines neuen Parameters; idealerweise anschließend sichtbar verbesserte Trennung.
     PRIORITÄT: A
     EMPFOHLENE LÄNGE: 12–18 s -->

### GC-02 · Eine unbekannte Mischprobe untersuchen

GC-02 ist deutlich offener.

Die Probe **GC-U02** enthält drei unbekannte flüchtige Komponenten. Die Lernenden müssen zunächst selbst eine Methode entwickeln, mit der

\[
R_s \ge 1{,}5
\]

erreicht wird.

Sobald die Trennung ausreichend ist, wird die erfolgreiche Methode für die Identifikation fixiert.

Anschließend stehen fünf mögliche Referenzstandards zur Verfügung. Drei davon gehören tatsächlich zur Probe, zwei sind bewusst als **Negativkandidaten** enthalten.

Die Aufgabe ist erst abgeschlossen, wenn

- alle drei Probenpeaks korrekt zugeordnet wurden,
- und auch die beiden nicht passenden Standards als **„kein passender Peak“** erkannt wurden.

Damit wird ein wichtiger analytischer Gedanke sichtbar: Auch ein negativer Referenzbefund ist Information.

[**GC-02 starten – unbekannte Mischprobe**](https://ekerzendorfer.github.io/GC_LAB/?task=GC02){ .md-button .md-button--primary }

<!-- ABBILDUNG GC-04
     DATEI: ../assets/images/analytik/gc-lab/gc04_gc02_referenzstandards.webp
     MOTIV: GC-02 nach ausreichender Trennung: unbekanntes Chromatogramm, Referenzstandard-Bereich und Peakzuordnung sichtbar.
     PRIORITÄT: A
     EMPFOHLENE BREITE: 1200–1400 px -->

## Unbekannte Proben und Referenzstandards

Neben den beiden Aufgaben stehen mehrere unbekannte Dreikomponentenproben **GC-U01 bis GC-U05** zur freien Bearbeitung bereit.

Sie unterscheiden sich im Anspruch der Methodenentwicklung. Nach einer ausreichend guten Trennung können Referenzstandards unter exakt denselben chromatographischen Bedingungen gemessen werden.

Die Identifikation erfolgt nicht automatisch:

1. Referenzstandard auswählen,
2. Referenzlauf durchführen,
3. Retentionszeit vergleichen,
4. passenden Probenpeak auswählen oder **„kein passender Peak“** angeben,
5. Zuordnung prüfen.

Erst nach korrekter Zuordnung erscheint der Stoffname beim entsprechenden Peak.

!!! warning "Retentionszeit ist kein universeller Stoff-Fingerabdruck"
    Eine Retentionszeit besitzt nur unter definierten chromatographischen Bedingungen Aussagekraft. Deshalb werden Probe und Referenz im GC-LAB immer unter **derselben Methode** verglichen.

## Rolle im Digitalen Analytiklabor

Das GC-LAB ist zugleich ein wichtiges Detail-Labor des **Digitalen Analytiklabors**.

Dort werden nach einer Destillation zunächst unbekannte Fraktionen an den Gaschromatographen übergeben. Der Hub übermittelt die jeweilige Fraktion, die Stoffidentitäten bleiben im GC-LAB jedoch verborgen.

Ein GC-Lauf liefert zunächst nur chromatographische Evidenz:

- Zahl der Peaks,
- Retentionszeiten,
- Peakflächen,
- Peakbreiten,
- minimale Auflösung.

Die Peaks bleiben als **P1, P2, ...** unidentifiziert.

Erst eine anschließende Strukturaufklärung kann eine Stoffhypothese liefern. Danach kann das GC-LAB erneut aufgerufen werden, diesmal zur gezielten Bestätigung mit **Referenzstandard und Aufstockung**.

Damit übernimmt die Gaschromatographie im Gesamtworkflow zwei unterschiedliche Rollen:

**Trennung unbekannter Komponenten → spätere chromatographische Bestätigung einer bereits begründeten Identität.**

<!-- ABBILDUNG GC-05
     DATEI: ../assets/images/analytik/gc-lab/gc05_hub_bestaetigung.webp
     MOTIV: gezielte Identitätsbestätigung aus dem Analytik-Hub mit Referenzstandard und Aufstockung.
     PRIORITÄT: B
     EMPFOHLENE BREITE: 1200–1400 px -->

[**Zum Digitalen Analytiklabor im Begleitkurs**](digitales-analytiklabor.md){ .md-button }

## Modellgrenzen

Das GC-LAB ist ein **didaktisches Methodenmodell** und kein universeller Retentionszeit-Rechner.

Derzeit bewusst nicht enthalten sind unter anderem:

- Temperaturprogramme,
- quantitative GC-Kalibration,
- komplexe Basislinien- und Detektoreffekte,
- reale Peak-Asymmetrien in ihrer gesamten Vielfalt.

Die kuratierten Stoff- und Retentionsparameter dienen dazu, zentrale Prinzipien der Gaschromatographie systematisch und reproduzierbar untersuchen zu können.

## Empfohlener Lernweg

Für den Einstieg bietet sich folgende Reihenfolge an:

1. **GC-01** – Einfluss einzelner Methodenparameter verstehen,
2. freies Experimentieren mit bekannten Mischungen,
3. **GC-02** – unbekannte Probe trennen und mit Referenzstandards identifizieren,
4. weitere unbekannte Proben GC-U01 bis GC-U05,
5. Einsatz des GC-LABs als Teil einer größeren analytischen Beweiskette im **Digitalen Analytiklabor**.

So entwickelt sich der Gaschromatograph vom geführten Lernwerkzeug schrittweise zu einem offenen analytischen Instrument.
