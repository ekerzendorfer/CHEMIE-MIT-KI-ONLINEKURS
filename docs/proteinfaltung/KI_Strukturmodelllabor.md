# KI-Strukturmodell-Labor

!!! info "Kurzidee"
    Das KI-Strukturmodell-Labor zeigt, wie man experimentelle Proteinstrukturen und KI-Strukturmodelle didaktisch sinnvoll vergleicht.  
    Im Mittelpunkt steht nicht die Frage „richtig oder falsch?“, sondern: **Was zeigt ein Modell gut – und wo braucht es Kontext?**

## Worum geht es?

Proteine sind keine starren Gebilde. Ihre Funktion hängt davon ab,

- wie ihre Aminosäurekette gefaltet ist,
- welche Bereiche beweglich oder geordnet sind,
- ob Ionen, Liganden oder andere Moleküle gebunden sind,
- und welcher experimentelle oder biologische Zustand betrachtet wird.

KI-Modelle wie AlphaFold oder ColabFold sind sehr leistungsfähig, aber sie ersetzen experimentelle Strukturaufklärung nicht vollständig. Sie liefern Strukturmodelle, die interpretiert werden müssen.

Das Tool macht diese Unterscheidung sichtbar:

```text
Sequenz → KI-Strukturmodell → experimentelle Struktur → Overlay → Unterschiede → Modellgrenzen
```

## Lernziele

Nach der Arbeit mit dem Tool sollen Schüler:innen bzw. Kursteilnehmer:innen erklären können:

1. Warum die räumliche Struktur eines Proteins für seine Funktion entscheidend ist.
2. Was der Unterschied zwischen experimenteller Struktur und Strukturmodell ist.
3. Warum ein gutes Overlay hilfreich, aber nicht die ganze Aussage ist.
4. Wie der Modus **Unterschiede** zu lesen ist.
5. Warum Liganden, Ionen und Konformationszustände für die Interpretation wichtig sind.
6. Warum KI-Modelle besonders stark sind, aber fachlich eingeordnet werden müssen.

## Empfohlene Reihenfolge der Beispiele

### 1. Ubiquitin – ein stabiles Referenzprotein

Ubiquitin eignet sich gut als Einstieg, weil die Grundfaltung sehr stabil und kompakt ist.  
Im Overlay stimmen experimentelle Struktur und gutes KI-Modell meist deutlich überein.

**Didaktische Kernidee:**  
Manchmal ist gerade das Fehlen großer Unterschiede die wichtigste Beobachtung.

**Arbeitsauftrag:**

1. Experiment und bestes Modell vergleichen.
2. Danach **Unterschiede** aktivieren.
3. Prüfen: Welche Bereiche werden überhaupt markiert?
4. Deuten: Ein gutes KI-Modell kann die Grundfaltung sehr gut treffen, sagt aber noch nicht alles über Dynamik, Bindungspartner oder Funktion aus.

### 2. Trp-cage – kleines Peptid, größere Beweglichkeit

Trp-cage zeigt, dass kleine Peptide und flexible Bereiche schwieriger zu interpretieren sein können.  
Abweichungen bedeuten hier nicht automatisch „falsch“, sondern können auf Beweglichkeit, Randbereiche oder unterschiedliche Modellzustände hinweisen.

**Didaktische Kernidee:**  
Ein Strukturmodell ist ein Vorschlag für eine mögliche räumliche Anordnung, nicht immer eine endgültige Form.

**Arbeitsauftrag:**

1. Gesamtform vergleichen.
2. Seitenketten betrachten.
3. **Unterschiede** aktivieren.
4. Markierte Bereiche als Hinweis auf flexible oder unsichere Abschnitte deuten.

### 3. Calmodulin – Zustand, Ca²⁺ und Kontext

Calmodulin ist besonders geeignet, um den Begriff **Zustand** zu diskutieren.  
Die experimentelle Struktur 1CLL zeigt den Ca²⁺-gebundenen Zustand. Modelle ohne expliziten Kontext können davon abweichen.

**Didaktische Kernidee:**  
Bei Proteinen mit beweglichen Domänen und Ionenbindung reicht die Sequenz allein oft nicht aus, um den betrachteten Zustand vollständig zu verstehen.

**Arbeitsauftrag:**

