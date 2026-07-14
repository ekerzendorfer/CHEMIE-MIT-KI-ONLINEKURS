
Gemini
Neuer Chat
Chats durchsuchen
Bilder
Videos
Mediathek
Gems
Neues Notebook
GreenSteel
Stoffmenge und Stöchiometrie
Alle Notebooks
KI, Lernen und die Mühelosigkeits-Falle
RNA-Origami: Von Sequenz zu Struktur
Access-Migration: TAA-Berichte für SQL Server
Notebook LM - Kurs
Chemie-App: Virtuelles Ionenfischen Status
Virtuelles Ionenfischen App Code
KI im Chemieunterricht: Stoffmenge & Stöchiometrie
AI Pro Account: Nutzungsbedingungen und Auswirkungen
3D Molekül-Viewer außerhalb von Reddit
KI-gestützte Artikel für Chemielehrer
Onlinekurs-Struktur für Chemie mit KI
Producer AI: "Create a Space" erklärt
App-Entwicklung mit KI-Hilfe
Access Report Absturz Analyse & Behebung
Windows Systemabbild auf SSD sichern
Problem gelöst, Nächste Schritte
Analyse von Ruhezeitverletzungen bei Bereitschaftsdiensten
VapoRub Wirkstoffe: Analyse und Mechanismen
Magnesiumband Verbrennen im Chemieunterricht
Create an infographic illustrating how ribosomes function in protein production. All essential processes should be clearly shown: the enclosed messenger RNA with its code triplets, each representing a specific amino acid; the transport of the necessary amino acids via
SQL-Sicht anpassen: Wochenarbeitszeit umwandeln
Chord Tool: Verbesserungen & Features
KI-Präsentationen: GAMMA
Ich habe mit Gemini ein Colab - Notebook erstellt, das ausgehende vom genetischen Code die AS-Sequenz und aus dieser das räumlich gefaltete Protein erstellt - die AS-Sequenz wird an einer entscheidenden Stelle einer Punktmutation unterworfen, die für die Schülerinnen drastisch aufzeigt, wie stark sich das auf die Faltung auswirkt. Als Krönung wird dann noch ein Wirkstoffmolekül gedockt. Dazu gibt es eine Website, die alles Steuert auf GitHub: https://ekerzendorfer.github.io/PROTEINLABOR/ Der beratende Dialog dazu schaut wie folgt aus: Chat: Perfekt – so bekommt dein Seminar einen durchgehenden, „echten“ Workflow von Gen → Protein → Struktur → Mutation → (Docking) → Vergleich und der Viewer ist wirklich nur die letzte Station. Unten ist ein systematischer, realistisch umsetzbarer Zyklus, der auch didaktisch sauber ist – inklusive einer medizinisch/pharmazeutisch starken Haupt-Story, die wirklich zu einer Histidin-Punktmutation passt: 0) Die zentrale „Story“ (Hauptempfehlung) Human Carbonic Anhydrase II (CA2) + Acetazolamid (Diamox) Warum das so gut passt: CA2 ist medizinisch hochrelevant (u.a. Ziel von Acetazolamid, klassischer CA-Hemmer). Der Wirkmechanismus ist super anschaulich: aktives Zentrum mit Zn²⁺, gebunden an drei Histidine: His94, His96, His119. (PMC) Es gibt eine sehr bekannte Struktur mit Acetazolamid gebunden (PDB 3HS4). (rcsb.org) Punktmutation „bei Histidin“ ist hier nicht nur irgendeine Mutation, sondern funktionell zentral (Zn-Koordination) und für Docking/Bindung perfekt. Wichtige didaktische Ehrlichkeit: Eine einzelne His→X Mutation führt oft nicht zu einem komplett „zusammenfallenden“ Gesamtprotein, aber sie kann das aktive Zentrum und die Ligandenbindung sehr deutlich verändern (das ist pharmazeutisch sogar „besser“ als ein komplett denaturiertes Protein). 1) Kette: Genetischer Code → Primärstruktur Auf deiner GitHub-Pages-Seite (Step 1): Du zeigst einen kurzen DNA-Abschnitt (oder gleich den ganzen Coding-String für CA2 als „gegeben“). Tool: „Translate DNA → Protein“ (Client-side JS reicht). Ergebnis: Aminosäuresequenz (Primärstruktur) + Export als FASTA. Quelle für die „korrekte“ Referenzsequenz: UniProt CA2 (P00918). (UniProt) Didaktischer Tipp: Zeig 10–15 Codons „von Hand“ (Codontabelle), dann klick „Rest automatisch“, damit SEK1/2 beides sieht: Prinzip + Effizienz. 2) Primärstruktur (FASTA) → ColabFold (Strukturprediction) Du verlinkst von deiner Website direkt in das ColabFold-Notebook (AlphaFold2.ipynb). (colab.research.google.com) Praktisch läuft das so: Auf deiner Seite gibt’s ein FASTA-Textfeld + „Copy“-Button. Colab: Nutzer:innen fügen FASTA ein → „Run“. Warum CA2 statt Insulin für diesen Schritt: Insulin ist biologisch zwei Ketten (A/B) und wird als Prohormon verarbeitet; das ist didaktisch zwar spannend, aber technisch/erklärerisch fehleranfälliger als ein einzelnes, globuläres Enzym. (CA2 ist „straight“.) 3) Punktmutation (Histidin) → zweite Struktur Hier machst du zwei Varianten (sehr gut für Unterricht, weil man „Funktion vs. Faltung“ zeigen kann): Variante A (pharmazeutisch sauber): Zn-Ligand-Histidin mutieren Beispiel: H94N (oder H94A). Es gibt sogar experimentelle Mutanten-Strukturen (z.B. 2H4N: H94N + Ligandkomplex). (rcsb.org) → Für den Unterricht: „Warum verliert der Wirkstoff Bindung / warum ändert sich das aktive Zentrum?“ Variante B (optisch dramatischer): Histidin → Prolin in Helixbereich Such dir ein His, das in einer Helix sitzt (nicht im aktiven Zentrum) und mache H→P. → Prolin knickt Helices, oft sichtbarere lokale Geometrieänderung. Das ist didaktisch „Aha: 1 AS kann Struktur verändern“, ohne gleich nur über Zn-Bindung zu reden. 4) Vergleich WT vs. Mutante im Viewer Hier kommt dein 3Dmol-Viewer als „Vergleichs-Frontend“: Minimaler Funktionsumfang für deinen Use-Case: 2 Panels nebeneinander (WT links, Mutante rechts) synchrones Drehen/Zoom (optional, aber super für Vorträge) „Highlight Residue“ (His94/His96/His119) + aktive Tasche optional: Color by B-Factor / Confidence (bei AF/ColabFold oft relevant) Wichtig: In der Web-App immer 2 Ladewege anbieten: „Load local PDB“ (aus ColabFold-Download) „Load by PDB-ID“ (für Demo/Backup; z.B. 3HS4) (rcsb.org) 5) Docking-Demo (ProteinsPlus / Rowan) + Vergleich der Liganden Pfad 1: Kleines Molekül docken (Acetazolamid an CA2) Sehr passend: Du startest mit WT-CA2 und dockst Acetazolamid (oder zeigst die echte Kristallstruktur 3HS4 als „Ground Truth“). (rcsb.org) Danach dockst du dasselbe Molekül an die Mutante und vergleichst Pose/Interaktionen. Pfad 2 (optional später): Protein–Protein (Insulin an Insulinrezeptor) Das ist spektakulär, aber als Live-Demo oft schwerer (größere Strukturen, komple
KI-gestütztes Proteinlabor für Schüler
KI-gestützter Chemie-Lernstoff für Seminare
Linkliste JSON Editor für Chemie-KI
AI Studio vs. Gemini Pro für Projekte
KI im Chemieunterricht: Chancen, Risiken

