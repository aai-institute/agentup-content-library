---
# source: f2e7391e7233a36a
id: mission-1-see-which-skills-your-ai-already-has
number: 1
title: Finde die Skills, die deine KI schon hat
summary: Finde die Skills, die deine KI-App mitbringt, sieh, wie deine KI einen davon liest, und rufe einen beim Namen oder mit einer passenden Anfrage auf, wenn eine Aufgabe passt.
artefact: keins
---

Track: Integrating Agents
Level: foundation
Time: 20 Minuten
Tools: Claude (Desktop-App oder claude.ai), die ChatGPT-Desktop-App oder die Gemini-App (Mac-App oder gemini.google.com)
Artefact kind: none
Artefact file: none

## Context
Du **erklärst deiner KI dieselben Aufgaben** immer wieder, dabei hat deine App für einige davon schon **fertige Schritte**. In dieser Mission findest du diese Schritte, siehst, wie deine KI einen Skill liest, und rufst einen auf, einen Schritt nach dem anderen.

## Your task
Finde die **fertigen [[Skills|Agent-Skill]]** in deiner KI-App, lies einen davon und **rufe einen auf zwei Wegen auf**: beim Namen und mit einer einfachen Anfrage, die zu dem passt, wofür der Skill gedacht ist.

## After this, you can
Zeige, wo deine App ihre Skills auflistet, und rufe einen Skill beim Namen und mit einer einfachen Anfrage auf.

## You need
- **Claude** (Desktop-App oder claude.ai), bei dem **Create and edit files** unter **Settings**, **Capabilities** eingeschaltet ist
- oder die **ChatGPT-Desktop-App** mit einem Business-, Enterprise-, Healthcare- oder Edu-Tarif
- oder die **Gemini-App** (Mac-App oder gemini.google.com), wenn du mindestens 18 Jahre alt bist und **Keep Activity** eingeschaltet hast
- Einen **Browser**

## You should already
- Einen **neuen Chat** in deiner KI-App **starten**
- Die **Einstellungen oder die Seitenleiste** deiner App finden
- Eine **Webseite durchsuchen**, mit **Cmd+F** (Mac) oder **Ctrl+F** (Windows)

## Concept
Heading: Was ein Skill enthält und was die KI wann liest
Lead: Ein **Skill** ist ein Ordner mit einer Datei `SKILL.md`, wie dieser ausgedachte Skill **meeting-agenda**.
- [[Kopfbereich]]: die Zeilen zwischen zwei `---`-Zeilen ganz oben in `SKILL.md`, in denen Name und Beschreibung stehen.
- Name: eine kurze Bezeichnung für den Skill, etwa `meeting-agenda`.
- [[Beschreibung]]: was der Skill tut und wann er verwendet wird, etwa „Macht aus einer Liste von Themen eine einseitige Meeting-Agenda. Verwenden, wenn jemand eine Agenda anfragt oder ein Meeting vorbereiten will.“
- Schritte: die Anweisungen, denen die KI folgt, nach dem Kopfbereich, etwa „1. Frage nach Datum, Uhrzeit und Dauer des Meetings, falls sie fehlen. 2. Gib jedem Thema ein Zeitfenster und eine verantwortliche Person.“
- Weitere Dateien: andere Dateien im Ordner, die die KI nur liest, wenn die Schritte sie dorthin schicken.
Close: Zu Beginn eines Chats sieht die KI von jedem eingeschalteten Skill nur den Namen und die Beschreibung. Die Schritte liest sie, wenn die Beschreibung zu deiner Anfrage passt, und weitere Dateien nur, wenn die Schritte auf diese Dateien verweisen.
Toggle: Warum sagt die Beschreibung, wann der Skill verwendet wird? | Zu Beginn eines Chats sind Name und Beschreibung alles, was die KI von einem Skill sieht. Deine Anfrage muss zur Beschreibung passen, bevor die KI die Schritte liest. Deshalb entscheidet der Teil „wann verwenden“, ob der Skill zum Einsatz kommt.

