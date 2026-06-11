# MOL_LAB DIDACTIC

**MOL_LAB DIDACTIC** ist ein digitales Moleküllabor für den Chemieunterricht. Es hilft dabei, Molekülstrukturen nicht nur zu betrachten, sondern daraus begründete Aussagen zu Stoffeigenschaften und Reaktivität abzuleiten.

Im Mittelpunkt stehen kleine und mittelgroße Moleküle, die im Unterricht gut erklärbar sind. Das Tool ist bewusst reduziert und didaktisch geführt. Es soll keine Moleküldatenbank ersetzen, sondern beim chemischen Denken unterstützen.

!!! note "Leitidee"
Aus dem Bauplan eines Moleküls lassen sich viele Stoffeigenschaften verstehen: Polarität, Löslichkeit, Wechselwirkungen, Isomerie, Konformation und Reaktivität.

---

## Was kann MOL_LAB DIDACTIC?

MOL_LAB DIDACTIC unterstützt unter anderem:

* Darstellung von Molekülen als 2D-Struktur und 3D-Modell
* Vergleich ausgewählter Molekülpaare
* didaktische Polaritätsoberflächen
* qualitative Einschätzungen zu Polarität und Wasserlöslichkeit
* Hinweise zu funktionellen Gruppen
* qualitative Reaktivitäts-Hinweise
* Konformer-Vergleiche
* Stoffdaten bei ausgewählten Vergleichsbeispielen
* einen einfachen Schüler:innen-Protokolltext

Die Beispiele sind kuratiert. Das bedeutet: Sie wurden nicht ausgewählt, weil sie möglichst exotisch sind, sondern weil sie typische chemische Einsichten ermöglichen.

---

## Start in Google Colab

MOL_LAB DIDACTIC läuft als Google-Colab-Notebook.

### Schritt 1: Notebook öffnen

Öffne das Notebook über den bereitgestellten Colab-Link.

!!! tip "Hinweis"
Wenn du nicht mit deinem Google-Konto angemeldet bist, kannst du das Notebook trotzdem meist öffnen und ausführen. Für dauerhaftes Speichern eigener Kopien ist eine Anmeldung sinnvoll.

### Schritt 2: Alle Zellen ausführen

Nach dem Öffnen:

```text
Laufzeit → Alle ausführen
```

oder je nach Oberfläche:

```text
Runtime → Run all
```

Beim ersten Start werden die benötigten Pakete geladen. Das kann einen Moment dauern.

### Schritt 3: Warten, bis die Benutzeroberfläche erscheint

Am Ende des Notebooks erscheint die Bedienoberfläche von MOL_LAB DIDACTIC. Erst dann beginnt die eigentliche Arbeit mit den Molekülen.

!!! warning "Wenn etwas nicht sofort funktioniert"
In Google Colab kann es gelegentlich zu Problemen mit der 3D-Anzeige kommen. Häufig hilft es, das Notebook erneut mit „Alle ausführen“ zu starten.

---

## Aufbau der Oberfläche

Die Oberfläche besteht aus mehreren Bereichen.

### Modulauswahl

Zuerst wird ein Modul gewählt, zum Beispiel:

* Polarität und Löslichkeit
* Isomerie
* Funktionelle Gruppen
* Konformere
* Wirkstoffe und Biomoleküle

Jedes Modul verfolgt eine andere chemische Leitfrage.

### Molekül- oder Vergleichsauswahl

Je nach Modul wird entweder ein einzelnes Molekül oder ein Molekülpaar ausgewählt.

Einzelmoleküle eignen sich besonders, um funktionelle Gruppen, Polarität oder Reaktivität zu untersuchen.

Vergleichspaare sind besonders wichtig, wenn Unterschiede erklärt werden sollen, etwa bei:

* Ethanol vs. 1-Hexanol
* Ethanol vs. Dimethylether
* Maleinsäure vs. Fumarsäure
* Butan vs. Isobutan