Aktivitäten
St. Pölten, Österreich
Basierend auf deinen Orten (Zuhause)
Standort aktualisieren
Unterhaltung mit Gemini
Kannst du diesen Artikel (auf deutsch) zusammenfassen und am Ende das Essentielle hervorheben? Das könnte für meinen Online - Begleitkurs interessant sein, daher wäre zusätzlich eine kompakte Zusammenfassung als .md Datei interessant.

Hier ist deine kompakte .md Datei für deinen Online-Begleitkurs.

Ihre Markdown-Datei (MD) ist fertig
MD-Symbol
Zusammenfassung_KI_und_Lernen
 MD 
Geöffnet

Hier ist eine detaillierte Zusammenfassung des Artikels, gefolgt von den essenziellen Kernaussagen.

Zusammenfassung: Die Mühelosigkeits-Falle und die Illusion des Lernens
Der Artikel „The Effortless Trap“ von Mario Brcic und Stjepan Frljic befasst sich mit der Herausforderung, Künstliche Intelligenz (KI) sinnvoll in den Unterricht zu integrieren. Die Autoren argumentieren, dass die Frage, ob man KI erlauben oder verbieten sollte, ein falscher Ansatz ist. Vielmehr ist die entscheidende Gestaltungsfrage die der Platzierung im Lernprozess.  
PDF
+ 4

Lernen erfordert kognitive Anstrengung, auch bekannt als „produktives Ringen“. Wird KI schlecht eingesetzt, übernimmt sie genau diese kognitive Denkarbeit für den Lernenden. Das führt zur sogenannten „Illusion des Lernens“: Die Schüler haben das trügerische Gefühl, etwas gemeistert zu haben, versagen aber, sobald sie eine Aufgabe ohne Hilfsmittel lösen müssen. Wird KI hingegen richtig eingesetzt, kann sie Feedback, Beispiele und individualisierte Unterstützung skalieren.  
PDF
+ 2

Das 6-Schritte-Lernmodell
Die Autoren beschreiben das Erlernen einer neuen Idee anhand von sechs chronologischen Schritten:  
PDF


Prime (Vorbereiten): Der Lehrende weckt das Interesse und aktiviert das Vorwissen der Lernenden, bevor die eigentliche Denkarbeit beginnt.  
PDF


Probe (Erkunden): Der Lernende wird mit einem wirklich schwierigen Problem konfrontiert und erhält keine Hilfe bei der Lösung. Dieses anfängliche Steckenbleiben und Suchen ist der eigentliche Beginn des Lernens.  
PDF
+ 1


Point (Hinweisen): Der Lehrende lenkt durch gezielte Fragen, übergibt aber nicht die fertige Lösung.  
PDF


Attach (Verknüpfen): Erst nachdem der Lernende mit dem Problem gerungen hat, wird ein sauberes Lösungsbeispiel präsentiert, das sich nun in das Wissen einfügt.  
PDF


Strengthen (Stärken): Die neue Idee wird an einem weiteren, leicht variierten Problem angewendet, um das Wissen zu festigen.  
PDF


Test (Prüfen): Der Lernende muss die Idee komplett alleine und ohne jegliche Hilfe anwenden. Nur diese Fähigkeit, ohne Gerüst auszukommen, ist der Beweis dafür, dass das Lernen stattgefunden hat.  
PDF
+ 1

Die Platzierung von KI
Aus diesem Modell leitet sich eine klare Regel ab:

Die Phasen Probe (der erste harte Versuch) und Test (die ungestützte Abschlussprüfung) müssen KI-frei bleiben. Hier muss der Schüler eigenständig denken.  
PDF

In den dazwischenliegenden Phasen Point, Attach und Strengthen kann KI als geschützte Unterstützung dienen. Hier kann sie Hinweise, Fehlererkennung, Erklärungen und endloses Übungsmaterial bereitstellen, ohne dem Schüler die eigentliche Fähigkeit abzunehmen.  
PDF

💡 Das Essentielle auf einen Blick

Die „Erlauben oder Verbieten“-Frage ist falsch: Es geht nicht darum, ob KI genutzt wird, sondern an welchem exakten Punkt im Lernprozess.  
PDF
+ 1