## Check your understanding
Question: Der Skill meeting-agenda ist eingeschaltet. In einem neuen Chat schreibst du „Übersetze diese E-Mail ins Englische.“ Was glaubst du, was liest die KI vom Skill meeting-agenda?
- A: Nur den Namen und die Beschreibung, weil die Anfrage nicht zur Beschreibung passt
- B: Die ganze Datei samt Schritten, weil jeder eingeschaltete Skill zu Beginn eines Chats vollständig gelesen wird
- C: Gar nichts, weil du den Skill nicht beim Namen genannt hast
- D: Die Schritte und jede weitere Datei im Ordner des Skills
Answer: A
Why: Die KI sieht zu Beginn eines Chats Namen und Beschreibung jedes eingeschalteten Skills und liest die Schritte nur, wenn die Beschreibung zur Anfrage passt. Eine Übersetzungsanfrage passt nicht zu „Verwenden, wenn jemand eine Agenda anfragt oder ein Meeting vorbereiten will“, also bleiben die Schritte ungelesen. B liegt nahe, weil der Skill eingeschaltet ist, aber das Einschalten bringt nur Name und Beschreibung vor die KI. C liegt nahe, weil das Nennen des Namens tatsächlich dafür sorgt, dass die KI den Skill verwendet, aber Name und Beschreibung sind auch da, wenn du den Skill nicht nennst. D bringt die Reihenfolge durcheinander: Weitere Dateien kommen zuletzt, und nur, wenn die Schritte die KI dorthin schicken.

## Working example
Situation: Du möchtest ein einseitiges PDF der Agenda für ein Teammeeting, eine Aufgabe, zu der einer der fertigen Skills deiner App passt. Du kannst stattdessen auch eine Aufgabe aus deiner eigenen Woche nehmen.
Input: Eine ausgedachte Agenda für ein Teammeeting am Donnerstag, 10:00 bis 11:00 Uhr, mit drei Themen.
- Die KI sieht Name und Beschreibung jedes eingeschalteten Skills.
- Deine Anfrage „Erstelle ein einseitiges PDF dieser Agenda“ passt zur Beschreibung des PDF-Skills.
- Die KI liest die Schritte des PDF-Skills.
- Die KI folgt diesen Schritten und erstellt das PDF.
Result: Ein einseitiges PDF der Agenda, erstellt nach den Schritten des Skills statt nach deiner Erklärung.

