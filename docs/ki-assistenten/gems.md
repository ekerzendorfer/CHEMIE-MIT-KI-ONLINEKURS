# Exkurs: Eigene KI-Assistenten (Gems) bauen

Stellen Sie sich vor, Sie müssten Ihrer KI nicht jedes Mal aufs Neue erklären, dass Sie eine Chemielehrkraft sind und Material für eine 10. Klasse benötigen. Genau hier kommen sogenannte **Gems** (bei Google Gemini) oder **Custom GPTs** (bei ChatGPT) ins Spiel.

Ein Gem ist ein maßgeschneiderter KI-Assistent, dem Sie einmalig eine feste Rolle, spezielle Anweisungen (den sogenannten "System-Prompt") und ein bestimmtes Antwortverhalten einprogrammieren. Danach steht er Ihnen als dauerhafter Chat-Partner in der Seitenleiste zur Verfügung – auf Knopfdruck bereit.

---

## 🛠️ Wie baut man einen Gem? (In 3 Schritten)

Das Erstellen erfordert keinerlei Programmierkenntnisse. Es ist so einfach wie das Ausfüllen eines kleinen Steckbriefs:

1. **Assistenten-Menü öffnen:** Klicken Sie in Ihrem KI-Tool (z. B. Gemini Advanced oder ChatGPT Plus) auf "Gem-Manager" bzw. "GPTs entdecken" und wählen Sie "Erstellen".
2. **Name & Beschreibung:** Geben Sie Ihrem Assistenten einen passenden Namen (z. B. "Laborassistent") und eine kurze Beschreibung.
3. **Der System-Prompt (Das Herzstück):** In das große Textfeld "Anweisungen" schreiben Sie detailliert auf, wie sich die KI immer verhalten soll. 

Hier sind zwei bewährte Beispiele aus der Praxis, die Sie direkt für sich kopieren können:

---

## 🧪 Praxis-Beispiele für den Chemieunterricht

Klicken Sie auf die Boxen, um die fertigen "System-Prompts" (Anweisungen) für die beiden Assistenten aufzuklappen. Sie können diese Texte einfach kopieren und in das Anweisungsfeld Ihres neuen Gems einfügen.

??? example "Beispiel 1: Der Laborassistent (Sicherheit & Vorbereitung)"
    Dieser Assistent ist ideal für die Vorbereitung von Schülerübungen. Er kennt die GHS-Symbole, Entsorgungsrichtlinien und hilft beim Erstellen der Gefährdungsbeurteilung.
    
    > **System-Prompt (Bitte kopieren):**
    > "Du bist ein hochkompetenter, sicherheitsbewusster Laborassistent für den schulischen Chemieunterricht. Deine Hauptaufgabe ist es, Lehrkräfte bei der Vorbereitung von Experimenten zu unterstützen. 
    > 
    > **Deine Regeln:**
    > 1. Wenn ich dir ein Experiment oder Chemikalien nenne, nennst du mir als Erstes immer die relevanten GHS-Gefahrensymbole, H- und P-Sätze der beteiligten Stoffe.
    > 2. Gib konkrete Hinweise zur sicheren Entsorgung im schulischen Kontext.
    > 3. Weise auf typische Schülerfehler oder Sicherheitsrisiken bei diesem speziellen Versuch hin.
    > 4. Formuliere deine Antworten stets präzise, übersichtlich in Stichpunkten und fachlich absolut korrekt. Sicherheit hat oberste Priorität!"

??? example "Beispiel 2: Die PHARMA-KI (Organische Chemie & Wirkstoffe)"
    Ein fantastisches Tool für Projektwochen oder die Oberstufe. Die SchülerInnen können Medikamente eingeben und die KI bricht die komplexe organische Chemie auf Schulniveau herunter.
    
    > **System-Prompt (Bitte kopieren):**
    > "Du bist ein didaktisch versierter Experte für pharmazeutische Chemie. Deine Aufgabe ist es, komplexe Medikamente und deren Wirkstoffe für SchülerInnen der gymnasialen Oberstufe verständlich zu erklären.
    > 
    > **Deine Regeln:**
    > 1. Wenn ein Medikament oder Wirkstoff (z.B. Aspirin, Ibuprofen) genannt wird, analysierst du zunächst die Molekülstruktur und benennst alle enthaltenen funktionellen Gruppen.
    > 2. Erkläre den chemischen oder biologischen Wirkmechanismus im Körper anhand einer alltagsnahen, für Schüler greifbaren Analogie (z.B. Schlüssel-Schloss-Prinzip).
    > 3. Gehe kurz auf die historische Entdeckung oder Synthese ein.
    > 4. Passe dein Sprachniveau an 16- bis 18-Jährige an: Erkläre komplexe Fachbegriffe in Klammern, aber bleibe chemisch korrekt. Verwende für die Strukturierung Bulletpoints und fettgedruckte Kernbegriffe."

---

## 💡 Tipp für den Unterricht

Sie können diese Assistenten nicht nur für sich selbst nutzen! Bei vielen Plattformen lassen sich selbsterstellte Gems oder GPTs per Link teilen. So können Sie Ihrer Oberstufenklasse für eine Recherche-Hausaufgabe direkt den Link zur "PHARMA-KI" schicken, und die SchülerInnen arbeiten in einer von Ihnen didaktisch vorstrukturierten, sicheren Lernumgebung.

---

## 💡 Keine Pro-Version? So klappt es auch kostenlos!

Die offiziellen "Gems" (bei Gemini Advanced) oder das Erstellen eigener "Custom GPTs" (bei ChatGPT Plus) sind an kostenpflichtige Abonnements gebunden. Doch für den Schulalltag gibt es hervorragende, kostenlose Alternativen, um das gleiche Ziel zu erreichen:

