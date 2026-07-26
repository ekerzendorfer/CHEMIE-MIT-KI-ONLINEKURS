# KI-Strukturmodell-Labor

Das **KI-Strukturmodell-Labor** ist ein kleines Webtool zum Vergleich von KI-generierten Proteinstrukturmodellen mit experimentell bestimmten Strukturen.

Es ist bewusst kein vollständiges Strukturbiologie-Programm. Ziel ist ein geführter Lernweg:

> Sequenz → KI-Strukturmodell → experimentelle Struktur → Overlay → Modellgrenzen verstehen

## Didaktische Grundidee

Viele Schüler:innen begegnen AlphaFold und ähnlichen Werkzeugen zunächst mit der Vorstellung:

> Die KI berechnet die richtige Proteinstruktur.

Das Tool soll diese Aussage differenzieren. KI-Strukturmodelle sind oft außerordentlich stark, aber sie sind Modelle. Sie müssen im Kontext interpretiert werden:

- Welche Eingabe wurde verwendet?
- Ist ein Ligand, Ion oder Cofaktor beteiligt?
- Zeigt das Experiment einen bestimmten Zustand?
- Sind manche Bereiche flexibel oder ungeordnet?
- Was bedeutet eine sichtbare Abweichung wirklich?

## Die drei Beispielstufen

### 1. Trp-cage

Trp-cage ist ein sehr kleines Peptid. Es eignet sich als Einstieg, weil schon eine kurze Aminosäuresequenz eine räumliche Struktur bilden kann.

Didaktischer Fokus:

- kleine Peptide sind beweglich
- unterschiedliche Modellvorschläge können deutlich abweichen
- ein einzelnes Modell ist nicht automatisch „die“ endgültige Struktur

### 2. Ubiquitin

Ubiquitin ist ein kleines, stabiles Referenzprotein. Moderne KI-Modelle treffen die Grundfaltung sehr gut.

Didaktischer Fokus:

- KI-Modelle können experimentellen Strukturen sehr nahe kommen
- alternative Modelle sind nicht automatisch schlecht
- ein gutes Overlay ersetzt nicht die Interpretation von Funktion, Dynamik und Wechselwirkungen

### 3. Calmodulin

Calmodulin bindet Calcium-Ionen und zeigt zustandsabhängige Strukturunterschiede. Dieses Beispiel ist deutlich anspruchsvoller und eignet sich eher für interessierte Schüler:innen, Leistungskurse, Wahlpflichtfächer oder den Einstieg in Hochschulniveau.

Didaktischer Fokus:

- experimentelle Struktur = konkreter Ca²⁺-gebundener Zustand
- AF2/ColabFold = Sequenzmodell ohne explizit gesetzte Calcium-Ionen
- AlphaFold-DB = öffentliches AF2-Referenzmodell
- AF3 mit Ca²⁺ = Modell mit explizit angegebenem Cofaktor-Kontext
- mehr Kontext bedeutet nicht automatisch perfekte Übereinstimmung mit dem Experiment

## Modelltypen im Tool

| Modelltyp | Was zeigt es? | Was darf man nicht vorschnell schließen? |
|---|---|---|
| Experiment | Eine real gemessene Struktur unter bestimmten Bedingungen | Nicht automatisch alle möglichen Zustände |
| ColabFold / AF2 | Ein starkes Sequenzmodell | Keine expliziten Ionen, Liganden oder Zustände |
| AlphaFold-DB | Ein öffentliches Referenzmodell | Kein experimenteller Zustand |
| AF3 mit Kontext | Modell mit zusätzlichen Angaben wie Ca²⁺ | Nicht automatisch identisch mit dem Experiment |
| Didaktisches Störmodell | Bewusst stärker abweichendes Vergleichsmodell | Kein echtes AlphaFold-Ergebnis; muss klar gekennzeichnet werden |

## Vorschlag für einen Unterrichtsablauf

1. **Beobachten**  
   Schüler:innen betrachten zunächst nur die Gesamtform. Noch keine Wertung.

2. **Vergleichen**  
   Im Overlay werden übereinstimmende und abweichende Bereiche gesucht.

3. **Modellgrenze formulieren**  
   Am Ende steht keine Ja/Nein-Aussage, sondern eine begründete Modellkritik.

Beispielformulierung:

> Das KI-Modell trifft die Grundfaltung gut, weicht aber in bestimmten flexiblen Bereichen ab. Die experimentelle Struktur zeigt hier einen konkreten Zustand, während das Modell eine Vorhersage aus einer bestimmten Eingabe ist.

## Hinweise zur Verwendung

Für den normalen Unterricht reichen Trp-cage und Ubiquitin. Calmodulin ist ein Erweiterungsbeispiel für fortgeschrittene Gruppen.

Das Tool sollte nicht als „AlphaFold-Test“ verstanden werden, sondern als Training im wissenschaftlichen Modellverständnis.

