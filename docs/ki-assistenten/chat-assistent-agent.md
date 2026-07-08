# KI-Agenten im Chemieunterricht: Chat, Custom GPT/Gem oder Agent?

## Einordnung für Seminar und Kongress

KI-Agenten werden derzeit stark beworben. Für den Chemieunterricht ist aber nicht entscheidend, ob ein Werkzeug technisch als „Agent“ bezeichnet wird, sondern ob es Unterrichtsqualität steigert und Lehrkräfte sinnvoll entlastet.

Die zentrale Leitfrage lautet daher nicht:

> Was ist das neueste KI-Werkzeug?

sondern:

> Welcher Grad an KI-Unterstützung ist für eine konkrete Unterrichtsaufgabe sinnvoll, kontrollierbar und didaktisch verantwortbar?

Die Lehrkraft bleibt in allen Fällen die Instanz, die Ziele auswählt, fachliche Richtigkeit prüft, Unterricht steuert, Sicherheit verantwortet und Lernprozesse pädagogisch begleitet.

---

## Drei Stufen der KI-Nutzung

| Stufe | Kurzbeschreibung | Typischer Nutzen | Grenze |
|---|---|---|---|
| **Normaler Chat** | Die Lehrkraft steuert jeden Schritt über einzelne Prompts. | Schnell, flexibel, ideal für Ideen und erste Entwürfe. | Viel Nachsteuerung nötig. Qualität hängt stark vom Prompting ab. |
| **Custom GPT / Gem** | Rolle, Niveau, Stil, Regeln und Materialbezug werden dauerhaft festgelegt. | Wiederkehrende Aufgaben werden konsistenter und passender. | Arbeitet meist weiterhin dialogisch; Abläufe müssen oft von der Lehrkraft angestoßen werden. |
| **Agentischer Workflow** | Die KI arbeitet eine mehrschrittige Aufgabe mit Planung, Prüfschritten und Ausgabeformat systematisch ab. | Besonders nützlich bei wiederholbaren Arbeitsketten mit Kontrolle, Variantenbildung und Export. | Nur sinnvoll bei klar begrenzten Aufgaben; pädagogische Verantwortung darf nicht abgegeben werden. |

Merksatz:

> **Chat = ich steuere jeden Schritt.**  
> **Custom GPT/Gem = ich speichere Rolle und Regeln.**  
> **Agent = ich delegiere einen begrenzten, wiederkehrenden Arbeitsablauf mit Prüfschritten.**

---

# Beispiel: Elektronegativität und Bindungspolarität

## Gemeinsamer Ausgangsauftrag

> Erstelle Material zum Thema **Elektronegativität und Bindungspolarität** für den Chemieunterricht.

Das Thema eignet sich besonders gut, weil es viele typische Fehlvorstellungen enthält:

- „Unpolare Moleküle haben keine polaren Bindungen.“
- „Je größer die Elektronegativitätsdifferenz, desto polarer ist automatisch das ganze Molekül.“
- „CO₂ ist polar, weil die C=O-Bindungen polar sind.“
- „Wasser ist polar, weil Sauerstoff elektronegativer ist — die Molekülform spielt keine Rolle.“
- „Partialladungen sind echte Ionenladungen.“

---

## Variante 1: Normaler Chat

### Beispielprompt

> Erstelle Unterrichtsmaterial zum Thema Elektronegativität und Bindungspolarität für eine 10. Schulstufe. Es soll eine kurze Erklärung, drei Beispiele und fünf Übungsfragen mit Lösungen enthalten.

### Typisches Ergebnis

#### Kurzinfo für SchülerInnen

Elektronegativität beschreibt, wie stark ein Atom in einer chemischen Bindung die gemeinsamen Bindungselektronen anzieht. Wenn zwei Atome unterschiedliche Elektronegativitäten besitzen, werden die Bindungselektronen stärker zu einem Atom hingezogen. Dadurch entsteht eine **polare Atombindung**.

Das stärker elektronegative Atom erhält eine negative Partialladung δ−, das weniger elektronegative Atom eine positive Partialladung δ+.

