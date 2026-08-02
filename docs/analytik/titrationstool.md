# Titrationskurven aufnehmen, auswerten und verstehen

Das **TITRATIONSTOOL** ist ein browserbasiertes virtuelles Labor für Säure-Base-Titrationen. Es verbindet die Durchführung einer simulierten Titration mit der fachlichen Auswertung der Messdaten: Titrationskurve, erste und zweite Ableitung, Äquivalenzpunkte, Indikatorwahl, Halbäquivalenzpunkt und quantitative Konzentrationsbestimmung stehen in einer gemeinsamen Arbeitsumgebung zur Verfügung.

[**TITRATIONSTOOL öffnen**](https://ekerzendorfer.github.io/TITRATIONSTOOL/){ .md-button .md-button--primary }

[**Quellcode auf GitHub**](https://github.com/ekerzendorfer/TITRATIONSTOOL){ .md-button }

<!-- GIF 01: titrationstool-ueberblick.gif
     Kurzer Überblick: Stoff auswählen, tropfenweise titrieren, Kurve und Apparatur reagieren.
     Empfohlene Länge: 8–12 s, 1200–1400 px Breite. -->

## Warum ein virtuelles Titrationslabor?

Eine reale Titration verbindet mehrere anspruchsvolle Ebenen:

- eine Apparatur muss korrekt aufgebaut und bedient werden,
- das Volumen der Maßlösung muss zuverlässig abgelesen werden,
- Farbänderungen oder Messwerte müssen beobachtet werden,
- die stöchiometrische Reaktion muss verstanden werden,
- die Messreihe muss grafisch ausgewertet werden,
- aus dem Äquivalenzvolumen wird schließlich eine Konzentration berechnet.

Im Unterricht bleibt häufig nur wenig Zeit, alle Ebenen gleich gründlich zu behandeln. Das virtuelle Labor ersetzt das reale Experiment nicht. Es erlaubt aber, einzelne Aspekte gezielt zu isolieren, Messreihen beliebig zu wiederholen und die mathematische Auswertung unmittelbar mit dem Verlauf der Titration zu verbinden.

!!! info "Didaktische Grundidee"
    Das TITRATIONSTOOL ist weder eine reine Animation noch ein automatischer Aufgabenlöser. Die Lernenden erzeugen eine Messreihe, wählen die Auswertungsmethode und tragen Ergebnisse selbst ein. Das Werkzeug übernimmt dort Rechenarbeit, wo sie den Blick auf das chemische Konzept verstellen würde, und fordert eigene Auswertung dort, wo sie fachlich entscheidend ist.

## Lernziele

Mit dem TITRATIONSTOOL können SchülerInnen unter anderem:

- Titrationskurven starker und schwacher Säuren beziehungsweise Basen unterscheiden,
- den Einfluss der Säure- oder Basenstärke auf Anfangs-pH und Äquivalenzbereich erklären,
- Äquivalenzpunkte aus einer Titrationskurve abschätzen,
- erste und zweite Ableitung fachgerecht interpretieren,
- geeignete Indikatoren anhand ihres Umschlagsbereichs auswählen,
- den Halbäquivalenzpunkt bestimmen und \(pH=pK_\mathrm{s}\) anwenden,
- Stoffmengenverhältnisse aus Reaktionsgleichungen ableiten,
- Konzentrationen in mol/L und g/L berechnen,
- bei zweiprotonigen Säuren zwei Neutralisationsstufen unterscheiden,
- Messdaten für eine weiterführende Auswertung exportieren.

## Zwei Arbeitsbereiche

Die App besitzt zwei grundsätzlich verschiedene Zugänge.

### Freies Labor

Im freien Labor können alle wesentlichen Versuchsparameter selbst gewählt werden:

- Titrationsart
- Analyt
- Probenkonzentration
- Probenvolumen
- Konzentration der Maßlösung
- Tropfengröße
- Indikator
- manuelle oder automatische Zugabe

Die Stoffdaten können aus den hinterlegten Beispielen übernommen oder für eigene starke beziehungsweise schwache Säuren und Basen eingegeben werden.

<!-- GIF 02: titrationstool-freies-labor.gif
     Stoff- und Parameterauswahl, Start der Messung, Wechsel zwischen Einzeltropfen und Auto-Titration. -->

### Begleitende Aufgaben

Der Aufgabenbereich bietet neun sofort einsetzbare Lernaufgaben. Jede Aufgabe enthält:

- ein ausgewiesenes Lernziel,
- eine konkrete Versuchsanweisung,
- passende Voreinstellungen,
- gesperrte Parameter, die nicht verändert werden sollen,
- Eingabefelder für die Ergebnisse,
- gestufte Hinweise,
- eine Prüffunktion,
- eine einblendbare LehrerInnenlösung.

Bei den quantitativen Aufgaben wird bei jedem neuen Laden eine andere Variante erzeugt. Die zugrunde liegende Probenkonzentration bleibt verborgen. Die Äquivalenzvolumina werden bewusst in einem moderaten Bereich gewählt, damit keine unnötig langen Titrationen entstehen.

<!-- GIF 03: titrationstool-aufgabenmodus.gif
     Aufgabe auswählen, Versuch laden, Ergebnisfeld ausfüllen, Hinweis und Rückmeldung zeigen. -->

## Die simulierte Apparatur

Die schematische Apparatur zeigt:

- eine Bürette mit Maßlösung,
- eine angedeutete Bürettenablesung,
- ein Becherglas mit Analytlösung,
- eine pH-Elektrode,
- einen Magnetrührer mit Rührstäbchen,
- den fallenden Tropfen bei der Zugabe.

Der aktuelle pH-Wert und das zugegebene Volumen werden zusätzlich in einer digitalen Anzeige dargestellt. Die Apparatur ist bewusst reduziert. Sie dient der Orientierung und der Verknüpfung von Volumenzugabe, pH-Änderung und Kurvenverlauf.

!!! warning "Kein Ersatz für die Laborunterweisung"
    Die Darstellung zeigt das Prinzip einer Titration. Sicherheitsregeln, korrektes Spülen und Füllen der Bürette, Entfernen von Luftblasen, Ablesen des Meniskus und sachgerechter Umgang mit der pH-Elektrode müssen im realen Labor gesondert erarbeitet werden.

## Unterstützte Titrationsarten

Das Werkzeug deckt vier schulisch zentrale Klassen ab:

| Analyt | Maßlösung | Verlauf der pH-Kurve |
|---|---|---|
| starke Säure | starke Base | steigend |
| schwache Säure, ein- oder zweiprotonig | starke Base | steigend |
| starke Base | starke Säure | fallend |
| schwache einprotonige Base | starke Säure | fallend |

Damit lassen sich typische Unterschiede systematisch untersuchen:

- Lage des Anfangs-pH-Werts
- Größe und Lage des pH-Sprungs
- pH-Wert am Äquivalenzpunkt
- Ausbildung eines Pufferbereichs bei schwachen Protolyten
- Lage des Halbäquivalenzpunkts
- Eignung verschiedener Indikatoren

## Stoffauswahl

Die hinterlegten Beispiele wurden so gewählt, dass nicht nur Standardfälle, sondern auch didaktisch interessante Vergleiche möglich sind.

### Säuren

- Salzsäure
- Salpetersäure
- Chloressigsäure
- Ameisensäure
- Essigsäure
- Propionsäure
- Milchsäure
- Benzoesäure
- Oxalsäure
- Pyridiniumchlorid beziehungsweise Pyridinium-Ion

### Basen

- Natronlauge
- Ammoniak
- Methylamin
- Pyridin

Chloressigsäure erweitert den Bereich zu stärkeren einprotonigen Carbonsäuren. Beim Pyridiniumchlorid wird deutlich, dass ein sauer reagierendes Teilchen nicht zwingend eine Carboxygruppe enthalten muss: Titriert wird das Pyridinium-Ion als konjugierte Säure des Pyridins.

## Titrationskurven aufnehmen

Nach dem Laden eines Versuchs beginnt die Messreihe bei \(V=0\). Jeder weitere Messpunkt besteht aus:

- dem kumulativ zugegebenen Volumen der Maßlösung,
- dem zugehörigen pH-Wert nach vollständiger Durchmischung.

Die Tropfengröße kann verändert werden. Große Schritte liefern schnell einen Überblick, können aber den steilen Kurvenbereich unzureichend auflösen. Kleine Schritte erhöhen die Messpunktdichte und verbessern insbesondere die Ableitungsauswertung.

!!! tip "Bewährter Arbeitsablauf"
    Zunächst kann mit größeren Schritten bis in die Nähe des erwarteten Äquivalenzbereichs titriert werden. Dort wird die Tropfengröße reduziert. Im Aufgabenmodus sind geeignete Schrittweiten bereits vorgegeben.

<!-- GIF 04: titrationstool-tropfen-und-kurve.gif
     Mehrere Tropfen; pH-Anzeige, Flüssigkeitsfarbe und Kurve verändern sich synchron. -->

## Der Äquivalenzpunkt

Am Äquivalenzpunkt wurden Analyt und Maßlösung im stöchiometrisch erforderlichen Stoffmengenverhältnis umgesetzt. Bei einer einprotonigen Säure und Natronlauge gilt beispielsweise:

\[
n(HA)=n(OH^-)
\]

Daraus folgt:

\[
c(HA)\cdot V(HA)=c(OH^-)\cdot V_\mathrm{ÄP}
\]

Der Äquivalenzpunkt ist nicht mit einem bestimmten pH-Wert gleichzusetzen:

- starke Säure + starke Base: im idealisierten Modell ungefähr pH 7,
- schwache Säure + starke Base: Äquivalenzpunkt im basischen Bereich,
- schwache Base + starke Säure: Äquivalenzpunkt im sauren Bereich.

Diese Unterschiede gehören zu den wichtigsten Lernzielen der App.

## Erste Ableitung

Die erste Ableitung beschreibt die pH-Änderung pro Volumenänderung. Für zwei aufeinanderfolgende Messpunkte gilt:

\[
D_i^{(1)}=
\frac{pH_{i+1}-pH_i}{V_{i+1}-V_i}
\]

Der Wert wird nicht einem der beiden ursprünglichen Volumenwerte zugeordnet, sondern dem Mittelpunkt:

\[
V_i^{(1)}=\frac{V_i+V_{i+1}}{2}
\]

Bei einer steigenden Titrationskurve liegt im steilsten Bereich ein Maximum der ersten Ableitung. Bei einer fallenden Kurve entsteht entsprechend ein Minimum.

<!-- GIF 05: titrationstool-erste-ableitung.gif
     Von der Kurve zur ersten Ableitung wechseln und optional die Titrationskurve überlagern. -->

## Zweite Ableitung

Die zweite Ableitung wird aus benachbarten Punkten der ersten Ableitung berechnet:

\[
D_i^{(2)}=
\frac{D_{i+1}^{(1)}-D_i^{(1)}}
{V_{i+1}^{(1)}-V_i^{(1)}}
\]

Auch diese Werte werden an den jeweiligen Volumenmittelpunkten eingetragen. Im Bereich des Wendepunkts der Titrationskurve wechselt die zweite Ableitung ihr Vorzeichen. Der Nulldurchgang wird linear interpoliert.

Das TITRATIONSTOOL akzeptiert nicht jeden beliebigen Nulldurchgang als Äquivalenzpunkt. Es sucht zusätzlich nach einem ausreichend markanten Extremum der ersten Ableitung und ordnet diesem einen nahe gelegenen, zur Kurvenrichtung passenden Nulldurchgang der zweiten Ableitung zu.

- steigende Kurve: positiv-negativer Nulldurchgang nahe einem Maximum der ersten Ableitung
- fallende Kurve: negativ-positiver Nulldurchgang nahe einem Minimum der ersten Ableitung

Diese Kombination reduziert Fehlzuordnungen durch kleine numerische Schwankungen.

<!-- GIF 06: titrationstool-zweite-ableitung-aep.gif
     Zweite Ableitung, Nulllinie und interpolierter Nulldurchgang; Kurve optional überlagert. -->

!!! note "Keine Glättung"
    Die Ableitungen werden unmittelbar aus den aufgenommenen Messwerten berechnet. Es erfolgt keine Glättung, Polynom-Anpassung oder nachträgliche Verdichtung der Messreihe. Dadurch wird der Einfluss der gewählten Tropfengröße sichtbar.

## Titrationskurve und Ableitung überlagern

Bei der ersten und zweiten Ableitung kann die ursprüngliche Titrationskurve eingeblendet werden. Beide Größen verwenden getrennte y-Achsen. So bleibt die pH-Kurve didaktisch dominant, während gleichzeitig sichtbar wird,

- dass das Extremum der ersten Ableitung im steilsten Kurvenbereich liegt,
- dass der Nulldurchgang der zweiten Ableitung mit dem Wendebereich zusammenfällt.

Diese Darstellung eignet sich besonders für eine gemeinsame Besprechung am Beamer.

## Indikatoren und Umschlagsbereiche

Die Auswahl eines Indikators erfolgt nicht nach dem Prinzip „sauer oder basisch“, sondern nach der Lage seines Umschlagsbereichs im steilen Bereich der jeweiligen Titrationskurve.

Enthalten sind:

- Bromthymolblau: gelb → grün → blau
- Phenolphthalein: farblos → pink
- Methylorange: rot → gelb
- Thymolblau: zwei getrennte Umschlagsbereiche
- Universalindikator: schematische Farbskala über den gesamten pH-Bereich

Die Umschlagsbereiche werden als dezente Bänder im Diagramm angezeigt. Das Programm vergleicht außerdem den berechneten pH-Wert am Äquivalenzpunkt mit dem gewählten Bereich.

<!-- GIF 07: titrationstool-indikatoren.gif
     Bei identischem Versuch mehrere Indikatoren durchschalten; Farbe und Umschlagsband vergleichen. -->

!!! warning "Universalindikator"
    Ein Universalindikator ist ein Indikatorgemisch. Er eignet sich zur groben pH-Abschätzung, besitzt aber keinen einzelnen engen Umschlagsbereich und ist deshalb für eine präzise Endpunkterkennung ungeeignet.

## Hägg-Diagramme

Für schwache Säuren und Basen kann zusätzlich ein Hägg-Diagramm geöffnet werden. Es zeigt die relativen Anteile der beteiligten Protolyseformen in Abhängigkeit vom pH-Wert.

Bei einer einprotonigen Säure gilt am \(pK_\mathrm{s}\)-Wert:

\[
[HA]=[A^-]
\]

Bei zweiprotonigen Säuren werden drei Spezies dargestellt. Dadurch lässt sich erklären, warum zwei Neutralisationsstufen grundsätzlich möglich sind und weshalb ein Äquivalenzpunkt unter Umständen weniger deutlich ausgeprägt ist.

<!-- GIF 08: titrationstool-haegg.gif
     Hägg-Diagramm öffnen und pKs-Bereich einer ein- oder zweiprotonigen Säure zeigen. -->

## Der Halbäquivalenzpunkt

Bei der Titration einer einprotonigen schwachen Säure mit einer starken Base gilt am Halbäquivalenzpunkt:

\[
V_\mathrm{HÄP}=\frac{V_\mathrm{ÄP}}{2}
\]

Zu diesem Zeitpunkt wurde die Hälfte der ursprünglichen Säuremenge in ihre konjugierte Base umgewandelt. Daher gilt:

\[
[HA]=[A^-]
\]

Aus der Henderson-Hasselbalch-Beziehung folgt:

\[
pH=pK_\mathrm{s}
\]

Diese Beziehung wird in der abschließenden Identifikationsaufgabe genutzt.

## Challenge: eine unbekannte schwache Säure bestimmen

Eine unbekannte einprotonige schwache Säure wird mit Natronlauge titriert. Die SchülerInnen müssen:

1. den Äquivalenzpunkt bestimmen,
2. den Halbäquivalenzpunkt berechnen,
3. den pH-Wert an dieser Stelle ablesen,
4. \(pH=pK_\mathrm{s}\) anwenden,
5. den Stoff anhand einer Kandidatenliste identifizieren.

Der Kandidatenpool umfasst:

| Kandidat | \(pK_\mathrm{s}\) |
|---|---:|
| Chloressigsäure | 2,86 |
| Ameisensäure | 3,75 |
| Benzoesäure | 4,20 |
| Essigsäure | 4,76 |
| Pyridinium-Ion aus Pyridiniumchlorid | 5,23 |

Bei jedem Neuladen werden Stoff und Konzentration neu gewählt. Das Äquivalenzvolumen bleibt zwischen 9 und 15 mL. Eine unmittelbare Wiederholung desselben Stoffes wird vermieden.

<!-- GIF 09: titrationstool-haep-challenge.gif
     Aufgabe laden, ÄP bestimmen, HÄP berechnen, pH ablesen und Kandidat auswählen. -->

## Geführte quantitative Auswertung

Vier Aufgaben führen schrittweise von der Messung zur Konzentration:

- unbekannte Salzsäure
- unbekannte Essigsäure
- unbekannte Ammoniaklösung
- unbekannte Oxalsäure über den zweiten Äquivalenzpunkt

Die Lernenden bestimmen nacheinander:

1. Äquivalenzvolumen
2. Stoffmenge der Maßlösung
3. Stoffmengenverhältnis
4. Stoffmenge des Analyten
5. Konzentration in mol/L
6. Massenkonzentration in g/L

Bei \(c\) in mol/L und \(V\) in mL gilt zahlenmäßig:

\[
n\,[\mathrm{mmol}]=c\,[\mathrm{mol\,L^{-1}}]\cdot V\,[\mathrm{mL}]
\]

Für eine 1:1-Reaktion folgt:

\[
c_\mathrm{Analyt}=
\frac{c_\mathrm{Maßlösung}\cdot V_\mathrm{ÄP}}
{V_\mathrm{Probe}}
\]

Allgemein mit dem stöchiometrischen Faktor \(z\):

\[
c_\mathrm{Analyt}=
\frac{c_\mathrm{Maßlösung}\cdot V_\mathrm{ÄP}}
{z\cdot V_\mathrm{Probe}}
\]

Die Massenkonzentration ergibt sich aus:

\[
\beta=c_\mathrm{Analyt}\cdot M_\mathrm{Analyt}
\]

Bei Oxalsäure wird ausdrücklich der zweite Äquivalenzpunkt verwendet. Dort wurden zwei Stoffmengen Hydroxidionen pro Stoffmenge Oxalsäure umgesetzt; deshalb ist \(z=2\).

<!-- GIF 10: titrationstool-gefuehrte-auswertung.gif
     Zufallsvariante, schrittweise Eingaben von V(ÄP) bis g/L, Rückmeldungen zeigen. -->

## Die neun Aufgaben im Überblick

| ID | Aufgabe | Niveau | Schwerpunkt |
|---|---|---|---|
| A01 | Starke Säure – Äquivalenzpunkt bei pH 7 | Grundlagen | Kurve und Äquivalenz-pH |
| A02 | Essigsäure – ÄP aus der zweiten Ableitung | SEK II | Nulldurchgang |
| A03 | Pyridin – geeigneten Indikator wählen | Vertiefung | Indikatorauswahl |
| A04 | Oxalsäure – zwei Äquivalenzpunkte | SEK II | zweiprotonige Säure |
| A05 | Unbekannte Salzsäure | geführt | quantitative Auswertung |
| A06 | Unbekannte Essigsäure | geführt | schwache Säure |
| A07 | Unbekannte Ammoniaklösung | geführt | fallende Kurve |
| A08 | Oxalsäure über den zweiten ÄP | geführt | Faktor 2 : 1 |
| A09 | Unbekannte schwache Säure aus dem HÄP | geführt | Stoffidentifikation |

## Export in das MESSWERT_LAB

Die Messreihe kann als CSV-Datei exportiert und im MESSWERT_LAB weiter ausgewertet werden. Der Export enthält ausschließlich die Rohdaten:

```text
Volumen_Massloesung_mL;pH
0,0000000000;...
0,1000000000;...
...
```

Nach einer Leerzeile folgt ein Metadatenblock mit den Versuchsparametern, beispielsweise:

- Titrationsart
- Analyt und Maßlösung
- Konzentrationen und Probenvolumen
- molare Masse
- Protonenstufen
- pKs-Werte
- Indikator
- Soll-Schrittweite
- Arbeitsbereich und Aufgaben-ID

Ableitungen und Äquivalenzpunkte werden nicht exportiert. Das MESSWERT_LAB berechnet diese Größen selbst nach demselben verbindlichen Standard `TITR_AEP_V1`. Dadurch können Simulation und Datenlabor unabhängig voneinander arbeiten und dennoch dieselben Ergebnisse liefern.

<!-- GIF 11: titrationstool-export-messwertlab.gif
     CSV exportieren, im MESSWERT_LAB öffnen, Kurve/Ableitungen darstellen. -->

## Vorschläge für den Unterricht

### Einstieg: Warum liegt der Äquivalenzpunkt nicht immer bei pH 7?

1. Salzsäure mit Natronlauge titrieren.
2. Essigsäure mit Natronlauge titrieren.
3. Beide Kurven vergleichen.
4. Lage und pH-Wert des Äquivalenzpunkts erklären.

Zeitbedarf: etwa 20–30 Minuten.

### Ableitungen als Auswertungswerkzeug

1. Messreihe mit grober Schrittweite aufnehmen.
2. Erste und zweite Ableitung betrachten.
3. Messung mit kleinerer Schrittweite wiederholen.
4. Genauigkeit und Kurvenform vergleichen.

Zeitbedarf: etwa 30 Minuten.

### Indikatorwahl

1. Eine schwache Säure und eine schwache Base titrieren.
2. Äquivalenz-pH bestimmen.
3. mehrere Indikatoren vergleichen.
4. eine begründete Auswahl treffen.

Zeitbedarf: etwa 20 Minuten.

### Quantitative Analyse

Eine der geführten Aufgaben laden und die Konzentration vollständig bis zur Einheit g/L auswerten. Anschließend können die exportierten Daten im MESSWERT_LAB unabhängig kontrolliert werden.

Zeitbedarf: etwa 30–40 Minuten.

### Stoffidentifikation

Die HÄP-Challenge eignet sich als abschließende Anwendung nach der Einführung der Henderson-Hasselbalch-Beziehung.

Zeitbedarf: etwa 25–30 Minuten.

## Hinweise für Lehrkräfte

- Die Titrationskurve sollte zunächst immer qualitativ gelesen werden, bevor die Ableitungen verwendet werden.
- Große Tropfengrößen sind didaktisch nützlich, um den Einfluss der Messpunktdichte sichtbar zu machen.
- Die automatische Äquivalenzpunktbestimmung sollte nicht als „richtige Antwort aus dem Computer“, sondern als nachvollziehbares mathematisches Verfahren behandelt werden.
- Bei schwachen Säuren und Basen sollte der pH-Wert am Äquivalenzpunkt ausdrücklich mit der Protolyse des entstandenen konjugierten Teilchens verknüpft werden.
- Bei Oxalsäure ist der erste Äquivalenzpunkt weniger markant. Dies ist kein Programmfehler, sondern Folge der Gleichgewichtslage und der relativ nahen pKs-Werte.
- Der Universalindikator sollte bewusst als ungeeignetes Werkzeug für eine präzise Endpunkterkennung diskutiert werden.
- Die Apparaturdarstellung unterstützt das Verständnis, ersetzt aber keine praktische Laborübung.

## Fachliche Modellgrenzen

Das TITRATIONSTOOL konzentriert sich bewusst auf den schulischen Kernbereich der Protolyseanalytik. Nicht abgebildet werden unter anderem:

- Aktivitätskoeffizienten und Ionenstärke
- temperaturabhängige Gleichgewichtskonstanten
- gekoppelte Carbonat- oder Sulfitsysteme
- dreiprotonige Säuren
- mehrprotonige schwache Basen
- schwache Säure mit schwacher Base
- Fällungs-, Redox- und komplexometrische Titrationen
- reale Geräte- und Bedienfehler

Diese Begrenzung hält die Modelle fachlich nachvollziehbar und die Benutzeroberfläche übersichtlich.

## Technische Voraussetzungen

- aktueller Webbrowser
- JavaScript aktiviert
- Internetverbindung zum Laden der Diagrammbibliothek Chart.js
- keine Installation
- keine Anmeldung
- keine Übertragung der Messdaten an einen Server

Die Berechnungen erfolgen lokal im Browser. Die Anwendung ist responsiv und kann am Computer, Tablet oder Smartphone geöffnet werden; für eine ausführliche Diagrammauswertung ist ein größerer Bildschirm empfehlenswert.

## Zusammenfassung

Das TITRATIONSTOOL verbindet drei Ebenen, die im Unterricht oft getrennt behandelt werden:

1. **Versuchsdurchführung:** Maßlösung zugeben, pH-Wert beobachten, Indikatorfarbe verfolgen.
2. **Messdatenauswertung:** Kurve, erste und zweite Ableitung, Äquivalenzpunkt.
3. **chemische Interpretation:** Protolysegleichgewichte, Indikatorwahl, Halbäquivalenzpunkt und quantitative Analyse.

Der freie Laborbereich ermöglicht eigenes Erkunden. Die begleitenden Aufgaben machen daraus ein unmittelbar einsetzbares Unterrichtswerkzeug. Über die CSV-Schnittstelle können die Rohdaten anschließend im MESSWERT_LAB unabhängig weiterverarbeitet werden.