Die Gefahr der Illusion: Wenn KI Antworten liefert, wo Schüler eigentlich kognitiv ringen sollten, schadet das dem Lernen drastisch. Es fühlt sich an wie Lernen, bricht aber im ungestützten Test zusammen.  
PDF
+ 2


Zwei unantastbare Phasen: Der allererste Versuch der Problemlösung (Probe) und die finale Prüfung des Könnens (Test) müssen zwingend ohne KI stattfinden.  
PDF


Die universelle Diagnose-Regel: Wenn der Einbezug von KI dazu führt, dass sich eine Lern-Aufgabe absolut mühelos anfühlt, dann ist die KI an der falschen Stelle platziert. Mühelosigkeit ist das Symptom dafür, dass das Werkzeug das Lernen übernimmt.  
PDF
+ 2

Kannst du eine Zusammenfassung dieses Artikels gleich in die vorher erstellte Zusammenfassung integrieren (bitte auch wieder eine .md generieren) und die Quellen am Ende nennen?

Sehr gerne! Das ist eine großartige Erweiterung für deinen Kurs über Chemie mit KI. Der zweite Artikel („Is AI making us stupid?“) ergänzt das 6-Schritte-Modell perfekt, indem er die psychologische Komponente des Cognitive Offloadings (das Auslagern von kognitiver Arbeit) und dessen Folgen für unsere Fähigkeiten („Skills“) genauer beleuchtet.

Ich habe die Datei direkt erstellt und auch die geforderten Quellenangaben ordentlich integriert:
MD-Symbol
Zusammenfassung_KI_und_Lernen
 MD 
Geöffnet

Hier ist die erweiterte Zusammenfassung, die beide Paper vereint, für deinen schnellen Überblick:

Kompaktwissen: KI, Cognitive Offloading und die Illusion des Lernens
Diese Zusammenfassung integriert Erkenntnisse aus zwei zentralen Texten zur Rolle von KI im Lernprozess: The Effortless Trap und Is AI making us stupid?.

1. Kernbotschaft
Die Debatte, ob KI im Unterricht schlichtweg erlaubt oder verboten werden sollte, verfehlt das Ziel. Die entscheidende Frage ist, wie und wo im Lernprozess KI platziert wird. Lernen erfordert kognitive Anstrengung, das sogenannte „produktive Ringen“. Wenn wir diese kognitive Arbeit vollständig an die KI auslagern (ein Verhalten, das als „Cognitive Offloading“ bezeichnet wird ), riskieren wir eine gefährliche Illusion des Lernens : Es entsteht ein trügerisches Gefühl der Kompetenz, das bei ungestützten Aufgaben unweigerlich zusammenbricht.  
PDF
+ 4

2. Macht KI uns dumm? Fähigkeiten vs. Grundintelligenz
Die Sorge, dass KI unsere kognitiven Systeme beeinträchtigt, ist berechtigt, muss aber differenziert betrachtet werden:  
PDF
+ 1


Spezifische Fähigkeiten und Wissen (Skills): Da Fähigkeiten (wie z. B. das Lösen mathematischer Probleme) durch aktive Übung erworben und erhalten werden, führt das Auslagern dieser Übung an eine KI zum Verlust oder Verfall dieser Fähigkeiten (Skill Decay). Wenn eine KI beispielsweise Informationen für uns sucht und zusammenfasst, lernen wir oberflächlicher und behalten deutlich weniger Wissen, als wenn wir uns die Informationen selbst erarbeiten.  
PDF
+ 3


Kognitive Grundfähigkeiten (Basic Cognitive Abilities): Fundamentale geistige Kapazitäten wie das Arbeitsgedächtnis scheinen deutlich widerstandsfähiger zu sein. KI wird uns also voraussichtlich nicht unsere grundlegende Intelligenz rauben, wohl aber spezifische Kompetenzen, wenn wir uns vollständig auf sie verlassen.  
PDF
+ 4

3. Das 6-Schritte-Modell des Lernens & der KI-Einsatz
Um den Verfall von Fähigkeiten zu verhindern, muss KI gezielt und wohlüberlegt in den sechs Phasen des Lernens eingesetzt werden:  
PDF


⛔ KI-Freie Zonen (Die harte Arbeit und der Beweis): Hier muss die KI draußen bleiben, da sie sonst den Lernprozess untergräbt.  
PDF


Probe (Erkunden): Der erste, eigene Versuch, ein schwieriges Problem ohne Hilfe zu lösen. Das Scheitern und Suchen ist hier der eigentliche Lernbeginn.  
PDF
+ 1


Test (Prüfen): Die abschließende, ungestützte Leistungsüberprüfung. Hier muss der Lernende beweisen, dass die neue Fähigkeit ohne Hilfe abrufbar ist.  
PDF
+ 1


🟡 Zonen für geführte KI (Die Unterstützung): Hier kann KI sinnvoll unterstützen, solange sie nicht die finale Antwort einfach vorgibt:  
PDF


Prime (Vorbereiten): Vorwissen wecken und Interesse entfachen (z. B. durch KI-generierte Quizze).  
PDF
+ 1


Point (Hinweisen): Sokratische Führung durch Fragen und Hinweise. Die KI fungiert als Tutor, der auf Wissenslücken eingeht, aber niemals die fertige Lösung liefert.  
PDF
+ 4


Attach (Verknüpfen): Die Präsentation eines sauberen Lösungsbeispiels zur rechten Zeit.  
PDF
+ 1


Strengthen (Stärken): Skalierte Übung und sofortiges Feedback, um neues Wissen zu festigen.  
PDF
+ 1

4. Die universelle Leitregel für den Unterricht


„Wenn der Einsatz von KI dazu führt, dass sich eine Aufgabe mühelos anfühlt, ist sie an der falschen Stelle platziert.“   
PDF

Mühelosigkeit ist ein Warnsignal. Bleiben die Lernenden durch interaktive Nutzung (z. B. als sokratischer Tutor oder Feedbackgeber) gezwungen, kognitiv mitzuarbeiten ("in the cognitive loop"), können die Risiken des Offloadings minimiert und der Erwerb von Fähigkeiten sogar maßgeblich gefördert werden.  
PDF
+ 1