!!! note "Warum Vergleichspaare?"
Viele chemische Zusammenhänge werden erst im Vergleich klar. Eine einzelne Struktur zeigt etwas. Zwei sinnvoll gewählte Strukturen erklären etwas.

---

## 2D-Struktur und 3D-Modell

MOL_LAB DIDACTIC zeigt Moleküle in zwei Formen:

### 2D-Struktur

Die 2D-Struktur hilft beim Erkennen von:

* funktionellen Gruppen
* Bindungsverknüpfungen
* Summenformel und Strukturformel
* Isomerie
* polaren Bindungen

### 3D-Modell

Das 3D-Modell zeigt die räumliche Gestalt des Moleküls. Es kann gedreht und betrachtet werden.

Wichtig ist dabei:

> Moleküle sind keine flachen Zeichnungen. Ihre räumliche Form beeinflusst Eigenschaften und Wechselwirkungen.

Typische Fragen an das 3D-Modell:

* Ist das Molekül eher kompakt oder langgestreckt?
* Gibt es polare und unpolare Bereiche?
* Sind funktionelle Gruppen räumlich gut zugänglich?
* Können Moleküle Wasserstoffbrücken ausbilden?
* Gibt es auffällige Unterschiede zwischen Isomeren?

---

## Didaktische Polaritätsoberfläche

Ein wichtiger Bestandteil ist die **didaktische Polaritätsoberfläche**.

Sie soll sichtbar machen, welche Bereiche eines Moleküls eher polar oder eher unpolar sind. Diese Darstellung ist bewusst vereinfacht und dient der Orientierung.

Sie ist besonders hilfreich bei Fragen wie:

* Warum ist Ethanol gut wasserlöslich?
* Warum ist 1-Hexanol deutlich schlechter wasserlöslich?
* Warum reicht ein einzelnes Sauerstoffatom nicht immer für gute Wasserlöslichkeit?
* Warum sind große unpolare Molekülteile für die Löslichkeit wichtig?

!!! warning "Modellgrenze"
Die Polaritätsoberfläche ist eine didaktische Näherung. Sie ersetzt keine quantenchemisch berechnete elektrostatische Potentialoberfläche. Für den Unterricht ist sie aber oft hilfreicher, weil sie die zentrale Idee klarer sichtbar macht.

---

## Wichtige Modellwerte

MOL_LAB DIDACTIC zeigt einige berechnete Kennwerte. Sie sind keine fertige Antwort, sondern Hinweise, die gedeutet werden müssen.

### logP

Der logP-Wert beschreibt vereinfacht, ob ein Molekül eher wasserliebend oder fettliebend ist.

* niedriger logP: eher wasserliebend
* höherer logP: eher fettliebend / unpolar

!!! tip "Merksatz"
Je größer logP, desto stärker dominiert meist der unpolare Charakter.

### TPSA

TPSA steht für „Topological Polar Surface Area“, also die polare Oberfläche eines Moleküls.

* größere TPSA: mehr polare Oberfläche
* kleinere TPSA: weniger polare Oberfläche

TPSA ist besonders hilfreich, wenn Moleküle viele Sauerstoff- oder Stickstoffatome enthalten.

### H-Brücken-Donoren und -Akzeptoren

Moleküle können Wasserstoffbrücken bilden, wenn passende Gruppen vorhanden sind.

* Donoren können ein H-Atom für eine Wasserstoffbrücke bereitstellen.
* Akzeptoren können eine Wasserstoffbrücke aufnehmen.

Beispiele:

* Alkohole können meist Donor und Akzeptor sein.
* Ether können meist nur Akzeptor sein.
* Carbonylgruppen können Wasserstoffbrücken aufnehmen, aber keine spenden.

---

## Qualitative Einschätzungen

Neben Zahlenwerten zeigt MOL_LAB DIDACTIC auch qualitative Einschätzungen, etwa:

* didaktischer Polaritätseindruck
* Wasserlöslichkeits-Tendenz
* kurze Begründung