## Steps
### Einen echten Skill lesen
Why: Die KI entscheidet anhand der **Beschreibung**, ob sie die Schritte eines Skills liest. Deshalb suchst du bei jedem Skill zuerst nach dem Teil „wann verwenden“.
Do:
1. Öffne Anthropics Skill **pdf** in deinem Browser: [raw.githubusercontent.com/anthropics/skills/main/skills/pdf/SKILL.md](https://raw.githubusercontent.com/anthropics/skills/main/skills/pdf/SKILL.md).
2. Überspring den Python-Code: Du liest diese Datei nur.
3. Drücke **Cmd+F** (Mac) oder **Ctrl+F** (Windows) und suche die Zeile `description` im Kopfbereich.
4. Suche die Überschrift `Quick Start`, dort beginnen die Schritte.
5. Suche die Zeile, in der `FORMS.md` vorkommt.
Ask: Wann sollte die KI den pdf-Skill verwenden, in deinen eigenen Worten?

### Die fertigen Skills in deiner App finden
Why: Die Skill-Liste deiner App zeigt, welche fertigen Skills **eingeschaltet** sind, und nur diese Skills erreichen die KI zu Beginn eines Chats.
Do:
1. Öffne in Claude **Customize** und dann **Skills**.
2. Sieh dir Anthropics eigene Skills für Excel, Word, PowerPoint und PDF an.
3. Prüfe, ob der Schalter beim Skill **PDF** eingeschaltet ist.
4. Öffne einen Skill, der zu einer Aufgabe aus deiner Woche passt, und suche in seiner Beschreibung den Teil „wann verwenden“.
Ask: Welche fertigen Skills hast du gefunden, und wie lautet der Teil „wann verwenden“ bei deinem gewählten Skill?

### Die fertigen Skills in deiner App finden [chatgpt]
Why: Die Skill-Liste deiner App zeigt, welche fertigen Skills **eingeschaltet** sind, und nur diese Skills erreichen die KI zu Beginn eines Chats.
Do:
1. Wähle in der ChatGPT-Desktop-App in der Seitenleiste **Plugins** und dann den Tab **Skills**. Wenn deine Seitenleiste stattdessen **Skills** zeigt, öffne diesen Eintrag.
2. Sieh dir die fertigen Skills an, etwa **skill-creator**.
3. Wenn du keine Skills findest, aktualisiere die App und starte sie neu. Fehlen die Skills dann noch immer, frag die Admins deines Workspace, ob dein Tarif Skills enthält.
4. Öffne einen Skill, der zu einer Aufgabe aus deiner Woche passt, und suche in seiner Beschreibung den Teil „wann verwenden“.
Ask: Welche fertigen Skills hast du gefunden, und wie lautet der Teil „wann verwenden“ bei deinem gewählten Skill?

### Die fertigen Skills in deiner App finden [gemini]
Why: Die Skill-Liste deiner App zeigt, welche fertigen Skills **eingeschaltet** sind, und nur diese Skills erreichen die KI zu Beginn eines Chats.
Do:
1. Öffne in der Gemini-App **Customize** und dann **Skills**. Wenn du **Customize** nicht siehst, öffne zuerst **More**.
2. Sieh unter **Recommended** nach, dort hält Gemini seine fertigen Skills als Vorlagen bereit.
3. Klicke auf eine Vorlage, die zu einer Aufgabe aus deiner Woche passt, um sie zu verwenden.
4. Lies ihre **Description** und **Instructions** und suche den Teil „wann verwenden“.
Ask: Welche fertigen Skills hast du gefunden, und wie lautet der Teil „wann verwenden“ bei deinem gewählten Skill?

### Den Skill beim Namen aufrufen
Use: Eine Aufgabe aus deiner Woche, zu der dein gewählter Skill passt, oder die ausgedachte Agenda für den PDF-Skill.
Why: Wenn du einen Skill **beim Namen** aufrufst, sorgst du dafür, dass die KI ihn verwendet, und du siehst, was seine Schritte ergeben.
Do:
1. Starte einen **neuen Chat** in Claude.
2. Schreib „Nutze den Skill [Name]“ und danach deine Anfrage. Für den PDF-Skill kannst du die ausgedachte Agenda-Anfrage aus dem Codeblock kopieren.
3. Sende die Anfrage und vergleiche die Ausgabe mit den Schritten des Skills.
Code:
```text
Nutze den PDF-Skill. Erstelle ein einseitiges PDF dieser Agenda:
Teammeeting, Donnerstag 10:00 bis 11:00
1. Projekt Falcon: Starttermin Standort 2
2. Neuzugang Mira: Plan für die erste Woche
3. Datenexport: Wer ist verantwortlich?
```
Ask: Welche Schritte des Skills erkennst du in der Ausgabe?

### Den Skill beim Namen aufrufen [chatgpt]
Use: Eine Aufgabe aus deiner Woche, zu der dein gewählter Skill passt.
Why: Wenn du einen Skill **beim Namen** aufrufst, sorgst du dafür, dass die KI ihn verwendet, und du siehst, was seine Schritte ergeben.
Do:
1. Starte einen **neuen Chat** in der ChatGPT-Desktop-App.
2. Tippe `@` und wähle deinen Skill.
3. Ergänze deine Anfrage und sende sie.
4. Vergleiche die Ausgabe mit den Schritten des Skills.
Ask: Welche Schritte des Skills erkennst du in der Ausgabe?

### Den Skill beim Namen aufrufen [gemini]
Use: Eine Aufgabe aus deiner Woche, zu der dein gewählter Skill passt.
Why: Wenn du einen Skill **beim Namen** aufrufst, sorgst du dafür, dass die KI ihn verwendet, und du siehst, was seine Schritte ergeben.
Do:
1. Starte einen **neuen Chat** in der Gemini-App.
2. Tippe `/` oder `@` und wähle deinen Skill.
3. Ergänze deine Anfrage und sende sie.
4. Vergleiche die Ausgabe mit den Schritten des Skills.
Ask: Welche Schritte des Skills erkennst du in der Ausgabe?

## Trust check
Watch for:
- Beim Lesen der Datei des pdf-Skills im Browser: Lies den Kopfbereich und die Schritte und lass den Python-Code beiseite.
- Wenn du in Gemini einen empfohlenen Skill verwendest, kommt er zu deinen Skills dazu: Um ihn später zu entfernen, öffne **More** und dann **Deactivate** oder **Delete**.
- Bei der Wahl des Materials für deine Anfrage: Nimm eine Aufgabe, die du in diese KI-App eingeben darfst, oder die ausgedachte Agenda.
Ask: Darfst du das Material, das du mit dem Skill verwendest, in diese KI-App eingeben, oder nimmst du die ausgedachte Agenda?

## Test
Do:
1. Starte noch einen **neuen Chat**.
2. Schreib dieselbe Anfrage ohne den Namen des Skills, in Worten, die zu seiner Beschreibung passen, etwa „Erstelle ein einseitiges PDF dieser Agenda“ und danach die Agenda.
3. Notiere vor dem Senden, ob du erwartest, dass die KI den Skill verwendet.
4. Sende die Anfrage und suche in der Ausgabe nach den Schritten des Skills.
Check:
- Die Ausgabe zeigt dieselben Schritte wie beim Aufruf des Skills beim Namen.
- Was passiert ist, stimmt mit dem überein, was du vor dem Senden erwartet hast.
Ask: Was hast du erwartet, und was kam diesmal heraus?

## Done when
- Du kannst zeigen, wo deine App ihre fertigen Skills auflistet, und auf den Teil „wann verwenden“ einer Beschreibung zeigen.
- Du hast einen Skill beim Namen und mit einer passenden Anfrage aufgerufen und jede Ausgabe mit den Schritten des Skills verglichen.

## Practice
- Öffne einen anderen fertigen Skill in deiner App, lies seinen Teil „wann verwenden“ und rufe ihn beim Namen mit einer kleinen Aufgabe aus deiner Woche auf.
- Schreib für einen fertigen Skill eine Anfrage, die zu seiner Beschreibung passt, und eine, die nicht passt, und sende jede in einem neuen Chat.
- Wenn du das nächste Mal anfängst, deiner KI eine Aufgabe zu erklären, such in deiner Skill-Liste nach einer passenden Beschreibung und rufe stattdessen diesen Skill auf.

## Glossary
- Agent-Skill: ein Ordner mit einer Datei `SKILL.md`, in der ein Name, eine Beschreibung und die Schritte stehen, denen die KI bei einer Aufgabe folgt.
- Kopfbereich: die Zeilen zwischen zwei `---`-Zeilen ganz oben in `SKILL.md`, in denen Name und Beschreibung des Skills stehen.
- Beschreibung: die Zeile im Kopfbereich eines Skills, die sagt, was der Skill tut und wann er verwendet wird; die KI liest die Schritte nur, wenn eine Anfrage zu dieser Zeile passt.

## Sources
- [Agent Skills, Specification](https://agentskills.io/specification): das Format eines Skills und die Reihenfolge, in der die KI Name und Beschreibung, die Schritte und weitere Dateien liest.
- [Anthropic, Use skills in Claude, Claude Help Center](https://support.claude.com/en/articles/12512180-use-skills-in-claude): die Einstellung Create and edit files, wo Claude seine Skills auflistet, Anthropics eigene Skills und der Aufruf eines Skills beim Namen oder mit einer passenden Anfrage.
- [OpenAI, Build skills, ChatGPT documentation](https://learn.chatgpt.com/docs/build-skills): der Eintrag Skills in der Seitenleiste, der Aufruf eines Skills mit `@` und wie ChatGPT einen Skill wählt, wenn eine Anfrage zu seiner Beschreibung passt.
- [OpenAI, Skills in ChatGPT, OpenAI Help Center](https://help.openai.com/en/articles/20001066-skills-in-chatgpt): welche Tarife Skills enthalten, der Tab Plugins und Skills und der fertige skill-creator.
- [Google, Create & manage skills for Gemini Apps (Computer), Gemini Apps Help](https://support.google.com/gemini/answer/17094296?hl=en&co=GENIE.Platform%3DDesktop): Voraussetzungen, Customize und Skills, Vorlagen unter Recommended, der Aufruf mit `/` oder `@` und das Deaktivieren oder Löschen eines Skills.
- [Anthropic, skills, GitHub repository](https://github.com/anthropics/skills): der echte pdf-Skill, den die lernende Person liest.

Coach notes:

Arc of the mission: Die lernende Person lernt Skills von außen kennen, als fertige Schritte, die ihre App schon hat. Zuerst das Konzept (was ein Skill enthält und in welcher Reihenfolge die KI ihn liest), eine Verständnisfrage, dann drei Phasen am Laptop: einen echten Skill im Browser lesen, Skills in der eigenen App finden und einen beim Namen aufrufen. Der Test ist der zweite Aufruf, ohne den Namen. Die lernende Person kommt nach jeder Phase in den Chat zurück. Der Coach wartet ab, was die Person gesehen hat, beschreibt nie, was die App zeigen „wird“, und erledigt nie die Arbeit am Laptop für sie.

Check your understanding: Sprich die Wahl der lernenden Person anhand des Why durch. Hat sie B, C oder D gewählt, beginne mit dem, was daran stimmt (B: Eingeschaltet zu sein spielt eine Rolle; C: Das Nennen des Namens sorgt dafür, dass der Skill verwendet wird; D: Weitere Dateien gibt es tatsächlich), und erkläre dann die Lesereihenfolge.

Schritt 1, Einen echten Skill lesen. Abwarten: die eigenen Worte der lernenden Person dafür, wann der pdf-Skill verwendet werden sollte. Nachfragen, eine nach der anderen:
- Hast du die Überschrift `Quick Start` gefunden? Dort beginnen die Schritte.
- Was steht in der Zeile, in der `FORMS.md` vorkommt? Das ist eine weitere Datei, die die KI nur liest, wenn die Schritte sie dorthin schicken.
- Würde „Schreib diese Agenda als kurze E-Mail“ die KI dazu bringen, die Schritte des pdf-Skills zu lesen?
Merk dir die Antwort der lernenden Person auf die E-Mail-Frage: Der Test braucht sie vielleicht, und der Coach wiederholt sie ihr, statt sie zu bitten, sich daran zu erinnern. Verliert sich die Person im Python-Code, erinnere sie daran, nur nach `description`, `Quick Start` und `FORMS.md` zu suchen. Guided: eine Suche nach der anderen durchgehen. Fast-track: alle drei Fundstellen in einer Antwort erfragen.

Schritt 2, Die fertigen Skills finden. Abwarten: die Liste der gefundenen Skills und der Teil „wann verwenden“ des gewählten Skills, dazu der Teil „wann nicht verwenden“, falls es einen gibt. Claude: Wenn Skills nicht erscheint, prüfen, ob Create and edit files unter Settings, Capabilities eingeschaltet ist. ChatGPT: Fehlt der Tab Skills, aktualisiert die lernende Person die App und startet sie neu; fehlt er dann noch immer, fragt sie die Admins ihres Workspace, ob ihr Tarif Skills enthält, und du kannst mit dem Leseteil weitermachen und den Aufruf später nachholen. Gemini: Die fertigen Skills sind Vorlagen unter Recommended; ein Klick fügt eine Vorlage hinzu, und über More, Deactivate oder Delete lässt sie sich später entfernen. Findet die lernende Person keinen Skill, der zu ihrer Woche passt, schlag den PDF-Skill mit der ausgedachten Agenda in Claude vor oder den am besten passenden Skill in ihrer App.

Schritt 3, Den Skill beim Namen aufrufen. Abwarten: welche Schritte des Skills die lernende Person in der Ausgabe erkennt. Hilf ihr, die in der Ausgabe sichtbaren Schritte mit den Schritten im Skill zu verbinden. Bleib bei dem, was die Ausgabe zeigt: Sie deutet darauf hin, dass der Skill verwendet wurde, beweist aber nicht, was in der App passiert ist.

Test. Gib Lernenden, die die ausgedachte Agenda verwenden, diesen Text zum Kopieren:
```text
Erstelle ein einseitiges PDF dieser Agenda:
Teammeeting, Donnerstag 10:00 bis 11:00
1. Projekt Falcon: Starttermin Standort 2
2. Neuzugang Mira: Plan für die erste Woche
3. Datenexport: Wer ist verantwortlich?
```
Bei einer eigenen Aufgabe hilf der lernenden Person, die Anfrage mit den Worten aus dem Teil „wann verwenden“ der Beschreibung zu formulieren, ohne den Namen des Skills. Abwarten: ihre Vorhersage und was herauskam. Dann den passenden Zweig wählen:
- Es sieht so aus, als hätte die KI den Skill beide Male verwendet: Wiederhole die frühere Antwort der lernenden Person zur E-Mail-Anfrage, gib ihr „Schreib diese Agenda als kurze E-Mail“ zum Senden in einem neuen Chat und frag, ob ihre Antwort noch stimmt.
- Ohne den Namen scheint die KI den Skill übergangen zu haben: Die lernende Person formuliert die Anfrage mit den Worten aus dem Teil „wann verwenden“ der Beschreibung um und versucht es in einem neuen Chat noch einmal. Übergeht die KI den Skill weiterhin, braucht diese Aufgabe den Namen, und die Person ruft den Skill ab jetzt beim Namen auf.
Erfinde nie einen Fehlschlag; auch nach einem erfolgreichen ersten Durchlauf kommt die E-Mail-Anfrage als zweiter Fall.

Tools: Claude ruft einen Skill beim Namen in der Anfrage auf („Nutze den Skill [Name]“), ChatGPT mit `@`, Gemini mit `/` oder `@`. Alle drei können selbst einen Skill wählen, wenn eine Anfrage zu seiner Beschreibung passt.

Levels: Guided-Lernende bekommen jede Aktion einzeln und jeden Grund erklärt. Standard-Lernende folgen der Seite. Fast-Track-Lernende können die Verständnisfrage überspringen, wenn sie schnell antworten, und die Beschreibungen zweier fertiger Skills in ihrer App vergleichen.

Time budget: Konzept und Verständnisfrage 3 Minuten, pdf-Skill lesen 3, Skills finden 5, Aufruf beim Namen 4, Test und zweiter Fall 5.

Review, at the end:
- Was du gemacht hast: Frag, welchen Skill die lernende Person aufgerufen hat und was passiert ist, als sie ihn genannt hat und als sie ihn nicht genannt hat. Fass nur zusammen, was sie berichtet hat.
- Was du dir merken kannst: Die KI liest nur Name und Beschreibung, bis eine Anfrage passt; dann liest sie die Schritte. Eine einfache Anfrage funktioniert, wenn deine Worte zur Beschreibung passen. Der Aufruf beim Namen sorgt dafür, dass die KI den Skill verwendet: in der Anfrage in Claude, mit `@` in ChatGPT, mit `/` oder `@` in Gemini.
- In einem Satz: Wenn eine Aufgabe das nächste Mal zu einem Skill passt, den deine App mitbringt, rufe den Skill auf, statt die Aufgabe noch einmal zu erklären.
