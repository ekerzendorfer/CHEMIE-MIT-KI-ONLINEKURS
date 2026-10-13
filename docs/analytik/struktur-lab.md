# STRUKTUR-LAB – Spektren verstehen und Strukturen aufklären

Das **STRUKTUR-LAB** ist eine browserbasierte Lernumgebung zur organischen Strukturaufklärung. Es verbindet experimentell bestimmte Molmasse, Massenspektrometrie, IR-Spektroskopie und ¹H-NMR zu einem schrittweisen Analyseweg.

Die Lernenden erhalten nicht sofort einen Stoffnamen, sondern entwickeln aus mehreren unabhängigen Befunden eine begründete Strukturhypothese.

[**STRUKTUR-LAB öffnen**](https://ekerzendorfer.github.io/STRUKTUR_LAB/){ .md-button .md-button--primary }

[**Expertenmodus direkt öffnen**](https://ekerzendorfer.github.io/STRUKTUR_LAB/expert.html){ .md-button }

[**Quellcode auf GitHub**](https://github.com/ekerzendorfer/STRUKTUR_LAB){ .md-button }

<!-- ABBILDUNG SL-01
     DATEI: ../assets/images/analytik/struktur-lab/sl01_ueberblick.webp
     MOTIV: Gesamtansicht des STRUKTUR-LABs mit Schrittleiste, Spektrum und Analysenjournal.
     PRIORITÄT: A
     EMPFOHLENE BREITE: 1200–1400 px -->

## Die Grundidee

Bei einer realen Strukturaufklärung liefert keine einzelne Methode allein die vollständige Lösung.

Das STRUKTUR-LAB führt deshalb mehrere Informationsquellen zusammen:

1. **Molare Masse**
2. **Massenspektrum**
3. **IR-Spektrum**
4. **¹H-NMR-Spektrum**
5. **Stoffklasse und Strukturhypothese**

Zu jeder Phase wird ein kurzer eigener Befund dokumentiert. Erst danach wird die nächste Methode freigeschaltet.

!!! info "Didaktischer Schwerpunkt"
    Die Spektren sollen nicht nur betrachtet, sondern **interpretiert und miteinander verknüpft** werden. Entscheidend ist die Frage: Welche Struktur erklärt gleichzeitig Molmasse, Fragmentierung, funktionelle Gruppen und Protonenumgebungen?

## Schrittweise Strukturaufklärung

### Molare Masse

Zu Beginn steht eine experimentell bestimmte molare Masse zur Verfügung. Sie grenzt mögliche Strukturen ein, beweist aber noch keine Identität.

Im Basismodus wird zusätzlich die Summenformel als Hilfe angegeben.

Im Expertenmodus ist sie zunächst nicht bekannt.

### Massenspektrometrie

Im EI-Massenspektrum können Molekülion und charakteristische Fragmente untersucht werden.

Nach der später gelösten Struktur steht für ausgewählte Stoffe zusätzlich eine Lernhilfe zu diagnostischen Fragmenten zur Verfügung. Dabei wird nicht nur der Peak genannt, sondern auch gezeigt, welches geladene Fragment zu diesem Signal führen kann.

### IR-Spektroskopie

Das IR-Spektrum unterstützt vor allem bei der Identifikation funktioneller Gruppen.

Orientierungsbereiche können bei Bedarf eingeblendet werden; auch der Fingerprintbereich lässt sich hervorheben.

### ¹H-NMR

Das ¹H-NMR liefert Informationen über

- die Zahl unterschiedlicher Protonenumgebungen,
- chemische Verschiebungen,
- relative Integrale,
- Multiplizitäten
- und einfache Kopplungsmuster.

Nach gelöster Struktur können NMR-Signale direkt den zugehörigen Protonengruppen in der Strukturformel zugeordnet werden.

<!-- GIF SL-02
     DATEI: ../assets/images/analytik/struktur-lab/sl02_analyseweg.gif
     MOTIV: kurzer Ablauf MS → IR → ¹H-NMR mit Wechsel zwischen den Phasen und Eintrag ins Journal.
     PRIORITÄT: A
     EMPFOHLENE LÄNGE: 12–18 s -->

## Von der Stoffklasse zur Struktur

Nach MS, IR und ¹H-NMR muss zunächst eine **Stoffklasse** gewählt werden.

Erst wenn diese mit den bisherigen Daten vereinbar ist, werden mögliche Strukturkandidaten freigeschaltet.

Die Strukturkarten zeigen bewusst zunächst keine Namen. Die Entscheidung soll anhand der Strukturformeln und der zuvor dokumentierten Spektrenbefunde getroffen werden.

Anschließend muss die gewählte Struktur kurz begründet und erst danach der Stoffname zugeordnet werden.

<!-- ABBILDUNG SL-03
     DATEI: ../assets/images/analytik/struktur-lab/sl03_strukturhypothese.webp
     MOTIV: Phase Hypothese mit Stoffklassenwahl, Strukturkarten und Begründungsfeld; Stoffname möglichst noch nicht sichtbar.
     PRIORITÄT: A -->

## Geführter Modus und Expertenmodus

Das STRUKTUR-LAB besitzt zwei Anspruchsniveaus.

### Basismodus

Im Basismodus ist die Summenformel von Beginn an bekannt. Der Schwerpunkt liegt auf dem schrittweisen Lesen und Kombinieren von MS-, IR- und NMR-Informationen.

### Expertenmodus

Im Expertenmodus steht zunächst nur die experimentell bestimmte molare Masse zur Verfügung.

Die Summenformel kann über eine **Elementaranalyse** selbst erschlossen werden:

Massenanteile → Verhältnisformel → molare Masse der Verhältnisformel → Faktor \(n\) → Summenformel.

Für fortgeschrittene Lernende kann die Elementaranalyse aber auch bewusst **übersprungen** werden. Dann wird das Massenspektrum ohne vorab bekannte Summenformel freigeschaltet.

Damit entsteht ein deutlich offenerer Analyseweg:

**M → MS → IR → ¹H-NMR → Strukturhypothese**

Erst aus der korrekt gelösten Struktur ergibt sich anschließend auch die Summenformel.

<!-- ABBILDUNG SL-04
     DATEI: ../assets/images/analytik/struktur-lab/sl04_expertenmodus.webp
     MOTIV: Expertenmodus in Phase M mit den beiden Optionen „Elementaranalyse durchführen“ und „Ohne Elementaranalyse weiter“.
     PRIORITÄT: A -->

## Spektrenwerkstatt nach gelöster Struktur

Nach korrekter Struktur- und Namenszuordnung wird eine zusätzliche **Spektrenwerkstatt** geöffnet.

Sie dient nicht mehr dem Lösen des Falls, sondern dem rückblickenden Verstehen.

Dort können Lernende

- diagnostische MS-Fragmente genauer untersuchen,
- IR-Bereiche nochmals gezielt interpretieren,
- NMR-Signale den Protonengruppen in der bestätigten Struktur zuordnen,
- und die Spektren mit alternativen Strukturkandidaten vergleichen.

Gerade dieser zweite Blick ist didaktisch wertvoll: Aus „Welcher Stoff könnte das sein?“ wird die Frage **„Warum passt diese Struktur besser als die Alternativen?“**

## Reale Referenzspektren

Seit Version 0.3.1 werden nach korrekt bestätigter Identität zusätzlich Links zu **experimentellen Referenzspektren** freigeschaltet.

Verwendet werden zwei frei zugängliche wissenschaftliche Datenquellen:

- **AIST SDBS** – integrierte Spektrendatenbank mit unter anderem EI-MS, FT-IR, ¹H-NMR und ¹³C-NMR,
- **NIST Chemistry WebBook** – Referenzdaten mit besonders umfangreichen MS- und IR-Spektren.

Die Links erscheinen absichtlich erst **nach** der gelösten Identität und können die eigentliche Strukturaufklärung daher nicht vorwegnehmen.

Der Vergleich zeigt zugleich eine wichtige Modellgrenze: Ein reales Spektrum muss nicht pixelgenau wie das didaktisch reduzierte Spektrum aussehen. Lösungsmittel, Aggregatzustand, Konzentration, Messgerät und Auflösung können die Darstellung beeinflussen.

<!-- ABBILDUNG SL-05
     DATEI: ../assets/images/analytik/struktur-lab/sl05_reale_spektren.webp
     MOTIV: gelöster Fall mit freigeschaltetem Bereich „Reale Referenzspektren“ und den Buttons AIST SDBS / NIST.
     PRIORITÄT: A -->

## Einsatz im Digitalen Analytiklabor

Das STRUKTUR-LAB arbeitet auch als Detail-Labor des **Digitalen Analytiklabors**.

Bei ausreichend reinen GC-Fraktionen wird ein anonymisierter Peak zur Strukturaufklärung übergeben. Das STRUKTUR-LAB erhält dabei intern den passenden kuratierten Fall, zeigt den Lernenden aber zunächst keine Stoffidentität.

Nach einer begründeten Strukturhypothese wird das Ergebnis an den Hub zurückgegeben. Dort gilt die Identität zunächst nur als **spektroskopisch gestützt**.

Die endgültige Bestätigung erfolgt anschließend unabhängig im GC-LAB über Referenzstandard und Aufstockung.

Beim organischen Feststoff aus VCÖ-01 kann der Expertenmodus zusätzlich die klassische Feststoff-Voranalyse überspringen. Dadurch lässt sich die Strukturaufklärung ohne bereits bekannte Funktionsgruppenhinweise beginnen.

[**Zum Digitalen Analytiklabor im Begleitkurs**](digitales-analytiklabor.md){ .md-button }

## Aktuell ausgearbeitete Stoffe

Derzeit stehen vollständig kuratierte Spektrensätze für folgende Stoffe zur Verfügung:

- Ethanol
- Dimethylether
- Ethylacetat
- 1-Butanol
- 2-Butanol
- Salicylsäure
- 3-Hydroxybenzoesäure
- 4-Hydroxybenzoesäure

Die Auswahl enthält bewusst auch Isomere und strukturell ähnliche Verbindungen. Dadurch reicht es nicht, nur ein einzelnes charakteristisches Signal zu erkennen; mehrere Befunde müssen gemeinsam bewertet werden.

## Modellgrenzen

Das STRUKTUR-LAB ist **kein universeller Spektrensimulator**.

Die Spektren sind für Unterricht und Training kuratiert und zum Teil bewusst reduziert. Ziel ist nicht die vollständige Reproduktion jedes experimentellen Details, sondern das Erkennen tragfähiger analytischer Zusammenhänge.

Gerade deshalb ist der abschließende Vergleich mit echten Referenzspektren eine sinnvolle Ergänzung: Er verbindet das didaktische Modell wieder mit experimenteller Realität.
