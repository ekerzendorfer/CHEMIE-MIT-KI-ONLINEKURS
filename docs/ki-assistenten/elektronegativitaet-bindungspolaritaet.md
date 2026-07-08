# KI-Agenten im Chemieunterricht  
## Nüchterne Einordnung mit Beispiel „Elektronegativität und Bindungspolarität“

**Zielgruppe:** ChemielehrerInnen, die bereits erste Erfahrungen mit KI-Tools gesammelt haben  
**Ziel:** Das Thema KI-Agenten kurz, verständlich und kritisch einordnen — ohne Hype und ohne technischen Tiefgang.

---

## 1. Grundhaltung

KI-Agenten werden derzeit sehr stark beworben. Für den Chemieunterricht ist aber nicht entscheidend, ob ein Werkzeug neu, komplex oder „agentisch“ ist. Entscheidend ist, ob es **Unterrichtsqualität verbessert**, **Lehrkräfte entlastet** und **pädagogisch kontrollierbar** bleibt.

Der zentrale Maßstab sollte daher lauten:

> **KI darf Lehrkräfte entlasten, aber nicht entmündigen.**  
> **Sie darf Routinearbeit beschleunigen, aber nicht die pädagogische Verantwortung übernehmen.**

Für den Chemieunterricht bedeutet das: KI kann bei Materialentwürfen, Aufgabenvarianten, Differenzierung, Fehlvorstellungsanalyse, Protokollfeedback oder vorbereitenden Experimenten-Checks sehr nützlich sein. Die fachliche Prüfung, die Entscheidung über den Unterrichtsverlauf und die Verantwortung für Sicherheit, Bewertung und Lernsteuerung bleiben aber bei der Lehrkraft.

---

## 2. Chat, Custom GPT/Gem und Agent — einfache Abgrenzung

| Form | Was passiert? | Typischer Nutzen | Grenze |
|---|---|---|---|
| **Normaler Chat** | Die Lehrkraft steuert jeden Schritt durch Prompts. | Schnell, flexibel, ideal für Ideen und Einzelaufgaben. | Viel Nachsteuern nötig; Qualität hängt stark vom Prompt ab. |
| **Custom GPT / Gem** | Rolle, Stil, Regeln und ggf. Wissensmaterial werden gespeichert. | Wiederkehrende Aufgaben werden konsistenter. | Bleibt meist ein Dialogsystem; die Lehrkraft führt den Ablauf. |
| **Agentischer Workflow / Agent** | Ein mehrschrittiger Ablauf wird teilweise delegiert: planen, erzeugen, prüfen, überarbeiten, ggf. Werkzeuge nutzen. | Gut für wiederkehrende Routineabläufe mit Prüfschritten. | Nur sinnvoll, wenn der Ablauf klar begrenzt und kontrollierbar ist. |

Kurzform für eine Folie:

> **Chat:** Ich steuere jeden Schritt.  
> **Custom GPT/Gem:** Ich speichere Rolle und Regeln.  
> **Agent:** Ich delegiere einen begrenzten Arbeitsablauf mit Prüfschritten.

---

## 3. Wann Agenten im Chemieunterricht tatsächlich Mehrwert haben

Für viele schulische Anwendungen genügt ein guter Chat oder ein gut konfigurierter Custom GPT/Gem völlig. Agenten werden erst dann interessant, wenn mehrere Bedingungen zusammenkommen:

1. Der Ablauf wiederholt sich häufig.
2. Es gibt mehrere klar unterscheidbare Arbeitsschritte.
3. Zwischenergebnisse sollen geprüft oder verbessert werden.
4. Es sollen mehrere Ausgabeformate entstehen.
5. Die Lehrkraft möchte nicht jeden Zwischenschritt einzeln anstoßen.

Beispiele:

- Aufgabenvarianten erzeugen und rechnerisch prüfen.
- Material in mehreren Niveaustufen erstellen.
- typische Fehlvorstellungen und Diagnosefragen ergänzen.
- Schülerprotokolle nach einem festen Schema coachen.
- Molekülsteckbriefe aus einer Liste erzeugen.
- Experimentideen vorbereitend auf offensichtliche Sicherheits- und Durchführungsprobleme prüfen.