Diese Einschätzungen sind besonders wichtig, weil Schüler:innen lernen sollen, aus mehreren Informationen eine begründete Aussage zu bilden.

Beispiel:

> Ethanol ist gut wasserlöslich, weil die OH-Gruppe Wasserstoffbrücken ermöglicht und der unpolare Molekülteil noch klein ist.

Bei 1-Hexanol ist die OH-Gruppe ebenfalls vorhanden. Trotzdem ist die Wasserlöslichkeit deutlich geringer, weil der lange unpolare Kohlenwasserstoffrest stärker ins Gewicht fällt.

---

## Vermutungsfrage und Antwort prüfen

Zu vielen Beispielen gibt es eine kurze Multiple-Choice-Frage. Sie steht unter dem Abschnitt **„Vermute“**.

Diese Frage soll keine Prüfung im engeren Sinn sein. Sie dient dazu, eine typische Fehlvorstellung sichtbar zu machen.

Vorgehen:

1. Struktur und 3D-Modell betrachten.
2. Erste Vermutung formulieren.
3. Antwort auswählen.
4. „Antwort prüfen“ anklicken.
5. Rückmeldung lesen.
6. Erklärung anzeigen und mit der eigenen Vermutung vergleichen.

!!! tip "Für den Unterricht"
Besonders wertvoll ist nicht nur die richtige Antwort, sondern die Frage: Warum wirken die falschen Antworten auf den ersten Blick plausibel?

---

## Reaktivitäts-Hinweise

Bei ausgewählten Molekülen gibt es einen qualitativen Reaktivitäts-Hinweis.

Er besteht aus drei Teilen:

1. **Hinweis**
   Welche Art von Reaktivität ist zu erwarten?

2. **Warum?**
   Welche funktionelle Gruppe oder Struktur erklärt diese Reaktivität?

3. **Reaktionsidee**
   Welche typische Reaktion könnte daran anschließen?

Beispiel:

> Aldehyde reagieren leichter mit bestimmten Reaktionspartnern als Alkane, weil die Carbonylgruppe ein partiell positiviertes Kohlenstoffatom besitzt. Dadurch sind nucleophile Additionen möglich.

!!! warning "Kein Reaktivitätsindex"
MOL_LAB DIDACTIC verwendet bewusst keinen allgemeinen Zahlenwert für „Reaktivität“. Reaktivität hängt immer vom Reaktionspartner, den Bedingungen und dem Reaktionstyp ab.

---

## Stoffdaten und experimenteller Bezug

Bei ausgewählten Molekülvergleichen und Isomeren werden Stoffdaten oder experimentelle Hinweise angezeigt.

Sie sollen nicht auswendig gelernt werden, sondern helfen, die Struktur–Eigenschafts-Beziehung zu verstehen.

Beispiele:

* Warum ist Methan gasförmig, Hexan aber flüssig?
* Warum unterscheiden sich Ethanol und Dimethylether so stark?
* Warum haben Maleinsäure und Fumarsäure unterschiedliche Eigenschaften?
* Warum nimmt die Wasserlöslichkeit innerhalb einer Stoffklasse ab?

!!! note "Wichtig"
Stoffdaten sind im Tool dort besonders sinnvoll, wo sie den Vergleich stützen. Es geht nicht um eine vollständige Datenbank.

---

## Konformere

Im Modul **Konformere** geht es um die Beweglichkeit von Molekülen.

Viele Moleküle besitzen nicht nur eine einzige räumliche Form. Durch Drehungen um Einfachbindungen können verschiedene Anordnungen entstehen.

Typische Fragen:

* Welche Konformation ist besonders günstig?
* Welche Anordnung ist energiereicher?
* Welche Gruppen kommen sich räumlich nahe?
* Wie beeinflusst die Beweglichkeit die Molekülgestalt?

Beispiele im Tool sind unter anderem:

* Butan
* 1,2-Dichlorethan
* Ethylenglykol
* Cyclohexan
* Milchsäure
* n-Pentan
* 2-Butanol

