# Viewer für Strukturdateien

Wenn mit **PDB-, mmCIF- oder Molekül-Dateien** gearbeitet wird, stellt sich schnell die Frage:

**Welcher Viewer ist für Schule und Fortbildung wirklich praktisch?**

Wichtig sind dabei vor allem:

- **browserbasiert**
- **kostenlos**
- **ohne Installation**
- **auch für Kolleg:innen gut bedienbar**

---

## Kurzempfehlung

!!! tip "Empfehlung für die Praxis"
    - **Mol\*** = beste allgemeine Lösung zum **Öffnen und Betrachten lokaler Proteinstrukturen im Browser**
    - **3Dmol.js** = ideal, wenn Strukturen **in eine eigene Website eingebettet** werden sollen
    - **Frog2** = nützlich zur **Erzeugung von 3D-Konformeren kleiner Moleküle**, aber kein didaktisch komfortabler Viewer

---

## 1. Mol\* – der Standardviewer für Proteine

**Mol\*** ist derzeit die beste kostenlose Standardlösung, wenn Kolleg:innen einfach eine **lokale PDB- oder mmCIF-Datei** im Browser öffnen und betrachten möchten.

### Stärken
- läuft direkt im Browser
- keine Installation notwendig
- lokale Dateien können geladen werden
- Proteine, Liganden und Oberflächen werden sehr gut dargestellt
- weit verbreitet, da auch von **RCSB PDB** und **PDBe** verwendet

### Geeignet für
- Proteinstrukturen aus **PDB**
- Ergebnisse aus **ColabFold**
- spätere Betrachtung von Komplexen

### Didaktischer Nutzen
- gut für **Übersichtsdarstellungen**
- geeignet für **Struktur–Funktions-Beziehungen**
- sinnvoll für **SEK II**, aber auch für motivierende Demonstrationen in **SEK I**

**Link:**  
[Mol\* / RCSB 3D Viewer Dokumentation](https://www.rcsb.org/docs/3d-viewers/mol%2A/managing-the-display)

---

## 2. 3Dmol.js – ideal für eigene Webseiten

**3Dmol.js** ist besonders dann stark, wenn man **nicht nur betrachten**, sondern **selbst interaktive Viewer in eine eigene Website einbauen** möchte.

### Stärken
- frei nutzbar
- gut in HTML-Seiten integrierbar
- unterstützt viele Formate
- sehr flexibel für Unterrichtsprojekte

### Geeignet für
- eigene Kursseiten
- interaktive Lernumgebungen
- individuelle Buttons und Workflows
- Vergleich von WT / Mutante / Ligand

### Didaktischer Nutzen
- besonders gut für **maßgeschneiderte Unterrichtstools**
- ideal für deinen Ansatz mit **PROTEINLABOR**

**Link:**  
[3Dmol.js auf GitHub](https://github.com/3dmol/3Dmol.js)

---

## 3. Frog2 – gut für 3D-Konformer, aber nicht als Hauptviewer

**Frog2** ist hilfreich, wenn aus **SMILES oder 2D-Strukturen** eine **3D-Konformation** erzeugt werden soll. Für kleine bis mittlere Moleküle ist das eine interessante kostenlose Browserlösung.

### Stärken
- browserbasiert
- kostenlos
- erzeugt 3D-Konformere
- akzeptiert u. a. SMILES

### Schwächen
- kein wirklich komfortabler didaktischer Viewer
- eher Werkzeug zur **Strukturerzeugung** als zur **Visualisierung**
- für Schule allein meist nicht ausreichend

### Didaktischer Nutzen
- gut als **Vorschritt**
- danach sollte die Datei in einem Viewer wie **Mol\*** betrachtet werden

**Link:**  
[Frog2 Server](https://bioserv.rpbs.univ-paris-diderot.fr/services/Frog2/)

---

## 4. Praktischer Workflow für den Unterricht

### Für Proteine
1. Struktur aus **PDB** oder **ColabFold**
2. in **Mol\*** öffnen
3. drehen, zoomen, Ligand betrachten
4. ggf. Screenshot für Arbeitsblätter erstellen

### Für kleine Moleküle
1. Molekül in **Frog2** als 3D-Struktur erzeugen
2. Datei exportieren
3. in **Mol\*** oder in ein eigenes Tool mit **3Dmol.js** laden

---

## 5. Fazit

Für den naturwissenschaftlichen Unterricht ist derzeit die sinnvollste Kombination:

- **Mol\*** für das schnelle, kostenlose Betrachten von Strukturdateien
- **3Dmol.js** für eigene interaktive Webseiten
- **Frog2** für die 3D-Erzeugung kleiner Moleküle

!!! note "Kurzfassung"
    Wer Kolleg:innen **eine einzige Viewer-Empfehlung** geben möchte, sollte aktuell **Mol\*** nennen.  
    Wer **eigene interaktive Tools** baut, fährt mit **3Dmol.js** am besten.