Wichtig: Besonders bei Experimenten, Sicherheit und Leistungsbewertung darf ein Agent nur **vorbereiten**, niemals endgültig entscheiden.

---

## 4. Konkretes Vergleichsbeispiel

### Ausgangsauftrag

> **Erstelle Material zum Thema Elektronegativität und Bindungspolarität.**

Dieses Beispiel eignet sich gut, weil es fachlich überschaubar ist, typische Fehlvorstellungen enthält und sich leicht in drei Stufen demonstrieren lässt.

---

## 5. Variante A: Normaler Chat

### Beispielprompt

```text
Erstelle ein kurzes Unterrichtsmaterial für SEK II zum Thema Elektronegativität und Bindungspolarität. Es soll eine Erklärung, ein Beispiel und drei Aufgaben mit Lösungen enthalten.
```

### Typischer Ablauf

Die KI liefert einen ersten Entwurf. Die Lehrkraft muss danach meist weiter steuern:

```text
Bitte vereinfache die Erklärung.
```

```text
Ergänze typische Fehlvorstellungen.
```

```text
Erstelle noch eine Diagnosefrage.
```

```text
Bitte prüfe, ob die Aufgaben fachlich korrekt sind.
```

### Typisches Ergebnis

Der Chat erzeugt brauchbares Material, aber die Qualität entsteht vor allem durch die Nachsteuerung der Lehrkraft.

**Stärken:**

- schnell und flexibel
- ideal zum Brainstorming
- gut für einzelne Materialien oder Erklärungen

**Grenzen:**

- jeder Zusatzschritt muss erneut angefordert werden
- Format und Tiefe schwanken
- Selbstprüfung und Fehlvorstellungsanalyse fehlen oft, wenn sie nicht ausdrücklich verlangt werden

### Didaktische Einordnung

Für viele Unterrichtsvorbereitungen reicht diese Variante völlig aus. Sie ist besonders geeignet, wenn die Lehrkraft ohnehin aktiv am Material feilt und die KI eher als Ideengeber nutzt.

---

## 6. Variante B: Custom GPT oder Gem

### Grundidee

Ein Custom GPT/Gem bekommt dauerhaft gespeicherte Anweisungen. Dadurch muss die Lehrkraft nicht jedes Mal neu erklären, wie gutes Chemie-Unterrichtsmaterial aufgebaut sein soll.

### Beispiel für gespeicherte Grundanweisungen

```text
Du bist ein Assistent für Chemieunterricht in SEK I und SEK II.
Erstelle Materialien fachlich korrekt, sprachlich klar und didaktisch reduziert.
Berücksichtige immer:
- Zielgruppe und Vorwissen
- Lernziel
- kurze fachliche Erklärung
- typische Fehlvorstellungen
- mindestens eine Diagnosefrage
- Aufgaben mit Lösungen
- Hinweise zur Fachsprache
Gib keine endgültigen Sicherheits- oder Bewertungsentscheidungen aus, sondern formuliere Prüfpunkte für die Lehrkraft.
```

### Dann genügt als Arbeitsauftrag

```text
Erstelle Material zum Thema Elektronegativität und Bindungspolarität für SEK II.
```

### Typisches Ergebnis

Das System liefert automatisch eine strukturiertere Ausgabe, zum Beispiel:

1. Lernziel  
2. fachliche Kurzklärung  
3. typische Fehlvorstellungen  
4. Beispiel H–Cl, C–H, O–H  
5. Diagnosefrage  
6. Aufgaben mit Lösungen  
7. Lehrerhinweise

### Stärken

- wiederkehrender Stil
- weniger Prompt-Arbeit
- bessere Passung zum eigenen Unterrichtskonzept
- gut geeignet für Linkhub, Kursmaterialien oder wiederkehrende Seminaraufgaben

### Grenzen

- arbeitet meist nicht wirklich selbstständig mehrere Prüfschritte ab
- erzeugt zwar strukturierteres Material, verwirft aber nicht automatisch schlechte Varianten
- externe Werkzeuge, Tabellen, Dateien oder mehrstufige Prüfungen müssen meist weiterhin gezielt angestoßen werden