!!! warning "Modellgrenze"
Das Tool zeigt berechnete, stabile Konformere. Energiewerte und Strukturen sind Näherungen. Für den Unterricht sind sie als Vergleich und Denkmodell gedacht.

---

## Schüler:innen-Protokolltext

MOL_LAB DIDACTIC kann einen einfachen Protokolltext erzeugen.

Dieser enthält etwa:

* Molekül oder Vergleich
* Leitfrage
* wichtige Strukturmerkmale
* Polaritätseindruck
* Wasserlöslichkeits-Tendenz
* Mini-Aufgaben
* experimenteller Bezug
* Reaktivitäts-Hinweis

Der Text kann kopiert und weiterverwendet werden.

Er ersetzt kein vollständiges Arbeitsblatt, sondern dient als strukturierte Grundlage für:

* Heftnotizen
* kurze Protokolle
* Gruppenarbeiten
* Ergebnissicherung
* Unterrichtsgespräche

---

## Empfohlene Arbeitsweise

Für Schüler:innen empfiehlt sich dieser Ablauf:

1. **Nicht sofort auf die Erklärung klicken.**
2. Zuerst die Struktur betrachten.
3. Polare und unpolare Bereiche suchen.
4. Funktionelle Gruppen benennen.
5. Eine Vermutung formulieren.
6. Erst dann Antwort prüfen und Erklärung anzeigen.
7. Den Protokolltext nutzen, um die Ergebnisse zusammenzufassen.

!!! tip "Arbeitsauftrag"
Versuche immer einen Satz dieser Form zu formulieren:
„Dieses Molekül ist ... , weil seine Struktur ... enthält.“

Beispiele:

* „Ethanol ist gut wasserlöslich, weil die OH-Gruppe Wasserstoffbrücken ermöglicht und der unpolare Rest klein ist.“
* „1-Hexanol ist schlechter wasserlöslich, weil der lange unpolare Kohlenwasserstoffrest die OH-Gruppe teilweise überlagert.“
* „Ethanol und Dimethylether haben dieselbe Summenformel, aber unterschiedliche funktionelle Gruppen.“

---

## Grenzen des Tools

MOL_LAB DIDACTIC arbeitet mit vereinfachten Modellen. Das ist im Unterricht erwünscht, solange die Grenzen klar bleiben.

Wichtige Grenzen:

* Die 3D-Strukturen sind berechnete Modelle.
* Die Polaritätsoberfläche ist didaktisch vereinfacht.
* Reaktivität wird qualitativ beschrieben, nicht exakt berechnet.
* Lösungsmittel, Temperatur, pH-Wert und Reaktionsbedingungen werden nur vereinfacht berücksichtigt.
* Manche Stoffdaten hängen von Bedingungen und Quellen ab.
* Die 3D-Anzeige kann in Colab gelegentlich instabil sein.

!!! warning "Modellverständnis"
Ein Modell ist nicht falsch, nur weil es vereinfacht. Es ist dann gut, wenn es eine bestimmte Frage verständlich beantwortet und seine Grenzen bekannt sind.

---

## Typische Einsatzmöglichkeiten im Unterricht

MOL_LAB DIDACTIC eignet sich besonders für:

* Einstieg in Struktur–Eigenschafts-Beziehungen
* Wiederholung funktioneller Gruppen
* Vergleich von Isomeren
* Diskussion von Wasserlöslichkeit
* Einführung in Molekülgeometrie
* Erklärung einfacher Reaktivitätsunterschiede
* Arbeit mit digitalen Molekülmodellen
* Schüler:innen-Protokolle und kurze Präsentationen

Das Tool kann in Einzelarbeit, Partnerarbeit, Gruppenarbeit oder im gelenkten Unterrichtsgespräch eingesetzt werden.

---

## Weiter zu den Lernpfaden

Die Bedienung allein reicht nicht aus. Besonders sinnvoll wird MOL_LAB DIDACTIC, wenn es entlang geführter Lernpfade verwendet wird.

[Zu den Lernpfaden](lernpfade.md)