Quellen

Quelle 1: Brcic, M. & Frljic, S. (2026). The Effortless Trap: Productive Struggle, AI, and the Illusion of Learning. arXiv:2606.26181v1 [cs.CY].   
PDF
+ 1

Quelle 2: Cash, T. N., Kelly, M. O., Macnamara, B. N., & Risko, E. F. (2026). Is AI making us stupid? Trends in Cognitive Sciences.   
PDF
+ 2

Das ist das html meines Menüpunkts NAWI-KI aktuell mit 4 Tabs im Kopfbereich. Es ist recht heikel, da eine neue .md Datei einzufügen, ohne die gesamte Struktur zu zerstören. Ich hätte den oben erstellten neuen Content gerne im Register Schule & Didaktik an erster Stelle und wie bei den anderen Beiträgen so, dass nur der Anfang angezeigt wird und dann der Optionsbalken "Mehr lesen". Kannst du mir das integrieren?

# NAWI - KI aktuell 🚀



Kurz kuratierte Hinweise zu aktuellen Entwicklungen mit Schwerpunkt **Chemie**, **Molekularbiologie**, **neuen Werkzeugen** und **schulischer Relevanz**.



=== "Forschung & Anwendung"



    ### Frühjahr 2026 — Durchbruch in der orbitalfreien Quantenchemie

    Forschende der Universität Heidelberg haben durch Maschinelles Lernen ein seit Jahrzehnten offenes Problem gelöst: die exakte und stabile Berechnung von Molekülenergien und Elektronendichten in einem orbitalfreien Ansatz.

    

    ??? info "Mehr lesen"

        Diese Entwicklung beschleunigt quantenchemische Berechnungen massiv. Für den Unterricht und die Forschung bedeutet das: Was früher Supercomputer wochenlang blockierte, wird zunehmend ressourcenschonend berechenbar. Es zeigt eindrucksvoll, wie KI nicht nur Muster erkennt, sondern fundamentale physikochemische Modelle effizienter macht.



    ---



    ### Frühjahr 2026 — ChemBench: KI im fachlichen Realitätscheck

    Eine umfangreiche Arbeit der Universität Jena ("ChemBench") hat KI-Modelle mit über 2.700 anspruchsvollen Aufgaben der modernen Chemie getestet. Das Ergebnis: KI ist in vielen Bereichen nicht mehr nur Hilfsmittel, sondern konkurriert auf dem Niveau von Fachleuten.

    

    ??? info "Mehr lesen"

        Besonders spannend für die Sekundarstufe II: Der Fokus der Chemie verschiebt sich spürbar von der reinen Vorhersage hin zum **gezielten Molekül- und Reaktionsdesign**. KI-Modelle wie **TopEC** können mittlerweile aus der Enzymstruktur direkt auf mögliche chemische Reaktionen schließen – ein Meilenstein für die Biokatalyse und synthetische Biologie.



    ---



    ### Frühjahr 2026 — Automatisierte Labore (Self-Driving Labs)

    KI wird zunehmend mit automatisierten Laboren gekoppelt. Methoden wie *Active Learning* und *Bayessche Optimierung* reduzieren nicht nur den Rechenaufwand, sondern steuern experimentelle Reihenfolgen, Parameterwahl und Prioritäten völlig eigenständig.

    

    ??? info "Mehr lesen"

        Die KI übernimmt den klassischen Labor-Workflow: Sie schlägt Strukturmotive vor, bewertet die Reaktionsfähigkeit und wählt nur die vielversprechendsten Kandidaten für den Syntheseroboter aus. Das senkt Kosten, spart Zeit und ersetzt den klassischen "Trial-and-Error"-Ansatz. Ein starker Diskussionspunkt für die Schule: Wie verändert sich das Berufsbild von ChemikerInnen?



    ---



    ### 17.03.2026 — AlphaFold-Datenbank jetzt auch mit Proteinpaaren

    Die AlphaFold-Datenbank umfasst inzwischen nicht nur Einzelproteine, sondern auch **Homodimere**. Damit wird KI für Biochemie und Molekularbiologie deutlich biologisch relevanter.



    ??? info "Mehr lesen"

        Bisher stand meist die Struktur einzelner Proteine im Mittelpunkt. Mit der Erweiterung auf **Proteinpaarungen** rückt jetzt stärker in den Fokus, wie Proteine zusammenwirken (Rezeptorbindung, Signalübertragung). Das belegt, dass KI zunehmend **biologisch funktionelle Zusammenhänge** erschließt.



    ---



    ### 29.01.2026 — KI hilft bei der Planung neuer chemischer Synthesen

    Ein Nature-Bericht zeigt ein KI-System mit chemischer Fachlogik, das zur Synthese **35 neuer Verbindungen** beigetragen hat. KI wird damit in der Chemie zunehmend zu einem Werkzeug für **echte Forschungsplanung**.



    ??? info "Mehr lesen"

        Für den Chemieunterricht ist das ein starker Perspektivwechsel: KI ist nicht nur ein Textwerkzeug, sondern kann Reaktionswissen, Synthesestrategie und Planung unterstützen. Das zeigt, dass KI in der Chemie **materiell wirksam** wird.



