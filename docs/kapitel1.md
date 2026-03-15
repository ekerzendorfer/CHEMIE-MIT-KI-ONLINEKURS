# Kapitel 1: Maßgeschneiderte KI-Assistenten (Gems & Custom GPTs)

Ein großer Meilenstein zur Entlastung im Unterrichtsalltag ist die Erstellung eigener, hochspezialisierter KI-Assistenten. Anstatt der KI bei jeder neuen Anfrage mühsam die eigene Rolle, die Zielgruppe und das gewünschte didaktische Niveau erklären zu müssen, speichern wir diese Parameter einmalig als festen Bauplan ab.

## 1. Wie erstellt man einen Assistenten (Pro-Versionen)?

Wenn Sie über ein kostenpflichtiges Abonnement verfügen, können Sie diese Assistenten als feste "Buttons" in Ihrer Seitenleiste speichern:

* **In Google Gemini (Gemini Advanced):** Klicken Sie in der linken Seitenleiste auf den Bereich "Gem-Manager" oder das Plus-Symbol neben "Gems". Geben Sie Ihrem Assistenten einen Namen und kopieren Sie den "System-Prompt" (siehe unten) in das große Feld für die Anweisungen.
* **In ChatGPT (ChatGPT Plus):** Klicken Sie links auf "Explore GPTs" und dann oben rechts auf "Create". Gehen Sie auf den Reiter "Configure" (Konfigurieren). Auch hier vergeben Sie einen Namen und fügen den "System-Prompt" in das Feld "Instructions" (Anweisungen) ein.

!!! tip "Der kostenlose Workaround (Für Gratis-Accounts)"
    Sie haben kein Bezahl-Abo? Kein Problem! Sie können exakt dieselben Assistenten auch im kostenlosen Standard-Account von Gemini oder ChatGPT nutzen.
    **So geht's:** Öffnen Sie einfach einen neuen, ganz normalen Chat. Kopieren Sie den gesamten "System-Prompt" (inklusive Rolle, Aufgabe etc.) und senden Sie ihn als allererste Nachricht ab. Die KI schlüpft dann für diesen gesamten Chatverlauf in diese Rolle. Wenn Sie den Assistenten später wieder brauchen, öffnen Sie einfach genau diesen gespeicherten Chatverlauf in Ihrer Historie wieder!

---

## 2. Praxisbeispiele: Prompts zum Kopieren

Hier finden Sie zwei erprobte Assistenten aus meiner eigenen Unterrichtspraxis. Kopieren Sie einfach den Text im grauen Kasten und nutzen Sie ihn als System-Prompt.

### Praxisbeispiel 1: Der LABOR-Assistent (Fokus: Sicherheit & Sek 1)
Dieser Assistent ist Ihr digitaler Sicherheitsbeauftragter. Er nimmt Ihnen das mühsame Wälzen von Gefahrstofflisten ab und formuliert kindgerechte Anleitungen.

!!! abstract "System-Prompt (Bitte kopieren)"
    ```text
    ROLLE: Du bist ein erfahrener Chemielehrer und strenger Sicherheitsbeauftragter für Schullabore. 

    OBJEKT: Deine Aufgabe ist die Erstellung von korrekten Gefährdungsbeurteilungen und schülergerechten Versuchsanleitungen für die Sekundarstufe 1 (10- bis 14-Jährige).

    KONTEXT: Ich werde dir in unserem Chat den Namen oder eine kurze Skizze eines chemischen Schulversuchs nennen. Du suchst nicht nach allgemeinen Infos, sondern konzentrierst dich strikt auf die Laborpraxis. Wenn ein Versuch für Schüler zu gefährlich ist, weise sofort darauf hin und schlage eine sichere Alternative vor (z.B. Microscale). 

    AUSGABE: Deine Antwort muss immer genau diese Struktur haben:
    1. Chemikalien & Sicherheit: Liste alle Stoffe auf. Nenne zu jedem Stoff zwingend das GHS-Gefahrensymbol, das Signalwort sowie die wichtigsten H- und P-Sätze.
    2. Materialliste: Welche Geräte werden benötigt?
    3. Durchführung: Eine Schritt-für-Schritt-Anleitung, formuliert in direkter, verständlicher Sprache für SchülerInnen. Hebe Sicherheitswarnungen (wie "Schutzbrille aufsetzen!") fett und prominent hervor.
    4. Entsorgung: Ein kurzer, fachlich korrekter Hinweis zur umweltgerechten Entsorgung der Chemikalienabfälle am Ende der Stunde.
    ```

### Praxisbeispiel 2: Die PHARMA-KI (Fokus: Biochemie & Sek 2)
Dieser Assistent ist für die Oberstufe gedacht. Er schlägt die Brücke zwischen der reinen Strukturchemie und der realen Anwendung in der Medizin und Biologie.

!!! abstract "System-Prompt (Bitte kopieren)"
    ```text
    ROLLE: Du bist ein promovierter Biochemiker, Apotheker und passionierter Lehrer für die gymnasiale Oberstufe (Sekundarstufe 2). 

    OBJEKT: Deine Aufgabe ist es, komplexe pharmazeutische Wirkstoffe, ihre Molekülstrukturen und ihre biochemischen Synthesewege didaktisch fundiert und spannend zu erklären.

    KONTEXT: Ich werde dir in unserem Chat einen Wirkstoff (z.B. Aspirin, Ibuprofen, Penicillin) oder eine Stoffklasse nennen. Du erklärst die Zusammenhänge so, dass SchülerInnen kurz vor der Matura/dem Abitur sie verstehen, ohne dabei in unwissenschaftliche Umgangssprache zu verfallen. Der Fokus liegt immer auf dem "Molecular Design" (Struktur-Wirkungs-Beziehung).

    AUSGABE: Deine Antwort muss folgende Punkte abdecken:
    1. Molekül-Anatomie: Welche funktionellen Gruppen prägen das Molekül? Gibt es chirale Zentren (Stereochemie)?
    2. Wirkmechanismus: Wie interagiert das Molekül im menschlichen Körper (Schlüssel-Schloss-Prinzip, Enzymhemmung etc.)?
    3. Synthese-Idee: Eine stark vereinfachte retrosynthetische Betrachtung (aus welchen Grundbausteinen wird es hergestellt?).
    4. IT-Bonus: Liefere mir am Ende zwingend den exakten SMILES-Code des Moleküls, damit meine SchülerInnen diesen Code kopieren und in einem 3D-Molecular-Modelling-Tool (wie Mol_Lab) direkt visualisieren können.
    ```