1. Ca²⁺-Ionen einschalten und lokalisieren.
2. Experimentelle Struktur mit verschiedenen Modellen vergleichen.
3. **Unterschiede** nutzen, um Endbereiche, Linker und Domänenorientierung sichtbar zu machen.
4. Erklären: Die Frage ist nicht nur „Wie faltet sich Calmodulin?“, sondern „In welchem Zustand befindet es sich?“

### 4. Maltose-Bindeprotein – vom Schlüssel-Schloss-Modell zu induced fit

Das Maltose-Bindeprotein, kurz MBP, ist das didaktisch stärkste Beispiel für eine Konformationsänderung.  
Es ist kein Enzym, sondern ein Bindeprotein. Gerade deshalb kann man sich auf Bindung und Formänderung konzentrieren.

Verglichen werden zwei experimentelle Strukturen:

```text
1OMP → offen / ohne Maltose
1ANF → geschlossen / mit Maltose
```

**Didaktische Kernidee:**  
Die Maltose passt nicht einfach in eine starre Tasche. Das Protein verändert seine räumliche Gestalt und schließt sich um den Liganden.

## Der Modus „Unterschiede“

Der Modus **Unterschiede** ist eine Beobachtungs- und Deutungshilfe.

!!! warning "Wichtig"
    Die farbigen Markierungen bedeuten nicht automatisch: „Hier ist das Modell falsch.“  
    Sie zeigen Bereiche, in denen zwei Strukturen nach der Überlagerung besonders deutlich voneinander abweichen.

Je nach Beispiel hat der Unterschiede-Modus eine etwas andere didaktische Funktion:

| Beispiel | Was der Unterschiede-Modus zeigen soll |
|---|---|
| Ubiquitin | Geringe Abweichungen als Hinweis auf sehr gute Grundfaltung |
| Trp-cage | Auffällige Bereiche bei einem kleinen, flexiblen Peptid |
| Calmodulin | Zustand, Ca²⁺-Kontext, Endbereiche und Domänenorientierung |
| MBP | Domänenbewegung zwischen offenem und geschlossenem Zustand |

## MBP: empfohlener Unterrichtsablauf

Für MBP hat sich folgende Reihenfolge bewährt:

### Schritt 1: Offene Form betrachten

Zuerst nur die offene Struktur anzeigen.

Leitfragen:

- Wo erkennt man die beiden Domänen?
- Wie offen wirkt die Spalte zwischen den Domänen?
- Wo liegt die spätere Bindetasche?

### Schritt 2: Bindetasche hervorheben

Die offene Bindetasche wird hellviolett markiert.

Leitfragen:

- Liegt die spätere Bindetasche frei zugänglich?
- Welche Teile des Proteins grenzen die Tasche ein?

### Schritt 3: Geschlossene Form mit Maltose betrachten

Die Maltose ist hellblau markiert, die geschlossene Bindetasche orange.

Leitfragen:

- Wo sitzt die Maltose?
- Wie verändert sich die Umgebung der Bindetasche?
- Warum ist hier der Begriff „Bindetasche“ besser als „aktives Zentrum“?

### Schritt 4: Offen + geschlossen vergleichen

Nun beide experimentellen Zustände gemeinsam betrachten.

Leitfragen:

- Welche Domänen liegen in der geschlossenen Form anders?
- Wird die Bindungstasche enger?
- Warum ist die Überlagerung eindrucksvoll, aber für Lernende zunächst schwer zu lesen?

### Schritt 5: Unterschiede aktivieren

Im MBP-Unterschiedsmodus wird eine Ankerdomäne als Bezugspunkt verwendet.  
Die bewegte Domäne wird als Bändermodell hervorgehoben, Seitenketten bleiben auf die Bindetasche beschränkt.

Leitfragen:

- Welche Domäne bewegt sich relativ zur Ankerdomäne?
- In welche Richtung schließt sich das Protein?
- Warum ist das ein Beispiel für **induced fit**?

!!! note "Keine Animation"
    Die Ansicht **Unterschiede** ist kein Bewegungsfilm.  
    Sie zeigt zwei experimentelle Endzustände so, dass die Domänenbewegung besser erkennbar wird.

## Schlüssel-Schloss und induced fit

Das klassische Schlüssel-Schloss-Modell ist als Einstieg hilfreich:

```text
Ligand passt zur Bindestelle.
```

Bei MBP reicht dieses Bild aber nicht aus. Die bessere Deutung lautet:

```text
Die Bindung der Maltose stabilisiert eine geschlossene Form des Proteins.
Das Protein passt seine Gestalt an den Liganden an.
```

Das ist die didaktische Brücke zum Konzept **induced fit**.

## AlphaFold, ColabFold und AF3 im Kontext

AlphaFold und ColabFold können sehr gute Strukturmodelle erzeugen.  
Trotzdem muss man unterscheiden:

| Modelltyp | Was es gut zeigt | Was kritisch bleibt |
|---|---|---|
| AlphaFold/ColabFold aus Sequenz | wahrscheinliche Grundfaltung | Zustand, Liganden, Ionen, Beweglichkeit |
| AlphaFold-DB | öffentlich verfügbares Proteinmodell | keine Nicht-Protein-Komponenten |
| AF3 mit Kontext | kann zusätzliche Moleküle berücksichtigen | öffentlicher Server erlaubt nur ausgewählte Liganden |
| Experimentelle Struktur | konkreter beobachteter Zustand | abhängig von Methode, Bedingungen und Auflösung |

!!! info "AF3 und Liganden"
    Der öffentliche AlphaFold Server erlaubt derzeit nur eine begrenzte Auswahl an Liganden. Für Maltose ist daher ohne lokale AlphaFold-3-Installation oder alternative Spezialwerkzeuge kein einfacher Server-Workflow verfügbar.  
    Das ist kein Misserfolg, sondern ein guter Anlass, über die Grenzen aktueller Werkzeuge zu sprechen.

## Protokollvorschlag

Schüler:innen sollten ihre Beobachtungen nicht nur anklicken, sondern schriftlich begründen.

Ein einfaches Protokollschema:

```text
1. Welche Strukturen wurden verglichen?
2. Welche Bereiche stimmen gut überein?
3. Welche Bereiche werden im Unterschiede-Modus hervorgehoben?
4. Sind diese Unterschiede eher Hinweis auf Fehler, Beweglichkeit, Zustand oder Kontext?
5. Welche Modellgrenze lässt sich daraus ableiten?
```

Für MBP zusätzlich:

```text
6. Wie verändert sich die Bindetasche beim Übergang offen → geschlossen?
7. Warum zeigt MBP induced fit besser als ein starres Schlüssel-Schloss-Modell?
```

## Typische Missverständnisse

### „Die rote Markierung zeigt Fehler.“

Nicht unbedingt. Sie zeigt zunächst nur starke geometrische Abweichung nach der Überlagerung.

### „AlphaFold ersetzt Experimente.“

Nein. KI-Modelle sind enorm hilfreich, aber experimentelle Strukturen zeigen konkrete Zustände, gebundene Moleküle und reale Bedingungen.

### „Eine Proteinstruktur ist eine feste Form.“

Nur teilweise. Viele Proteine bewegen sich, wechseln Zustände oder werden durch Liganden, Ionen oder Partner stabilisiert.

### „Wenn zwei Modelle verschieden aussehen, ist eines falsch.“

Nicht automatisch. Sie können unterschiedliche Zustände, Bedingungen oder Modellannahmen widerspiegeln.

## Einbettung in den Unterricht

Geeignet für:

- SEK II / Oberstufe
- Wahlpflichtfach Chemie oder Biologie
- Chemieolympiade / Begabtenförderung
- Lehrer:innenfortbildung
- Einstieg in Strukturbiologie, Bioinformatik und KI in den Naturwissenschaften

Mögliche Unterrichtsfrage:

> Wie verändert KI die Strukturbiologie – und warum bleibt fachliche Interpretation trotzdem unverzichtbar?

## Quellen und weiterführende Links

- RCSB PDB 1OMP – Maltose-Bindeprotein offen: <https://www.rcsb.org/structure/1OMP>
- RCSB PDB 1ANF – Maltose-Bindeprotein mit Maltose: <https://www.rcsb.org/structure/1ANF>
- AlphaFold Protein Structure Database FAQ: <https://alphafold.ebi.ac.uk/faq>
- AlphaFold 3 Input Documentation: <https://github.com/google-deepmind/alphafold3/blob/main/docs/input.md>
- Nobel Prize in Chemistry 2024: <https://www.nobelprize.org/prizes/chemistry/2024/summary/>
- Nobel Prize in Chemistry 2017: <https://www.nobelprize.org/prizes/chemistry/2017/summary/>