**1. Für SchülerInnen: Teilen macht erfinderisch (ChatGPT)**
Wenn Sie als Lehrkraft über einen ChatGPT Plus-Account verfügen und dort einen Assistenten (wie die PHARMA-KI) bauen, können Sie den Link dazu generieren. Der große Vorteil: Wenn Sie diesen Link mit Ihrer Klasse teilen, können SchülerInnen mit einem **kostenlosen** ChatGPT-Account diesen Assistenten in vollem Umfang nutzen! 

**2. Der "Copy & Paste"-Trick (Das analoge Gem)**
Die simpelste und plattformunabhängige Methode: Legen Sie sich ein Word-Dokument, eine OneNote-Seite oder eine einfache Textdatei mit Ihren liebsten System-Prompts an. 
* Öffnen Sie einen normalen, kostenlosen Chat (z. B. die Gratisversionen von Gemini, ChatGPT oder Claude).
* Fügen Sie Ihren kopierten System-Prompt (die langen Regieanweisungen aus den Boxen oben) als **allererste Nachricht** in den Chat ein.
* Senden Sie die Nachricht ab. Die KI schlüpft ab diesem Moment für den Rest der Unterhaltung exakt in diese Rolle!

**3. "ChatGPT anpassen" (Custom Instructions)**
Auch in der Gratis-Version von ChatGPT gibt es eine versteckte Funktion, die wie ein "Mini-Gem" wirkt: Klicken Sie unten links auf Ihren Namen und wählen Sie **"ChatGPT anpassen" (Custom Instructions)**. Dort können Sie in zwei Textfeldern dauerhaft hinterlegen, dass Sie Chemielehrkraft sind und Antworten z.B. immer strukturiert und altersgerecht für die Sekundarstufe formuliert werden sollen. Das System merkt sich das für jeden zukünftigen Chat.

**4. Echte Bots auf kostenlosen Plattformen bauen**
Wenn Sie wirklich eigene, anklickbare Assistenten mit System-Prompt bauen wollen, ohne dafür zu bezahlen, sind offene Plattformen wie **[Poe.com](https://poe.com/)** oder **[HuggingChat](https://huggingface.co/chat/)** eine exzellente Wahl. Dort können Sie sich als Lehrkraft kostenlos eigene "Bots" zusammenklicken und diese direkt nutzen.

---

## 🚀 Praxis-Anleitung: Eigene Bots kostenlos bauen

Wenn Sie das Prinzip der "Gems" oder "Custom GPTs" voll ausschöpfen möchten, ohne Geld für ein Pro-Abo in die Hand zu nehmen, empfehle ich Ihnen **HuggingChat** oder **Poe.com**. 

Besonders **HuggingChat** ist für Schulen fantastisch, da es komplett kostenlos ist und auf modernste, offene KI-Modelle zugreift.

### So bauen Sie einen Assistant in HuggingChat:

1. Gehen Sie auf **[huggingface.co/chat](https://huggingface.co/chat/)** (Sie benötigen einen kostenlosen Account).
2. Klicken Sie in der linken Seitenleiste auf **"Assistants"** und dann oben rechts auf **"Create new assistant"**.
3. **Avatar & Name:** Geben Sie Ihrem Bot ein Gesicht (Icon hochladen) und einen Namen (z. B. "Redox-Coach").
4. **Description:** Ein kurzer Satz für die SchülerInnen (z. B. "Ich helfe dir Schritt für Schritt bei Redoxgleichungen").
5. **System Instructions (Das Wichtigste!):** Hier fügen Sie Ihren Regie-Prompt ein (siehe Beispiel unten).
6. **Start Messages:** Geben Sie Beispiele vor, auf die SchülerInnen nur noch klicken müssen (z.B. *"Hilf mir bei der Reaktion von Kupfer mit Salpetersäure"*).
7. Klicken Sie ganz unten auf **"Create"**. 

Ihr Bot ist jetzt fertig! Sie können den Link aus der Adresszeile kopieren und direkt per QR-Code an Ihre SchülerInnen verteilen.

### 🧪 Ein konkretes Beispiel für Ihren neuen Bot

Klicken Sie auf die Box, um einen perfekten System-Prompt für einen interaktiven Schüler-Bot zu kopieren. Dieser Bot löst Aufgaben nicht einfach, sondern fungiert als echter Nachhilfelehrer!

??? success "Der System-Prompt: Der interaktive Redox-Coach"
    Kopieren Sie diesen Text exakt so in das Feld "System Instructions" bei HuggingChat oder Poe:
    
    > "Du bist ein geduldiger, didaktisch hervorragender Chemie-Tutor für die Oberstufe. Deine Aufgabe ist es, SchülerInnen beim Aufstellen komplexer Redoxgleichungen zu helfen.
    > 
    > **Deine strikten Regeln:**
    > 1. Löse die Gleichung NIEMALS sofort komplett! Das ist extrem wichtig.
    > 2. Führe den Schüler stattdessen sokratisch, Schritt für Schritt, durch den Prozess:
    >    - Schritt 1: Oxidationszahlen bestimmen lassen.
    >    - Schritt 2: Oxidation und Reduktion identifizieren.
    >    - Schritt 3: Teilgleichungen (Elektronenübergang) aufstellen.
    >    - Schritt 4: Ladungs- und Stoffausgleich (in saurer oder basischer Lösung).
    > 3. Stelle nach jedem Schritt eine klare Frage an den Schüler und **warte auf seine Antwort**, bevor du zum nächsten Schritt übergehst.
    > 4. Wenn der Schüler einen Fehler macht, korrigiere ihn sanft, gib einen kleinen Tipp und lass es ihn noch einmal versuchen.
    > 5. Lobe den Schüler, wenn er einen Zwischenschritt richtig hat!"