### Didaktische Einordnung

Für den schulischen Alltag ist dies oft der beste Kompromiss: Die Lehrkraft bleibt vollständig steuernd, spart aber wiederkehrende Erklärungen und erhält konsistentere Ergebnisse.

---

## 7. Variante C: Agentischer Workflow

### Grundidee

Ein Agent oder agentischer Workflow bekommt nicht nur eine Rolle, sondern einen Ablauf. Er soll mehrere Schritte nacheinander bearbeiten und dabei Zwischenergebnisse prüfen.

### Beispielauftrag

```text
Erstelle ein Unterrichtspaket zum Thema Elektronegativität und Bindungspolarität für SEK II.
Arbeite in folgenden Schritten:

1. Formuliere ein präzises Lernziel.
2. Erstelle eine kurze fachliche Erklärung.
3. Identifiziere typische Fehlvorstellungen.
4. Erstelle drei Aufgaben in unterschiedlichen Schwierigkeitsgraden.
5. Prüfe die Aufgaben und Lösungen fachlich.
6. Ergänze eine Diagnosefrage und ein Exit Ticket.
7. Überarbeite das Material so, dass es in 15 Minuten einsetzbar ist.
8. Gib am Ende eine kurze Selbstprüfung aus: Was muss die Lehrkraft noch kontrollieren?
```

### Erwarteter agentischer Ablauf

Der Agent arbeitet nicht nur einen einzelnen Prompt ab, sondern folgt einer Kette:

```text
Planen → Entwerfen → Prüfen → Überarbeiten → Strukturieren → Ausgeben
```

Mögliche Zwischenschritte:

- Klärung: Geht es um Bindungspolarität oder Molekülpolarität?
- Prüfung: Stimmen die Beispiele zu den Elektronegativitätsunterschieden?
- Fehlvorstellungen: „unpolare Bindung“ versus „unpolarer Stoff“; Bindungspolarität versus Molekülpolarität.
- Differenzierung: eine einfache, eine mittlere und eine anspruchsvollere Aufgabe.
- Ausgabe: Arbeitsblatt, Lösungsblatt, Diagnosefrage, Lehrerhinweis.

### Typisches Ergebnis

Ein agentischer Workflow könnte automatisch ein kleines Unterrichtspaket liefern:

- kompakte Einführung
- Aufgabenblatt
- Lösungsteil
- Diagnosefrage
- Exit Ticket
- typische Fehlvorstellungen
- Prüfliste für die Lehrkraft

### Stärken

- weniger manuelle Zwischenschritte
- bessere Eignung für Routineaufgaben
- Prüfschritte können verbindlich eingebaut werden
- mehrere Ausgabeprodukte entstehen in einem Durchlauf

### Grenzen

- aufwendiger in der Einrichtung
- nur sinnvoll bei klar begrenzten Abläufen
- fachliche Kontrolle bleibt notwendig
- Gefahr der Scheinautonomie: Ein sauber klingendes Ergebnis kann trotzdem fachlich oder didaktisch problematisch sein

### Didaktische Einordnung

Agenten sind interessant, wenn aus einer Einzelanfrage ein wiederkehrender Produktionsablauf wird. Sie sind aber nicht automatisch „besser“ als ein gut geführter Chat. Ihr Nutzen liegt vor allem in Workflow-Automatisierung, nicht in pädagogischer Urteilskraft.

---

## 8. Die Unterschiede am Beispiel kurz zusammengefasst

| Frage | Chat | Custom GPT/Gem | Agentischer Workflow |
|---|---|---|---|
| Wer steuert den Ablauf? | Lehrkraft Schritt für Schritt | Lehrkraft, aber mit gespeicherten Regeln | Ablauf teilweise delegiert |
| Wie viel Prompt-Arbeit ist nötig? | hoch | mittel | gering, wenn der Ablauf eingerichtet ist |
| Wie konsistent ist das Ergebnis? | schwankend | relativ konsistent | konsistent, wenn Workflow gut definiert ist |
| Gibt es eingebaute Prüfschritte? | nur auf Nachfrage | als Regel möglich | als fester Ablauf möglich |
| Für Chemieunterricht sinnvoll? | ja, sehr oft | ja, besonders alltagstauglich | ja, aber eher für wiederkehrende Workflows |
| Risiko | unstrukturierte Ergebnisse | scheinbare Autorität durch feste Rolle | Scheinautonomie und Kontrollverlust |

