# Kapitel 3: App-Entwicklung in der Freistunde (Der Gleichungstrainer)

Haben Sie sich schon einmal gedacht: *"Eigentlich bräuchte ich für dieses Thema genau jetzt eine kleine, maßgeschneiderte Übungs-App für meine Klasse"*? 

Genau aus diesem Gedanken heraus ist der **Gleichungstrainer PRO** entstanden – und zwar buchstäblich in einer einzigen Freistunde (in unter 60 Minuten)! 

In diesem Kapitel werfen wir einen Blick hinter die Kulissen ("Making-of") und zeigen, wie Sie mit KI-Unterstützung (wie Gemini oder ChatGPT) vom reinen Konsumenten zum Architekten Ihrer eigenen, passgenauen Lernumgebung werden.

[Zum Gleichungstrainer PRO](https://ekerzendorfer.github.io/REAKTIONSTRAINER/){ .md-button .md-button--primary }

---

## 🚀 Der 3-Schritte-Workflow: Vom Foto zur Web-App

Der Weg von einer analogen Idee zu einem weltweit abrufbaren, digitalen Werkzeug erfordert heute keine Programmierkenntnisse mehr, sondern nur noch didaktische Führung.

### Schritt 1: Die Daten-Extraktion (KI als Schreibkraft)
**Die Ausgangslage:** Den Anstoß gab ein zufällig im Internet gefundenes Foto (ein Scan) mit 110 handschriftlichen chemischen Reaktionsgleichungen. 
Statt diese mühsam abzutippen, übernimmt die KI die Fleißarbeit.

!!! abstract "Der initiale Prompt an die KI"
    *"Kannst du die Reaktionsgleichungen auf diesem Bild auslesen und daraus eine kleine Web-App zum Ausgleichen von Reaktionsgleichungen machen? Dafür müssten die Koeffizienten entfernt und in der App durch Eingabefelder ersetzt werden. Die Formeln müssten mit korrekten, tiefgestellten Indizes dargestellt werden. Ideal wäre es, wenn die Reaktionsgleichungen gleich in ein editierbares JSON-File ausgelagert werden, wo auch der Schwierigkeitsgrad (SEK1 und SEK2) eingetragen werden kann. Natürlich muss auch für jede Gleichung die Lösung (richtige Koeffizienten) abgelegt sein. Die Gleichungen sollten in der App in einem zufälligen Mix aufgerufen werden."*

**Das Ergebnis:** Die KI extrahierte die Daten in Sekunden in einen strukturierten, digitalen Wissensschatz (eine sogenannte JSON-Datei) und lieferte das erste HTML-Grundgerüst für die App.

### Schritt 2: Co-Creation (Didaktik trifft Code)
In dieser Phase arbeiten Lehrkraft und KI iterativ zusammen. Der Lehrer liefert die fachdidaktischen Anforderungen, die KI schreibt den Code (HTML5 & modernes Tailwind CSS).

Wir haben die App durch gezielte Folge-Prompts im Chat didaktisch verfeinert:
* **Differenzierung:** Einbau von Auswahlschaltflächen (SEK1, SEK2, ALLE) zur Schnellumschaltung der Schwierigkeitsgrade.
* **Scaffolding:** Sofortiges visuelles Feedback (falsche Felder werden rot, richtige grün eingerahmt). Nach erfolgreichem Lösen wird die Gleichung zusätzlich in kompakter Fachschreibweise eingeblendet.
* **Motivation:** Ein integrierter "Sofort-Richtig-Zähler" (Score), der die SchülerInnen anspornt, genau zu überlegen, bevor sie prüfen.

### Schritt 3: Deployment (In 2 Minuten online)
Die fertigen Dateien (`index.html` und `equations.json`) wurden einfach in ein kostenloses GitHub-Repository hochgeladen. Mit der Aktivierung von "GitHub Pages" war die App sofort und werbefrei über einen Link (oder QR-Code) weltweit erreichbar – und funktioniert einmal geladen sogar komplett offline im Chemiesaal!

---

## 🛠️ Der Lehrer-Bonus: Das integrierte Admin-Panel

Das größte Problem vieler Apps: Sie sind starr. Wenn eine bestimmte Gleichung zu schwer ist oder eine neue ergänzt werden soll, stößt man als Lehrkraft an Grenzen.

Um das zu lösen, haben wir die KI gebeten, ein kleines **Content-Management-System (CMS)** mitzuliefern.

!!! tip "Die `admin.html`"
    Neben der eigentlichen App für die SchülerInnen gibt es im Hintergrund eine Datei für Lehrkräfte (`admin.html`). Ruft man diese auf, öffnet sich ein tabellarischer Editor im Browser. 
    Dort können KollegInnen ohne eine einzige Zeile Code zu berühren:
    
    * Den Schwierigkeitsgrad einzelner Gleichungen anpassen.
    * Gleichungen über ein einfaches Häkchen ("selected") für die Klasse ein- oder ausblenden.
    * Die Bezeichnungen (z. B. "Knallgasprobe") abändern.
    * Eigene, völlig neue Gleichungen unten an die Liste anfügen.
    
    Ein Klick auf "Exportieren" generiert die neue Datenbank, die man einfach wieder hochlädt.

## 👨‍🏫 Fazit: Die neue Lehrerrolle
Dieses Projekt zeigt eindrucksvoll: Wir müssen keine Programmierer sein, aber wir sind die **Architekten unserer Lernumgebungen**. Die KI senkt die technische Hürde gegen Null, sodass Ihre didaktischen Ideen in der Freistunde Realität werden können!