Ob ein ganzes Molekül polar ist, hängt aber nicht nur von den Bindungen ab, sondern auch von der **räumlichen Anordnung** der Bindungen.

#### Beispiele

| Molekül | Bindungen | Molekül polar? | Erklärung |
|---|---|---|---|
| HCl | polar | ja | Chlor zieht die Bindungselektronen stärker an. |
| H₂O | polar | ja | Die O–H-Bindungen sind polar und das Molekül ist gewinkelt. |
| CO₂ | polar | nein | Die C=O-Bindungen sind polar, aber das Molekül ist linear und symmetrisch. |

#### Übungsfragen

1. Was versteht man unter Elektronegativität?  
2. Was bedeutet δ−?  
3. Warum ist HCl polar?  
4. Warum ist CO₂ trotz polarer Bindungen unpolar?  
5. Vergleiche H₂O und CO₂ hinsichtlich Bindungspolarität und Molekülpolarität.

#### Lösungen

1. Elektronegativität ist das Maß dafür, wie stark ein Atom Bindungselektronen anzieht.  
2. δ− bedeutet negative Partialladung.  
3. Chlor ist elektronegativer als Wasserstoff und zieht die Elektronen stärker an.  
4. Die beiden polaren C=O-Bindungen sind symmetrisch angeordnet und heben sich in ihrer Wirkung auf.  
5. Beide enthalten polare Bindungen; H₂O ist wegen seiner gewinkelten Form polar, CO₂ wegen seiner linearen Form unpolar.

### Einordnung

Diese Variante ist schnell und brauchbar. Die Lehrkraft bekommt einen ersten Materialentwurf. Allerdings muss sie selbst prüfen:

- Ist das Niveau passend?
- Sind typische Fehlvorstellungen berücksichtigt?
- Gibt es Diagnosefragen?
- Ist Differenzierung vorhanden?
- Sind die Beispiele didaktisch gut gewählt?
- Fehlt ein Experiment oder Modellbezug?

Der normale Chat eignet sich daher sehr gut für **erste Entwürfe, Ideen und schnelle Formulierungshilfen**.

---

## Variante 2: Custom GPT / Gem

Ein Custom GPT oder Gem kann mit festen Vorgaben erstellt werden. Dadurch muss die Lehrkraft nicht jedes Mal alle didaktischen Regeln neu formulieren.

### Beispielhafte Systemvorgaben für einen „Chemie-Unterrichtsassistenten“

> Du bist ein Assistent für Chemieunterricht in der Sekundarstufe I und II.  
> Erstelle Materialien immer fachlich korrekt, altersgemäß und klar strukturiert.  
> Berücksichtige typische Fehlvorstellungen.  
> Unterscheide zwischen Beobachtung, Modell und Deutung.  
> Gib Aufgaben möglichst mit Lösungen und didaktischem Kommentar aus.  
> Verwende österreichische Schulkontexte, wenn passend.  
> Die Lehrkraft bleibt verantwortlich für Auswahl, Anpassung und Prüfung.

### Beispielprompt im Custom GPT/Gem

> Erstelle einen Unterrichtsbaustein zu Elektronegativität und Bindungspolarität für die 10. Schulstufe. Fokus: Unterschied zwischen polarer Bindung und polarem Molekül.

### Typisches Ergebnis

#### Unterrichtsbaustein: Polare Bindung ≠ polares Molekül

**Zielgruppe:** 10. Schulstufe  
**Dauer:** ca. 20–25 Minuten  
**Voraussetzungen:** Atombindung, Molekülform, einfache Strukturformeln

### Lernziel

Die SchülerInnen können erklären, dass eine polare Bindung durch unterschiedliche Elektronegativitäten entsteht, die Polarität eines Moleküls aber zusätzlich von der Molekülgeometrie abhängt.

### Einstieg

Leitfrage:

> CO₂ enthält zwei polare C=O-Bindungen. Warum ist das Molekül trotzdem unpolar?

Kurze Abstimmung:

- CO₂ ist polar.
- CO₂ ist unpolar.
- Ich bin unsicher.

### Erarbeitungsphase

#### Schritt 1: Bindungspolarität

Bei einer polaren Atombindung zieht ein Atom die gemeinsamen Bindungselektronen stärker an. Dadurch entstehen Partialladungen.

Beispiel: H–Cl  
H erhält δ+, Cl erhält δ−.

#### Schritt 2: Molekülpolarität

Für die Polarität eines Moleküls ist entscheidend:

1. Gibt es polare Bindungen?
2. Wie sind diese Bindungen räumlich angeordnet?
3. Heben sich die Bindungspolaritäten auf oder nicht?

### Vergleichsbeispiele

| Molekül | Bindung(en) polar? | Molekülform | Molekül polar? | Didaktischer Kommentar |
|---|---|---|---|---|
| HCl | ja | linear, zweiatomig | ja | Einfachstes Beispiel für Bindungspolarität. |
| H₂O | ja | gewinkelt | ja | Form verhindert Aufhebung der Dipole. |
| CO₂ | ja | linear | nein | Zentrale Fehlvorstellung: polare Bindung bedeutet nicht automatisch polares Molekül. |
| CH₄ | kaum polar | tetraedrisch | nein | Symmetrisches Molekül ohne relevanten Gesamtdipol. |

### Diagnosefrage

> Ein Molekül besitzt zwei polare Bindungen. Muss das Molekül daher polar sein? Begründe mit einem Beispiel.

**Musterantwort:**  
Nein. CO₂ besitzt zwei polare C=O-Bindungen, ist aber linear gebaut. Die Bindungspolaritäten heben sich gegenseitig auf, daher ist das Molekül insgesamt unpolar.

### Typische Fehlvorstellungen

| Fehlvorstellung | Korrekturimpuls |
|---|---|
| „Polare Bindung bedeutet immer polares Molekül.“ | Molekülgeometrie mitberücksichtigen. |
| „Partialladungen sind volle Ionenladungen.“ | δ+ und δ− sind nur Teilladungen. |
| „CO₂ ist polar, weil Sauerstoff elektronegativer ist.“ | Die Bindungen sind polar, das Molekül als Ganzes aber nicht. |

### Einordnung

Diese Variante ist gegenüber dem normalen Chat deutlich konsistenter, weil die didaktischen Regeln bereits hinterlegt sind. Die Lehrkraft bekommt nicht nur Material, sondern ein stärker unterrichtsorientiertes Produkt.

Der Custom GPT/Gem eignet sich besonders gut für **wiederkehrende schulische Aufgaben mit ähnlicher Struktur**, zum Beispiel:

- Molekülsteckbriefe
- Aufgaben mit Lösungen
- Fehlvorstellungsanalysen
- kurze Unterrichtsbausteine
- Protokollfeedback
- Differenzierung

---

## Variante 3: Agentischer Workflow

Ein Agent würde nicht einfach eine Antwort schreiben, sondern einen festgelegten Ablauf abarbeiten. Dieser Ablauf könnte z. B. aus fünf Prüfschritten bestehen.

### Beispielauftrag an einen Agenten

> Erstelle einen geprüften Unterrichtsbaustein zu Elektronegativität und Bindungspolarität für die 10. Schulstufe.  
> Arbeite in folgenden Schritten:  
> 1. Formuliere ein konkretes Lernziel.  
> 2. Identifiziere typische Fehlvorstellungen.  
> 3. Erstelle einen Unterrichtsbaustein mit Einstieg, Erklärung, Beispielen und Übungsaufgaben.  
> 4. Prüfe die fachliche Konsistenz, insbesondere den Unterschied zwischen Bindungspolarität und Molekülpolarität.  
> 5. Erstelle drei Ausgabeformate: Lehrkraft-Kurzfassung, SchülerInnen-Arbeitsblatt und Exit-Ticket.  
> Gib am Ende an, welche Punkte die Lehrkraft unbedingt prüfen oder anpassen sollte.

### Möglicher agentischer Ablauf

#### Schritt 1: Lernziel