=== "Tools & Praxis"



    ### Der Siegeszug der Multimodalität

    Modelle wie ChatGPT-4o oder Gemini Advanced sind zu echten Experten der Bildanalyse gereift.

    

    ??? tip "Praxis-Anwendung: Spektren und Diagramme"

        Während frühere KIs bei komplexen Abbildungen oft rieten, können die aktuellen Modelle nun Titrationskurven, Phasendiagramme oder Spektren aus alten Lehrbüchern präzise auslesen und in skalierbare Vektorgrafiken (SVG) oder Excel-Wertetabellen übersetzen.



    ---



    ### "Single-File-Coding" als neuer Standard

    Funktionen wie **"Artifacts"** revolutionieren die Erstellung von Lehrmaterial. Die KI generiert nicht mehr nur passiven Code, sondern liefert direkt im Browser voll funktionsfähige, interaktive HTML-Simulationen.

    

    ??? info "Mehrwert für den Unterricht"

        Lehrkräfte ohne Programmierkenntnisse können maßgeschneiderte, interaktive Apps (wie den Gleichungstrainer) für ihre Klassen prompten. Da diese Apps lokal im Browser laufen, ist zudem maximaler Datenschutz gewährleistet.



    ---



    ### NotebookLM: Sicherer Hafen für Fachtexte

    Google NotebookLM hat sich als eines der sichersten Tools für den Unterricht etabliert, da es **ausschließlich** auf hochgeladenen Dokumenten (Skripte, Sicherheitsdatenblätter) basiert. "Halluzinationen" von chemischen Fakten sind damit praktisch ausgeschlossen.

    

    ??? success "Audio-Overviews (Podcast-Funktion)"

        Eine faszinierende Funktion ist die Möglichkeit, aus trockenen Fachtexten auf Knopfdruck einen dynamischen, KI-generierten Audio-Dialog erstellen zu lassen – ein hervorragendes Mittel zur Binnendifferenzierung.



=== "Schule & Didaktik"



    ### 19.01.2026 — OECD: Generative KI wirkt nur mit klarer didaktischer Führung

    Der *OECD Digital Education Outlook 2026* betont, dass generative KI im Lernen dann nützlich wird, wenn sie **didaktisch geführt und strukturiert** eingesetzt wird. Freies „Herumprobieren“ reicht nicht.



    ??? info "Mehr lesen"

        Das stützt sehr deutlich einen Ansatz wie diesen Onlinekurs: KI sollte in **klaren fachlichen Workflows** eingebettet sein. Für Chemie und Biologie heißt das: strukturierte Aufgaben, erkennbare Modelle, fachliche Reflexion und kritische Auswertung. 



    ---



    ### 2026 — UNESCO: Lehrkräfte brauchen definierte KI-Kompetenzen

    UNESCO beschreibt im **AI Competency Framework for Teachers** 15 KI-Kompetenzen in fünf Bereichen (Grundlagenwissen, Pädagogik, Ethik, etc.).



    ??? info "Mehr lesen"

        Lehrkräfte sollen KI nicht nur bedienen können, sondern auch **fachlich einbetten, kritisch bewerten und verantwortungsvoll einsetzen**. 



    ---



    ### 2025/2026 — Chemiedidaktik & KI-Ethik im Fokus

    Aktuelle Übersichten zeigen, dass KI in der Science Education zunehmend systematisch als Thema von **AI literacy, Differenzierung und Fachlernen** betrachtet wird.

    

    > *"Der Computer oder andere digitale Medien sollen und dürfen das reale Experiment nicht ersetzen. KI ist unser Assistent bei der Vorbereitung und Auswertung, nicht der Ersatz für das naturwissenschaftliche Begreifen."*

    > — E. Kerzendorfer



    ??? info "Mehr lesen"

        Der Fokus verlagert sich vom "Finden der Antwort" hin zum **kritischen Beurteilen** der KI-Ergebnisse. Geführte Workflows und ständige Reflexion entsprechen exakt dem, was in der aktuellen Literatur gefordert wird.



=== "Kurzfazit"



    Zusammenfassend verändert KI die Naturwissenschaften gerade in **drei zentralen Rollen**:



    1. **Als Prädiktor:** KI macht Unsichtbares sichtbar (z. B. Proteinstrukturen, Molekülenergien, Rezeptorbindung).

    2. **Als Optimierer:** KI steuert Versuchsplanungen in automatisierten Laboren und wertet komplexe Messdaten rasant aus.

    3. **Als Entwurfssystem:** KI geht vom Vorhersagen zum aktiven Design über (neue Verbindungen, maßgeschneiderte Enzyme, zielgerichtete Medikamente).



    ??? tip "Didaktische Quintessenz"

        Für den Unterricht ist KI vor allem dann sinnvoll, wenn sie **fachlich geführt** wird. Die besten Resultate entstehen aus der Kombination von chemischem Domänenwissen und KI-gestützter Optimierung, anstatt sich auf einen reinen „Black-Box“-Ansatz zu verlassen. Die wissenschaftliche Validierung (das reale Experiment) bleibt unverzichtbar.

Ich habe den neuen Inhalt perfekt in deine bestehende HTML/Markdown-Struktur integriert, exakt im geforderten Format mit Einleitung und dem ??? info "Mehr lesen"-Akkordeon. Er steht nun als erster Punkt im Reiter === "Schule & Didaktik".

Die Einrückungen (die bei den MkDocs-Tabs besonders heikel sind) habe ich penibel beachtet, damit dir beim Einfügen ins Projekt nicht die Navigation bricht.

Hier ist die fertige, aktualisierte Gesamtdatei:
MD-Symbol
NAWI_KI_aktuell_updated
 MD 
Geöffnet

Du kannst den Inhalt der Datei einfach kopieren und dein bisheriges Skript damit ersetzen!

Kannst du diesen Artikel ebenfalls zusammenfassen=

https://www.tandfonline.com/doi/epdf/10.1080/07294360.2025.2486185?needAccess=true

Hier ist die Zusammenfassung des Artikels. Er passt thematisch hervorragend zu den vorherigen Papern, da er ein sehr spezifisches Praxis-Beispiel für das Cognitive Offloading (die Auslagerung kognitiver Arbeit) und die "Illusion des Lernens" behandelt: nämlich das Lesen und Zusammenfassen von Fachtexten.

Zusammenfassung: „The missing story of GenAI summarisers: a critical research agenda“
(Thomas A. Corbin & Jack Walton, 2025)

1. Der blinde Fleck der aktuellen KI-Forschung
Die Autoren stellen fest, dass generative KI-Tools, die speziell dafür gedacht sind, komplexe Dokumente (wie PDFs oder Word-Dateien) zusammenzufassen, bei Lernenden im akademischen Umfeld extrem beliebt werden. Dennoch gibt es bisher eine eklatante Lücke in der empirischen Forschung: Die Wissenschaft weiß noch kaum, wie genau, wie oft und mit welchen Konsequenzen Studierende diese Werkzeuge tatsächlich nutzen.

