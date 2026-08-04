# Datenexport und Weiterverarbeitung

## Warum Rohdaten exportieren?

Die App ist ein virtuelles Messgerät, keine vollständige Statistiksoftware. Die Exporte ermöglichen:

- Auswertung in einer Tabellenkalkulation,
- Übergabe an `MESSWERT_LAB`,
- Erstellung eigener Diagramme,
- Dokumentation im Laborprotokoll,
- Vergleich mehrerer SchülerInnengruppen.

## Einheitliche Dateinamen

Die Dateien verwenden das Präfix `PHOT`, den Versuchstyp, eine Stoff- oder Versuchserkennung und einen Zeitstempel.

Beispiele:

```text
PHOT_EICHUNG_PERMANGANAT_20260804_102300.csv
PHOT_KINETIK_KRISTALLVIOLETT_20260804_102500.csv
PHOT_AUFGABE_KI_CV_01_20260804_102700.md
```

## CSV-Aufbau

Je nach Modul unterscheiden sich die Spalten. Ein zusätzlicher Metadatenblock enthält unter anderem:

- App-Version,
- Exportzeit,
- Versuchstyp,
- Stoff oder Reaktionssystem,
- Messwellenlänge,
- Schichtdicke,
- Betriebsart,
- Versuchskennung,
- Aufgabenkennung.

<!-- ABBILDUNG EX-01 | DATEI: ../assets/images/analytik/photometer/ex01_csv_metadaten.webp | MOTIV: Ausschnitt einer exportierten CSV in Texteditor oder Tabellenansicht; Rohdaten und Metadatenblock sichtbar | ALT: Aufbau einer CSV-Datei mit photometrischen Rohdaten und Metadaten | PRIORITÄT: B | EINFÜGEN ALS: ![CSV-Rohdaten und Metadaten](../assets/images/analytik/photometer/ex01_csv_metadaten.webp){ loading=lazy } -->

## Dezimal- und Trennzeichen

Die CSV-Ausgabe ist für deutschsprachige Tabellenprogramme vorbereitet:

- Semikolon als Feldtrenner,
- Dezimalkomma,
- UTF-8-Zeichencodierung.

Beim Import in andere Programme müssen Trennzeichen und Dezimalformat gegebenenfalls bestätigt werden.

## Exporte der einzelnen Bereiche

### Spektrum

- Wellenlänge,
- Absorbanz,
- Stoff,
- Konzentration,
- Schichtdicke.

### Eichkurve

- Standard oder unbekannte Probe,
- Konzentration der Standards,
- Wiederholungsnummer,
- Absorbanz,
- sichtbarer Laborhinweis,
- Zeitstempel.

### Gleichgewicht

- pH-Wert,
- Wellenlänge,
- Absorbanz,
- modellierte Speziesanteile,
- Bedingungen.

### Kinetik

- Zeit,
- Absorbanz,
- Reaktionsbedingungen,
- Messintervall,
- gegebenenfalls Schwelleninformation.

## Markdown-Exporte

Der Aufgabenmodus kann erzeugen:

- Aufgabenblatt,
- Messübersicht.

Markdown lässt sich direkt in Kursseiten, Notizen oder ein digitales Laborjournal übernehmen.

## Weiterverarbeitung mit MESSWERT_LAB

`MESSWERT_LAB` ist als eigenständige browserbasierte Auswertungsapp vorgesehen. Geplant sind:

- CSV-Import,
- Mittelwert und Standardabweichung,
- Regression und Eichkurve,
- unbekannte Konzentration,
- Residuen,
- kinetische Linearisierungen.

<!-- ABBILDUNG EX-02 | DATEI: ../assets/images/analytik/photometer/ex02_photometer_messwertlab.svg | MOTIV: selbst erstelltes Schema SpektralLab → CSV/JSON → MESSWERT_LAB → Diagramm/Statistik → Protokoll | ALT: Geplanter Datenfluss vom virtuellen Photometer zur browserbasierten Messwertauswertung | PRIORITÄT: C | EINFÜGEN ALS: ![Datenfluss zu MESSWERT_LAB](../assets/images/analytik/photometer/ex02_photometer_messwertlab.svg) -->

Bis zur Fertigstellung kann eine Tabellenkalkulation verwendet werden.

## Datenschutz

Die Berechnung erfolgt lokal im Browser. Exportdateien werden auf dem Gerät gespeichert. Es werden keine Messdaten an einen Server übertragen.
