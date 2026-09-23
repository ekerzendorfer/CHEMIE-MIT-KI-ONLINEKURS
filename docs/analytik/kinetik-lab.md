# KINETIK-LAB – vom Phänomen zum Geschwindigkeitsgesetz

Das **KINETIK-LAB** ist eine browserbasierte Lernumgebung zur photometrischen Reaktionskinetik. Im Mittelpunkt steht nicht das bloße Abspielen einer Simulation, sondern ein vollständiger Erkenntnisweg von einer überraschenden Beobachtung über die Planung und virtuelle Erprobung einer Messstrategie bis zur Auswertung realer Messdaten.

[**KINETIK-LAB öffnen**](https://ekerzendorfer.github.io/KINETIK_LAB/){ .md-button .md-button--primary }

!!! info "Aktueller Entwicklungsstand"
    **Version v0.1.9** ist ein fortgeschrittener Entwicklungsprototyp. Der zentrale Referenzfall der Kristallviolett-Kinetik wurde inzwischen an einem realen Schulversuch kalibriert. Weitere Realmessungen dienen der Überprüfung und Verfeinerung, nicht dem „Glattziehen“ experimenteller Abweichungen.

## Das Beispiel

Ausgangspunkt ist eine einfache Beobachtung aus dem Labor: Eine violette Kristallviolett-Lösung entfärbt sich in einem Becherglas deutlich schneller als erwartet. Erst nach einer ersten Diskussion wird die Zusatzinformation gegeben, dass sich im Gefäß noch **Reste von Natronlauge** befanden.

Aus dieser Beobachtung entwickeln die SchülerInnen schrittweise eine quantitative Fragestellung:

**Wie lässt sich das Verschwinden der Farbe messen – und was kann aus dem zeitlichen Verlauf über die Reaktionskinetik abgeleitet werden?**

## Der Lernweg

Das KINETIK-LAB führt in fünf aufeinander aufbauenden Phasen durch die Untersuchung:

1. **Beobachten und Hypothesen bilden**  
   Eine unerwartete Farbänderung wird beschrieben und zunächst ohne fertige Erklärung diskutiert.

2. **Messung planen**  
   Die SchülerInnen überlegen, wie Farbintensität quantitativ erfasst werden kann, skizzieren einen erwarteten Verlauf und entwickeln einen ersten Messplan.

3. **Virtuell erproben**  
   Wellenlänge, Messintervall und Messdauer werden getestet. Ungeeignete Strategien dürfen ausdrücklich ausprobiert und verbessert werden.

4. **Real messen**  
   Der entwickelte Plan wird – sofern ein geeignetes Photometer oder Colorimeter vorhanden ist – im realen Experiment umgesetzt. Alternativ können reale Referenzdaten oder ein bereitgestellter Testdatensatz verwendet werden.

5. **Aus Messdaten Erkenntnisse ableiten**  
   Rohdaten werden geprüft, reale und virtuelle Kurven verglichen und unterschiedliche mathematische Darstellungen untersucht. Daraus werden schrittweise Aussagen zur Reaktionsordnung und zum Geschwindigkeitsgesetz entwickelt.

!!! tip "Didaktischer Kern"
    Das KINETIK-LAB ersetzt weder den realen Versuch noch den vorhergehenden Unterricht zur Reaktionskinetik. Es soll vorhandenes Wissen auf eine reale Messsituation anwenden helfen und den Weg **Messwert → Messkurve → mathematische Darstellung → kinetische Aussage** sichtbar machen.

## Real kalibriert – aber nicht realitätskosmetisiert

Der zentrale virtuelle Referenzfall wurde inzwischen an einer realen Messung mit einem **Vernier Colorimeter bei 565 nm** abgestimmt.

Für den derzeitigen Referenzansatz gelten:

- c₀(CV⁺) = **1,20 × 10⁻⁵ mol/L**
- c₀(OH⁻) = **0,0300 mol/L**
- k_app ≈ **0,00534 s⁻¹**
- A∞ ≈ **0,01136**
- reale Startverzögerung durch Mischen und Überführen: etwa **15 s**

Die Startverzögerung wird dokumentiert, aber **nicht künstlich in das virtuelle Reaktionsmodell eingebaut**.

Wichtig ist die Trennung zwischen:

- **real gemessen**,
- **aus Messdaten gefittet**,
- **im Modell vorhergesagt**.

Die weiteren OH⁻-Konzentrationen werden derzeit noch aus dem kalibrierten Modell abgeleitet und sollen später ebenfalls durch Realmessungen überprüft werden.

!!! note
    Abweichungen zwischen realen und virtuellen Kurven werden nicht verborgen. Sie gehören zur Diskussion über Messunsicherheit, Modellgrenzen und die Aussagekraft experimenteller Daten.

## Zusammenspiel mit dem SpektralLab

Das **SpektralLab** bleibt das offenere virtuelle Messgerät; das **KINETIK-LAB** ist dagegen als konkrete Forschungssequenz aufgebaut.

Im KINETIK-LAB wird der Erkenntnisweg strukturiert:

**Beobachten → Planen → Erproben → Real messen → Auswerten → Interpretieren**

Das SpektralLab kann ergänzend für photometrische Grundlagen und weitere virtuelle Messungen verwendet werden. Der kinetische Kern soll in einer späteren Version noch auf denselben real kalibrierten Referenzfall abgestimmt werden.

[**SpektralLab – Virtuelles Photometer öffnen**](https://ekerzendorfer.github.io/VIRTUELLES_PHOTOMETER/){ .md-button }

## Anleitungen

Die beiden Anleitungen sind direkt an den Phasen der App orientiert.

[**Kurzanleitung für SchülerInnen**](kinetik-lab-schuelerinnen.md){ .md-button }

[**Anleitung für LehrerInnen**](kinetik-lab-lehrerinnen.md){ .md-button }

Die SchülerInnen-Anleitung begleitet durch die einzelnen Arbeitsschritte, ohne die fachlichen Lösungen vorwegzunehmen. Die LehrerInnen-Anleitung ergänzt didaktische Hinweise, erwartbare Schülerideen, Hinweise zum Realexperiment, Referenzwerte und den aktuellen Validierungsstand.

## Videos zum Realexperiment

Zwei kurze Videos zeigen die qualitative Entfärbung und die praktische Datenerfassung mit dem Vernier Colorimeter. Die derzeit vorhandenen Fassungen sind noch unbearbeitet und werden vor der endgültigen Veröffentlichung ergänzt.

<!--
Qualitative Beobachtung der Entfärbung:
https://youtu.be/hc1YmpWaESE

Datenerfassung mit Vernier Colorimeter:
https://youtu.be/XL6rqaDQCKs
-->

---

## KI bei der Entwicklung

Die Messwerte der App werden nicht von einer generativen KI „erfunden“.

Die Rollen sind klar getrennt:

- **Reales Experiment:** liefert den empirischen Referenzpunkt.
- **Fachmodell:** beschreibt den chemisch-mathematischen Zusammenhang.
- **Generative KI:** unterstützt bei Programmierung, Gestaltung des Lernwegs, Formulierung von Hilfen und iterativer Überarbeitung.

**Nicht die KI entscheidet, was chemisch richtig ist – das Modell muss sich an realen Messungen und fachlichen Kriterien bewähren.**