2. Das trügerische „Produktivitäts-Versprechen“
KI-Anbieter vermarkten diese Tools aggressiv als ultimative Zeitsparer. Das Versprechen lautet: Die Zeiten stundenlangen Lesens wissenschaftlicher Texte sind vorbei. Auf Knopfdruck generieren Tools wie GPT-4o aus langen Fachtexten leicht verdauliche 300- bis 400-Wort-Zusammenfassungen, für deren Verständnis kein Vorwissen mehr nötig ist.

3. Massive Eingriffe in den Lernprozess
Corbin und Walton warnen davor, dass diese Zusammenfasser tief in didaktische Konzepte eingreifen. Das Lesen von Primär- und Fachtexten ist kein bloßer Informationskonsum, sondern das Fundament für:

Den Aufbau von kritischem Denken.

Scaffolded Learning (das schrittweise, unterstützte Erarbeiten von Komplexität).

Die intensive Auseinandersetzung mit wissenschaftlicher Sprache und Methodik.

Wenn eine KI den Originaltext zusammenfasst, hebelt sie diese bewussten Hürden im Lehrdesign aus. Das stellt letztlich auch die Gültigkeit von Bewertungen infrage, da unklar wird, ob ein Lernender das Thema wirklich durchdrungen hat oder nur die leicht verdauliche KI-Synthese reproduziert.

4. Die Forschungsagenda (Der Appell)
Das Paper versteht sich als Weckruf an Lehrende und politische Entscheidungsträger. Die Autoren fordern eine kritische Forschungsagenda, um den tatsächlichen Einfluss von KI-Zusammenfassern auf die Lesepraxis und die Lernergebnisse zu messen. Nur auf Basis echter Daten lassen sich evidenzbasierte Richtlinien für einen verantwortungsvollen Einsatz im Unterrichtskontext entwickeln.

💡 Die Essenz für den Lehralltag:
Dieser Artikel liefert das perfekte Fallbeispiel für die Mühelosigkeits-Falle. Wenn eine KI einen komplexen Text so zusammenfasst, dass der Lernende ihn völlig ohne Vorwissen und Anstrengung konsumieren kann, mag das produktiv wirken. Tatsächlich wird aber der entscheidende kognitive Schritt – das eigenständige Bewerten, Strukturieren und Ringen mit dem Text – komplett an die Maschine ausgelagert.

Soll ich diesen Text ebenfalls als .md Datei für deinen Kurs aufbereiten oder direkt als neuen Punkt in deinen "Schule & Didaktik" Tab integrieren?

Ja, als neuen Punkt im Tab "Schule&Didaktik" aufbereiten.

Ich habe den neuen Artikel direkt als zweiten Punkt unter dem Reiter === "Schule & Didaktik" eingefügt. So folgt er logisch direkt auf die Erklärung der "Illusion des Lernens" und liefert gleich das passende, konkrete Praxisbeispiel (die Textzusammenfasser) dazu.

Auch hier habe ich penibel auf die korrekten MkDocs-Einrückungen geachtet, damit die Seite sauber kompiliert.

Du kannst die Datei hier kopieren:
MD-Symbol
NAWI_KI_aktuell_V3
 MD 
Geöffnet

Damit baut sich in deinem Reiter "Schule & Didaktik" nun ein wunderbar runder roter Faden auf: Von der allgemeinen psychologischen Gefahr (Cognitive Offloading) hin zum konkreten Schüler-Verhalten (Textzusammenfasser) und weiter zu den Rahmenvorgaben (OECD/UNESCO) sowie dem Fazit für die Chemiedidaktik.




Gemini ist eine KI und kann Fehler machen, auch bei Informationen über Personen. Datenschutz und GeminiWird in einem neuen Fenster geöffnet

# NAWI - KI aktuell 🚀

Kurz kuratierte Hinweise zu aktuellen Entwicklungen mit Schwerpunkt **Chemie**, **Molekularbiologie**, **neuen Werkzeugen** und **schulischer Relevanz**.