Die SchülerInnen können den Unterschied zwischen Bindungspolarität und Molekülpolarität erklären und auf einfache Moleküle wie HCl, H₂O, CO₂ und CH₄ anwenden.

#### Schritt 2: Fehlvorstellungen

Der Agent erkennt als zentrale Stolpersteine:

1. Polare Bindung wird mit polarem Molekül gleichgesetzt.
2. Elektronegativitätsdifferenzen werden nur rechnerisch betrachtet, ohne Molekülgeometrie.
3. Partialladungen werden mit Ionenladungen verwechselt.
4. Symmetrie wird nicht als Kriterium für die Aufhebung von Dipolen genutzt.

#### Schritt 3: Unterrichtsbaustein

**Einstieg:**  
CO₂ und H₂O werden gegenübergestellt. Beide enthalten Bindungen zwischen Atomen unterschiedlicher Elektronegativität. Trotzdem ist H₂O polar, CO₂ aber unpolar.

**Kernidee:**  
Die Polarität eines Moleküls ergibt sich aus zwei Fragen:

1. Sind die Bindungen polar?
2. Ist das Molekül so gebaut, dass sich die Bindungspolaritäten aufheben?

**Beispiele:**

| Molekül | Polare Bindung? | Geometrie | Gesamtdipol? | Ergebnis |
|---|---|---|---|---|
| HCl | ja | linear, zweiatomig | ja | polar |
| H₂O | ja | gewinkelt | ja | polar |
| CO₂ | ja | linear symmetrisch | nein | unpolar |
| CH₄ | praktisch nein / sehr schwach | tetraedrisch symmetrisch | nein | unpolar |
| NH₃ | ja | trigonal-pyramidal | ja | polar |

**Übungsaufgaben:**

1. Markiere in HCl δ+ und δ−.  
2. Erkläre, warum H₂O polar ist.  
3. Erkläre, warum CO₂ kein permanenter Dipol ist.  
4. Vergleiche CO₂ und NH₃.  
5. Formuliere eine Regel: Wann kann ein Molekül trotz polarer Bindungen unpolar sein?

#### Schritt 4: Selbstprüfung des Materials

Der Agent prüft:

- Wird Bindungspolarität klar von Molekülpolarität getrennt? → ja
- Wird die Molekülgeometrie einbezogen? → ja
- Wird CO₂ korrekt erklärt? → ja
- Werden Partialladungen nicht als Ionenladungen dargestellt? → ja
- Sind Beispiele für symmetrische und unsymmetrische Moleküle vorhanden? → ja

#### Schritt 5: Drei Ausgabeformate

### A. Lehrkraft-Kurzfassung

**Kernbotschaft:**  
Eine polare Bindung entsteht durch unterschiedliche Elektronegativität. Ein Molekül ist aber nur dann polar, wenn sich die einzelnen Bindungspolaritäten räumlich nicht aufheben.

**Didaktischer Fokus:**  
Der Gegensatz H₂O/CO₂ ist zentral. Beide Moleküle enthalten polare Bindungen; nur H₂O ist aufgrund seiner gewinkelten Struktur ein Dipol.

**Typische Fehlvorstellung:**  
„CO₂ ist polar, weil die C=O-Bindungen polar sind.“

### B. SchülerInnen-Arbeitsblatt

#### Polare Bindung und polares Molekül

Elektronegativität gibt an, wie stark ein Atom Bindungselektronen anzieht. Wenn zwei gebundene Atome unterschiedliche Elektronegativitäten besitzen, entsteht eine polare Bindung.

Das bedeutet aber nicht automatisch, dass das ganze Molekül polar ist. Dafür ist auch die Form des Moleküls wichtig.

**Merke:**  
Ein Molekül ist polar, wenn es polare Bindungen besitzt und diese räumlich so angeordnet sind, dass sie sich nicht gegenseitig aufheben.