---

## 9. Beispiel: Inhaltliche Zielstruktur für das Material

Unabhängig vom Werkzeug sollte das Material zum Thema Elektronegativität und Bindungspolarität einige Kernpunkte enthalten:

### Lernziel

Die SchülerInnen können erklären, dass Bindungspolarität durch unterschiedliche Elektronegativität der Bindungspartner entsteht, und sie können einfache Bindungen anhand der Elektronegativitätsdifferenz begründet vergleichen.

### Fachliche Kernaussage

Elektronegativität beschreibt die Fähigkeit eines Atoms, Bindungselektronen anzuziehen. Wenn zwei Atome in einer kovalenten Bindung unterschiedlich stark an den Bindungselektronen ziehen, entsteht eine polare Atombindung. Das stärker elektronegative Atom trägt eine negative Partialladung, das weniger elektronegative Atom eine positive Partialladung.

### Typische Fehlvorstellungen

- „Eine polare Bindung bedeutet automatisch, dass das ganze Molekül polar ist.“
- „Partialladungen sind echte Ionenladungen.“
- „Elektronegativität ist eine feste Kraft, die unabhängig vom Bindungspartner wirkt.“
- „C–H-Bindungen sind stark polar, weil Wasserstoff besonders ist.“
- „Wenn ein Molekül polare Bindungen enthält, muss es wasserlöslich sein.“

### Diagnosefrage

> CO₂ enthält polare C=O-Bindungen. Warum ist das CO₂-Molekül trotzdem insgesamt unpolar?

### Erwartete Antwort

Die C=O-Bindungen sind polar, aber das Molekül ist linear und symmetrisch. Die Bindungsdipole heben sich daher gegenseitig auf. Deshalb ist das Molekül insgesamt unpolar.

### Exit Ticket

> Erkläre in zwei Sätzen den Unterschied zwischen einer polaren Bindung und einem polaren Molekül.

---

## 10. Empfohlene Position für Seminar und Kongress

Für eine kurze Vorstellung reicht eine nüchterne Botschaft:

> **Für 80 % der schulischen Anwendungen genügt ein guter Chat oder ein gut gebauter Custom GPT/Gem.**  
> **Agenten werden dann interessant, wenn ein Ablauf immer wieder gleich abläuft, mehrere Prüfschritte enthält und am Ende ein strukturiertes Produkt entstehen soll.**

Oder als prägnanter Abschluss:

> **Nicht jeder neue KI-Trend verbessert Unterricht.**  
> **Entscheidend ist nicht, ob ein Werkzeug agentisch ist, sondern ob es Lehrkräfte stärkt, Unterricht verbessert und pädagogische Kontrolle erhält.**

---

## 11. Rote Linien

KI-Agenten sollten im schulischen Kontext nicht eingesetzt werden für:

- autonome Leistungsbewertung
- endgültige Sicherheitsentscheidungen
- verbindliche Gefährdungsbeurteilungen
- personenbezogene Lernprofile ohne klare Datenschutzgrundlage
- vollständige Steuerung individueller Lernwege ohne Lehrkraft
- automatische Auswahl von Unterrichtszielen

Geeignete Einsatzbereiche sind dagegen:

- Materialentwürfe
- Aufgabenvarianten
- Differenzierung
- Fehlvorstellungsanalyse
- Protokoll-Coaching
- vorbereitende Plausibilitätschecks
- Strukturierung von Unterrichtsbausteinen

---

## 12. Schlussbotschaft

KI-Agenten können im Chemieunterricht nützlich sein, wenn sie als begrenzte Assistenzsysteme verstanden werden. Sie sollten Lehrkräfte bei wiederkehrenden und überprüfbaren Arbeitsschritten entlasten. Sie dürfen aber nicht die Unterrichtssteuerung übernehmen.

> **Nicht: KI statt LehrerInnen.**  
> **Sondern: bessere Werkzeuge für LehrerInnen.**