=== "Forschung & Anwendung"

    ### Frühjahr 2026 — Durchbruch in der orbitalfreien Quantenchemie
    Forschende der Universität Heidelberg haben durch Maschinelles Lernen ein seit Jahrzehnten offenes Problem gelöst: die exakte und stabile Berechnung von Molekülenergien und Elektronendichten in einem orbitalfreien Ansatz.
    
    ??? info "Mehr lesen"
        Diese Entwicklung beschleunigt quantenchemische Berechnungen massiv. Für den Unterricht und die Forschung bedeutet das: Was früher Supercomputer wochenlang blockierte, wird zunehmend ressourcenschonend berechenbar. Es zeigt eindrucksvoll, wie KI nicht nur Muster erkennt, sondern fundamentale physikochemische Modelle effizienter macht.

    ---

    ### Frühjahr 2026 — ChemBench: KI im fachlichen Realitätscheck
    Eine umfangreiche Arbeit der Universität Jena ("ChemBench") hat KI-Modelle mit über 2.700 anspruchsvollen Aufgaben der modernen Chemie getestet. Das Ergebnis: KI ist in vielen Bereichen nicht mehr nur Hilfsmittel, sondern konkurriert auf dem Niveau von Fachleuten.
    
    ??? info "Mehr lesen"
        Besonders spannend für die Sekundarstufe II: Der Fokus der Chemie verschiebt sich spürbar von der reinen Vorhersage hin zum **gezielten Molekül- und Reaktionsdesign**. KI-Modelle wie **TopEC** können mittlerweile aus der Enzymstruktur direkt auf mögliche chemische Reaktionen schließen – ein Meilenstein für die Biokatalyse und synthetische Biologie.

    ---

    ### Frühjahr 2026 — Automatisierte Labore (Self-Driving Labs)
    KI wird zunehmend mit automatisierten Laboren gekoppelt. Methoden wie *Active Learning* und *Bayessche Optimierung* reduzieren nicht nur den Rechenaufwand, sondern steuern experimentelle Reihenfolgen, Parameterwahl und Prioritäten völlig eigenständig.
    
    ??? info "Mehr lesen"
        Die KI übernimmt den klassischen Labor-Workflow: Sie schlägt Strukturmotive vor, bewertet die Reaktionsfähigkeit und wählt nur die vielversprechendsten Kandidaten für den Syntheseroboter aus. Das senkt Kosten, spart Zeit und ersetzt den klassischen "Trial-and-Error"-Ansatz. Ein starker Diskussionspunkt für die Schule: Wie verändert sich das Berufsbild von ChemikerInnen?

    ---

    ### 17.03.2026 — AlphaFold-Datenbank jetzt auch mit Proteinpaaren
    Die AlphaFold-Datenbank umfasst inzwischen nicht nur Einzelproteine, sondern auch **Homodimere**. Damit wird KI für Biochemie und Molekularbiologie deutlich biologisch relevanter.

    ??? info "Mehr lesen"
        Bisher stand meist die Struktur einzelner Proteine im Mittelpunkt. Mit der Erweiterung auf **Proteinpaarungen** rückt jetzt stärker in den Fokus, wie Proteine zusammenwirken (Rezeptorbindung, Signalübertragung). Das belegt, dass KI zunehmend **biologisch funktionelle Zusammenhänge** erschließt.

    ---

    ### 29.01.2026 — KI hilft bei der Planung neuer chemischer Synthesen
    Ein Nature-Bericht zeigt ein KI-System mit chemischer Fachlogik, das zur Synthese **35 neuer Verbindungen** beigetragen hat. KI wird damit in der Chemie zunehmend zu einem Werkzeug für **echte Forschungsplanung**.

    ??? info "Mehr lesen"
        Für den Chemieunterricht ist das ein starker Perspektivwechsel: KI ist nicht nur ein Textwerkzeug, sondern kann Reaktionswissen, Synthesestrategie und Planung unterstützen. Das zeigt, dass KI in der Chemie **materiell wirksam** wird.

=== "Tools & Praxis"

    ### Der Siegeszug der Multimodalität
    Modelle wie ChatGPT-4o oder Gemini Advanced sind zu echten Experten der Bildanalyse gereift.
    
    ??? tip "Praxis-Anwendung: Spektren und Diagramme"
        Während frühere KIs bei komplexen Abbildungen oft rieten, können die aktuellen Modelle nun Titrationskurven, Phasendiagramme oder Spektren aus alten Lehrbüchern präzise auslesen und in skalierbare Vektorgrafiken (SVG) oder Excel-Wertetabellen übersetzen.

    ---

    ### "Single-File-Coding" als neuer Standard
    Funktionen wie **"Artifacts"** revolutionieren die Erstellung von Lehrmaterial. Die KI generiert nicht mehr nur passiven Code, sondern liefert direkt im Browser voll funktionsfähige, interaktive HTML-Simulationen.
    
    ??? info "Mehrwert für den Unterricht"
        Lehrkräfte ohne Programmierkenntnisse können maßgeschneiderte, interaktive Apps (wie den Gleichungstrainer) für ihre Klassen prompten. Da diese Apps lokal im Browser laufen, ist zudem maximaler Datenschutz gewährleistet.

    ---

    ### NotebookLM: Sicherer Hafen für Fachtexte
    Google NotebookLM hat sich als eines der sichersten Tools für den Unterricht etabliert, da es **ausschließlich** auf hochgeladenen Dokumenten (Skripte, Sicherheitsdatenblätter) basiert. "Halluzinationen" von chemischen Fakten sind damit praktisch ausgeschlossen.
    
    ??? success "Audio-Overviews (Podcast-Funktion)"
        Eine faszinierende Funktion ist die Möglichkeit, aus trockenen Fachtexten auf Knopfdruck einen dynamischen, KI-generierten Audio-Dialog erstellen zu lassen – ein hervorragendes Mittel zur Binnendifferenzierung.