| Molekül | Erklärung |
|---|---|
| HCl | Chlor zieht die Elektronen stärker an. Das Molekül ist polar. |
| H₂O | Die O–H-Bindungen sind polar. Das Molekül ist gewinkelt und daher polar. |
| CO₂ | Die C=O-Bindungen sind polar. Das Molekül ist linear, daher heben sich die Bindungspolaritäten auf. |

**Aufgaben:**

1. Erkläre den Begriff Elektronegativität.  
2. Zeichne H–Cl mit δ+ und δ−.  
3. Warum ist H₂O polar?  
4. Warum ist CO₂ trotz polarer Bindungen unpolar?  
5. Formuliere eine allgemeine Regel.

### C. Exit-Ticket

Beantworte am Ende der Stunde in zwei Sätzen:

1. Was ist der Unterschied zwischen einer polaren Bindung und einem polaren Molekül?  
2. Warum ist CO₂ kein Dipolmolekül?

#### Punkte, die die Lehrkraft prüfen/anpassen sollte

- Passen die Molekülbeispiele zum Vorwissen der Klasse?
- Wurde Molekülgeometrie bereits eingeführt?
- Sollen Elektronegativitätswerte angegeben oder bewusst weggelassen werden?
- Ist ein Modellbaukasten, eine 3D-Darstellung oder ein digitales Moleküllabor verfügbar?
- Soll das Niveau stärker in Richtung SEK I oder SEK II angepasst werden?

### Einordnung

Der agentische Workflow liefert nicht nur ein Ergebnis, sondern ein Paket aus mehreren abgestimmten Produkten. Der Unterschied liegt nicht in einer völlig anderen „Intelligenz“, sondern in der systematischen Abarbeitung eines Arbeitsprozesses.

Er eignet sich besonders dann, wenn Lehrkräfte immer wieder ähnliche Materialpakete brauchen:

- Unterrichtsbaustein
- Arbeitsblatt
- Lösungen
- Diagnosefrage
- Differenzierung
- Selbstprüfung
- Exportformat

---

# Vergleich der drei Ansätze

| Kriterium | Normaler Chat | Custom GPT / Gem | Agentischer Workflow |
|---|---|---|---|
| Einstiegshürde | sehr niedrig | mittel | höher |
| Qualität bei Einzelaufgaben | gut, aber schwankend | meist konsistenter | gut, wenn Workflow sauber definiert ist |
| Nachsteuerung durch Lehrkraft | hoch | mittel | geringer |
| Wiederholbarkeit | gering bis mittel | hoch | sehr hoch |
| Prüfschritte | müssen extra verlangt werden | können als Regel hinterlegt werden | Teil des Ablaufs |
| Ausgabeformate | müssen einzeln angefordert werden | können vorbereitet sein | können automatisch erzeugt werden |
| Risiko der unkritischen Übernahme | mittel | mittel | höher, wenn zu viel delegiert wird |
| Pädagogische Verantwortung | vollständig bei Lehrkraft | vollständig bei Lehrkraft | muss bewusst bei Lehrkraft bleiben |

---

# Didaktische Schlussfolgerung

Für die meisten schulischen Anwendungen genügt ein guter Chat oder ein sorgfältig gebauter Custom GPT/Gem. Agenten werden erst dann wirklich interessant, wenn wiederkehrende Arbeitsabläufe mit mehreren Prüfschritten automatisiert werden sollen.

Das Ziel ist aber nicht, Unterricht an KI-Systeme abzugeben. Sinnvoll ist KI dort, wo sie Lehrkräfte entlastet und die Unterrichtsqualität verbessert:

- bessere Aufgaben
- gezieltere Differenzierung
- klarere Erklärungen
- mehr Aufmerksamkeit für Fehlvorstellungen
- weniger Routinearbeit

Die Lehrkraft bleibt verantwortlich für:

- Auswahl der Lernziele
- fachliche Prüfung
- didaktische Reduktion
- Steuerung des Unterrichts
- Sicherheitsentscheidungen
- Bewertung von Schülerleistungen
- pädagogische Beziehung

Schlussformel:

> **Nicht KI statt LehrerInnen.**  
> **Sondern bessere Werkzeuge für LehrerInnen.**