=== "Schule & Didaktik"

    ### Frühjahr 2026 — KI-Offloading und die "Illusion des Lernens"
    Die Debatte, ob KI im Unterricht schlichtweg erlaubt oder verboten werden sollte, verfehlt das Ziel [cite: 11]. Die entscheidende Frage ist, *wie* und *wo* im Lernprozess KI platziert wird [cite: 11, 503]. Werden kognitive Anstrengungen vollständig an die KI ausgelagert ("Cognitive Offloading" [cite: 449]), riskieren Lernende eine gefährliche "Illusion des Lernens" [cite: 56], die bei ungestützten Aufgaben unweigerlich zusammenbricht [cite: 52, 56, 455].

    ??? info "Mehr lesen"
        **Fähigkeiten vs. Grundintelligenz**
        KI wird uns voraussichtlich nicht die kognitiven Grundfähigkeiten rauben [cite: 459, 477, 479], führt aber bei vollständigem Auslagern von Übungen zum Verfall spezifischer Kompetenzen (Skill Decay) [cite: 457, 461, 469, 470]. 

        **Das 6-Schritte-Modell des Lernens & der KI-Einsatz**
        Um diesen Verfall zu verhindern, muss KI gezielt und wohlüberlegt in den sechs Phasen des Lernens eingesetzt werden [cite: 84, 671]:
        * **⛔ KI-Freie Zonen:** Die Phasen **Probe** (erster eigener Lösungsversuch ohne Hilfe [cite: 88, 675]) und **Test** (ungestützte Leistungsüberprüfung [cite: 152, 739]) müssen KI-frei bleiben [cite: 85, 672]. Das Scheitern und Suchen ist hier der eigentliche Lernbeginn [cite: 89, 90, 676, 677].
        * **🟡 Zonen für geführte KI:** In Phasen wie **Prime** (Vorwissen wecken [cite: 86, 190]), **Point** (sokratische Hinweise [cite: 92, 191]), **Attach** (Lösungsbeispiel zur rechten Zeit [cite: 95, 194]) und **Strengthen** (skalierte Übung & Feedback [cite: 98, 200]) kann KI effektiv unterstützen, solange sie niemals die fertige Lösung liefert [cite: 172, 191, 512, 513].

        **Die universelle Leitregel für den Unterricht:**
        > *"Wenn der Einsatz von KI dazu führt, dass sich eine Aufgabe mühelos anfühlt, ist sie an der falschen Stelle platziert."* [cite: 165, 752]

        Mühelosigkeit ist ein Warnsignal [cite: 166, 753]. Bleiben die Lernenden durch interaktive Nutzung (z. B. als sokratischer Tutor) gezwungen, kognitiv mitzuarbeiten ("in the cognitive loop"), können die Risiken minimiert und der Kompetenzerwerb maßgeblich gefördert werden [cite: 524, 1111].

        *(Basierend auf: Brcic & Frljic, 2026, "The Effortless Trap" [cite: 2, 3, 5, 6] & Cash et al., 2026, "Is AI making us stupid?" [cite: 437, 440, 442])*

    ---

    ### Frühjahr 2026 — KI-Textzusammenfasser: Produktivitäts-Booster oder Lernfalle?
    Generative KI-Tools, die lange Fachtexte auf Knopfdruck zusammenfassen, erfreuen sich enormer Beliebtheit. Ein aktueller Weckruf von Corbin & Walton (2025) warnt jedoch vor den tiefgreifenden Folgen dieses Werkzeugs beim Lesen und fordert eine kritische Auseinandersetzung mit dem Verlust der eigenständigen Textarbeit.
    
    ??? info "Mehr lesen"
        **Das trügerische Versprechen:** Tools wie ChatGPT oder dedizierte PDF-Reader versprechen, stundenlanges Lesen überflüssig zu machen. Es werden leicht verdauliche Zusammenfassungen generiert, für die kein Vorwissen mehr nötig ist.
        
        **Eingriff in den Lernprozess:** Das Lesen komplexer Primärtexte ist nicht nur reiner Informationskonsum, sondern das Fundament für kritisches Denken und das Verstehen wissenschaftlicher Methodik. Nimmt die KI diese Hürden weg, entfällt das wichtige *Scaffolded Learning* (das schrittweise Erarbeiten von Komplexität).
        
        **Fazit für die Schule:** Dies ist ein exzellentes Praxisbeispiel für die **Mühelosigkeits-Falle**. Wenn eine KI den Text zusammenfasst, lagert der Lernende den entscheidenden kognitiven Schritt – das Bewerten und Strukturieren – vollständig an die Maschine aus. Solche Tools sollten daher erst *nach* der eigenen Auseinandersetzung mit dem Originaltext als Abgleich genutzt werden.

    ---

    ### 19.01.2026 — OECD: Generative KI wirkt nur mit klarer didaktischer Führung
    Der *OECD Digital Education Outlook 2026* betont, dass generative KI im Lernen dann nützlich wird, wenn sie **didaktisch geführt und strukturiert** eingesetzt wird. Freies „Herumprobieren“ reicht nicht.

    ??? info "Mehr lesen"
        Das stützt sehr deutlich einen Ansatz wie diesen Onlinekurs: KI sollte in **klaren fachlichen Workflows** eingebettet sein. Für Chemie und Biologie heißt das: strukturierte Aufgaben, erkennbare Modelle, fachliche Reflexion und kritische Auswertung. 

    ---

    ### 2026 — UNESCO: Lehrkräfte brauchen definierte KI-Kompetenzen
    UNESCO beschreibt im **AI Competency Framework for Teachers** 15 KI-Kompetenzen in fünf Bereichen (Grundlagenwissen, Pädagogik, Ethik, etc.).

    ??? info "Mehr lesen"
        Lehrkräfte sollen KI nicht nur bedienen können, sondern auch **fachlich einbetten, kritisch bewerten und verantwortungsvoll einsetzen**. 

    ---

    ### 2025/2026 — Chemiedidaktik & KI-Ethik im Fokus
    Aktuelle Übersichten zeigen, dass KI in der Science Education zunehmend systematisch als Thema von **AI literacy, Differenzierung und Fachlernen** betrachtet wird.
    
    > *"Der Computer oder andere digitale Medien sollen und dürfen das reale Experiment nicht ersetzen. KI ist unser Assistent bei der Vorbereitung und Auswertung, nicht der Ersatz für das naturwissenschaftliche Begreifen."*
    > — E. Kerzendorfer

    ??? info "Mehr lesen"
        Der Fokus verlagert sich vom "Finden der Antwort" hin zum **kritischen Beurteilen** der KI-Ergebnisse. Geführte Workflows und ständige Reflexion entsprechen exakt dem, was in der aktuellen Literatur gefordert wird.

=== "Kurzfazit"

    Zusammenfassend verändert KI die Naturwissenschaften gerade in **drei zentralen Rollen**:

    1. **Als Prädiktor:** KI macht Unsichtbares sichtbar (z. B. Proteinstrukturen, Molekülenergien, Rezeptorbindung).
    2. **Als Optimierer:** KI steuert Versuchsplanungen in automatisierten Laboren und wertet komplexe Messdaten rasant aus.
    3. **Als Entwurfssystem:** KI geht vom Vorhersagen zum aktiven Design über (neue Verbindungen, maßgeschneiderte Enzyme, zielgerichtete Medikamente).

    ??? tip "Didaktische Quintessenz"
        Für den Unterricht ist KI vor allem dann sinnvoll, wenn sie **fachlich geführt** wird. Die besten Resultate entstehen aus der Kombination von chemischem Domänenwissen und KI-gestützter Optimierung, anstatt sich auf einen reinen „Black-Box“-Ansatz zu verlassen. Die wissenschaftliche Validierung (das reale Experiment) bleibt unverzichtbar.
NAWI_KI_aktuell_V3.md
NAWI_KI_aktuell_V3.md wird angezeigt.
