---
# source: 215e7b9453129f74
id: mission-2-install-the-humanizer-and-see-when-it-loads
number: 2
title: Humanizer installieren und sehen, wann er lädt
summary: Prüfe und installiere einen beliebten Skill, der deinen Entwürfen den KI-Klang nimmt, und teste, bei welchen Anfragen deine KI ihn nutzt. So weißt du, wie du ihn das nächste Mal ansprichst.
artefact: der Humanizer-Skill, installiert und getestet
---

Track: Integrating Agents
Level: foundation
Time: 20 Minuten
Tools: Claude in der Desktop-App oder auf claude.ai, die ChatGPT-Desktop-App oder Gemini in der Mac-App oder auf gemini.google.com
Artefact kind: text
Artefact file: SKILL.md

## Context
Du lässt KI **Newsletter, Posts oder E-Mails** entwerfen und korrigierst danach Formulierungen wie „ist nicht nur X, sondern Y“ von Hand. Der **Humanizer** ist ein Skill aus externer Quelle. Er schreibt einen Entwurf so um, dass er nicht mehr nach KI klingt, und behält bei, was der Entwurf aussagt. In dieser Mission prüfst du den Humanizer, installierst ihn und findest Schritt für Schritt heraus, **welche Anfragen** deine KI dazu bringen, ihn zu nutzen.

## Your task
**Prüfe und installiere** den Humanizer, teste, **welche Anfragen** deine KI dazu bringen, ihn zu nutzen, und wende ihn auf einen **Text an, der nach KI klingt**.

## After this, you can
Der Humanizer ist in deiner KI eingeschaltet. Du hast notiert, welche Anfragen deine KI dazu gebracht haben, ihn zu nutzen, und wie du ihn für einen Entwurf angefragt hast.

## You need
- **Claude** in der Desktop-App oder auf claude.ai, mit eingeschaltetem **Create and edit files** unter **Settings**, **Capabilities**. In einem Enterprise-Tarif muss zuerst ein Owner Skills freischalten.
- Die **GitHub-Seite** des Humanizers: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- Einen **von KI entworfenen Text** von dir, wenn deine Organisation ihn in dieser App erlaubt, oder den erfundenen Newsletter-Absatz aus dieser Mission.

## You need [chatgpt]
- Die **ChatGPT-Desktop-App** in einem Business-, Enterprise-, Healthcare- oder Edu-Tarif, wenn dein **Workspace Skills erlaubt**.
- Die **GitHub-Seite** des Humanizers: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- Einen **von KI entworfenen Text** von dir, wenn deine Organisation ihn in dieser App erlaubt, oder den erfundenen Newsletter-Absatz aus dieser Mission.

## You need [gemini]
- **Gemini** in der Mac-App oder auf gemini.google.com. Du musst mindestens 18 Jahre alt sein, und **Keep Activity** muss eingeschaltet sein.
- Die **GitHub-Seite** des Humanizers: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- Einen **von KI entworfenen Text** von dir, wenn deine Organisation ihn in dieser App erlaubt, oder den erfundenen Newsletter-Absatz aus dieser Mission.

## You should already
- Eine Datei von einer Website **herunterladen**.
- Einen Ordner **zippen**.
- Wissen, dass ein **Skill** ein Ordner mit einer Datei `SKILL.md` ist, die Namen, Beschreibung und Anweisungen des Skills enthält.

## You should already [chatgpt]
- Text von einer Website **kopieren**.
- Wissen, dass ein **Skill** ein Ordner mit einer Datei `SKILL.md` ist, die Namen, Beschreibung und Anweisungen des Skills enthält.

## You should already [gemini]
- Eine Datei von einer Website **herunterladen**.
- Wissen, dass ein **Skill** ein Ordner mit einer Datei `SKILL.md` ist, die Namen, Beschreibung und Anweisungen des Skills enthält.

## Concept
Heading: Wie deine KI entscheidet, einen Skill zu nutzen
Lead: In jedem Chat sieht deine KI von jedem Skill nur den **Namen** und die **[[Beschreibung|Beschreibung (des Skills)]]**. Die **Anweisungen** des Skills liest sie erst, wenn die Beschreibung zu deiner Anfrage passt.
- Name und Beschreibung: sind immer im Blick. Deshalb gleicht deine KI deine Anfrage mit der Beschreibung des Humanizers ab, die mit „Rewrite AI-sounding text so it reads like the writer without changing what it says“ beginnt (sinngemäß: Schreibe Text, der nach KI klingt, so um, dass er nach der schreibenden Person klingt, ohne zu ändern, was er aussagt).
- Anweisungen: werden nur gelesen, wenn die Beschreibung passt. Dann **[[lädt|Laden]]** der Skill.
- [[KI-Anzeichen]]: die Angewohnheiten, die die Beschreibung nennt, etwa „Das ist nicht nur ein Feature, das ist ein Wandel“ (nicht X, sondern Y), „Lass das mal sacken“ (einzeiliger Schlusssatz), „Und jetzt kommt's“ (inszenierter Einstieg) und „eintauchen“ (typisches KI-Wort).
Close: Deine KI sieht Name und Beschreibung von Anfang an und entscheidet in jedem Chat neu. Deshalb entscheiden die Worte deiner Anfrage, ob die Anweisungen des Humanizers laden.
Toggle: Was steht vollständig in der Beschreibung des Humanizers? | „Rewrite AI-sounding text so it reads like the writer without changing what it says. Use when editing or reviewing prose for AI tells: not-X-but-Y contrasts, one-line closers, staged openers, forced triads, dashes everywhere, inflated claims, sales language, stock AI words, bold labels, or filler. Based on Wikipedia's "Signs of AI writing."“ Sinngemäß: Schreibe Text, der nach KI klingt, so um, dass er nach der schreibenden Person klingt, ohne zu ändern, was er aussagt. Nutze den Skill, wenn du Texte auf KI-Anzeichen hin bearbeitest oder prüfst: Gegensätze nach dem Muster „nicht X, sondern Y“, einzeilige Schlusssätze, inszenierte Einstiege, erzwungene Dreierreihen, Gedankenstriche überall, aufgeblähte Behauptungen, Verkaufssprache, typische KI-Wörter, fette Labels oder Füllwörter. Beruht auf dem Wikipedia-Artikel „Signs of AI writing“.
Toggle: Warum liest die KI nicht in jedem Chat die Anweisungen aller Skills? | Deine KI behält von jedem Skill nur Namen und Beschreibung im Blick und liest die Anweisungen, wenn sie passen. Die Entscheidung hängt deshalb an der Beschreibung.

## Check your understanding
Question: Der Humanizer ist eingeschaltet, und du fragst „Fasse diese E-Mail in einem Satz zusammen“. Was glaubst du, macht deine KI mit dem Humanizer?
- A: Sie sieht Namen und Beschreibung des Humanizers und lässt die Anweisungen sehr wahrscheinlich ungelesen, weil das Zusammenfassen einer E-Mail nicht zur Beschreibung passt.
- B: Sie liest vor jeder Antwort die Anweisungen aller eingeschalteten Skills, also auch die des Humanizers.
- C: Sie wendet den Humanizer auf die Zusammenfassung an, weil der Skill eingeschaltet ist.
- D: Sie kann den Humanizer gar nicht sehen, wenn du den Skill nicht in deiner Anfrage nennst.
Answer: A
Why: Deine KI sieht in jedem Chat nur Namen und Beschreibung jedes Skills und liest die Anweisungen erst, wenn die Beschreibung zur Anfrage passt. Eine E-Mail in einem Satz zusammenzufassen heißt nicht, einen Text auf KI-Anzeichen hin zu bearbeiten oder zu prüfen. B liegt nahe, weil sich ein eingeschalteter Skill „aktiv“ anfühlt, aber die Anweisungen werden nur gelesen, wenn die Beschreibung passt. C verwechselt „eingeschaltet“ mit „genutzt“: Das Einschalten bringt die Beschreibung in den Blick, und die Anfrage entscheidet trotzdem. D hat einen wahren Kern, denn den Skill zu nennen ist ein Weg, ihn anzufragen. Die Beschreibung ist aber auch ohne Nennung im Blick.

## Working example
Situation: Du lässt KI einen Newsletter-Absatz entwerfen und korrigierst dann vor dem Versand Formulierungen wie „ist nicht nur X, sondern Y“ von Hand.
Input: Die `SKILL.md` des Humanizers auf GitHub, drei erfundene Testanfragen und der erfundene Newsletter-Absatz.
- Du liest die `SKILL.md` des Humanizers und installierst den Skill in deiner KI.
- Du schickst drei Anfragen, jede in einem eigenen neuen Chat, und deine KI entscheidet anhand der Beschreibung, ob sie den Humanizer lädt.
- Wenn der Humanizer lädt, antwortet deine KI mit einem Entwurf, einer kurzen Liste verbliebener KI-Muster und einer endgültigen Überarbeitung.
- Du fragst den Humanizer für einen Entwurf mit Worten an, die ihn geladen haben, und prüfst Namen, Daten und Zahlen.
Result: Der Humanizer ist eingeschaltet, du hast notiert, welche Anfragen ihn geladen haben, und ein Entwurf klingt weniger nach KI, mit unveränderten Fakten.

## Steps
### Lies den Humanizer vor der Installation
Why: Ein Skill handelt mit den **Zugriffsrechten** deiner KI. Ein Schritt in seinen Anweisungen, der Links öffnet, Dateien verschickt oder Programme ausführt, würde das also mit deinen Zugriffsrechten tun. Wenn du zuerst die `SKILL.md` liest, siehst du, was du einschaltest.
Do:
1. Öffne [github.com/blader/humanizer](https://github.com/blader/humanizer) und klicke auf **SKILL.md**.
2. Klicke auf **Raw**, um den reinen Text zu sehen.
3. Lies den Teil mit der Überschrift *How to work*: Prüfe, dass er keine Schritte enthält, die Links öffnen, Dateien verschicken oder Programme ausführen.
4. Suche auf der Seite mit **Cmd+F** oder **Ctrl+F** nach `http`: Der einzige Link sollte der zu Wikipedia sein.
5. Andere Links oder solche Schritte gefunden? Frag im Chat nach, bevor du installierst. Du entscheidest, ob du den Skill installierst.

### Installiere den Humanizer
Why: Durch die Installation sind **Name und Beschreibung** des Humanizers in jedem Chat im Blick. Wenn du danach die Beschreibung prüfst, siehst du, dass sie **unverändert** angekommen ist.
Do:
1. Klicke zurück auf der Seite der `SKILL.md` auf **Download raw file** (das Download-Symbol).
2. Prüfe, dass die Datei `SKILL.md` heißt, lege sie in einen neuen Ordner namens `humanizer` und zippe den Ordner.
3. Gehe in Claude zu **Customize**, **Skills**, **+**, **Create skill**, **Upload a skill** und wähle die ZIP-Datei.
4. Suche den Humanizer in deiner Skill-Liste und prüfe, dass sein Schalter eingeschaltet ist.
5. Prüfe, dass die Beschreibung noch mit „Rewrite AI-sounding text“ beginnt.
Ask: Was hast du beim Lesen der `SKILL.md` gefunden, und beginnt die Beschreibung in deiner Skill-Liste genauso?

### Installiere den Humanizer [chatgpt]
Why: Durch die Installation sind **Name und Beschreibung** des Humanizers in jedem Chat im Blick. Wenn du danach die Beschreibung prüfst, siehst du, dass sie **unverändert** angekommen ist.
Do:
1. Kopiere auf der **Raw**-Seite der `SKILL.md` den gesamten Text.
2. Stelle in der ChatGPT-Desktop-App das Eingabefeld auf **Work** um.
3. Tippe `@skill-creator` und schicke dann die Anfrage aus dem Codeblock, mit dem kopierten Text dahinter eingefügt.
4. Gehe zu **Plugins**, **Skills**, **Created by me** und suche den Humanizer.
5. Prüfe, dass die Beschreibung noch mit „Rewrite AI-sounding text“ beginnt. Hat sie sich geändert? Bitte skill-creator, das Original zu behalten.
Code:
```text
Erstelle einen Skill aus genau dieser SKILL.md, unverändert. Er braucht keine Skripte.
```
Ask: Was hast du beim Lesen der `SKILL.md` gefunden, und beginnt die Beschreibung in deiner Skill-Liste genauso?

### Installiere den Humanizer [gemini]
Why: Durch die Installation sind **Name und Beschreibung** des Humanizers in jedem Chat im Blick. Wenn du danach die Beschreibung prüfst, siehst du, dass sie **unverändert** angekommen ist.
Do:
1. Klicke zurück auf der Seite der `SKILL.md` auf **Download raw file** (das Download-Symbol) und prüfe, dass die Datei `SKILL.md` heißt.
2. Gehe in Gemini zu **Customize** (unter **More**, falls ausgeblendet), **Skills**, **Create**, **Upload**.
3. Wähle die Datei und klicke auf **Create**.
4. Suche den Humanizer in deiner Skill-Liste: Zeigt **More** den Eintrag **Deactivate**, ist er aktiv.
5. Prüfe, dass die Beschreibung noch mit „Rewrite AI-sounding text“ beginnt.
Ask: Was hast du beim Lesen der `SKILL.md` gefunden, und beginnt die Beschreibung in deiner Skill-Liste genauso?

### Teste, welche Anfragen ihn laden
Why: Deine KI entscheidet **in jedem Chat neu**, ob eine Anfrage zur Beschreibung passt. Deshalb kommt jede Anfrage in einen eigenen neuen Chat, und eine Anfrage schickst du zweimal, um zu sehen, ob die Entscheidung gleich bleibt.
Do:
1. Notiere, welche der drei erfundenen Anfragen den Humanizer deiner Meinung nach laden: die Garten-Anfrage, die E-Mail-Anfrage und die Newsletter-Anfrage.
2. Schicke jede Anfrage in einem eigenen neuen Chat.
3. Schicke die Newsletter-Anfrage oder eine überraschende eigene Anfrage noch einmal in einem neuen Chat.
4. Überfliege jede Antwort: Ein Entwurf, eine kurze Liste verbliebener KI-Muster und eine endgültige Überarbeitung bedeuten, dass der Humanizer geladen hat. Eine einzelne Überarbeitung bedeutet, dass er sehr wahrscheinlich nicht geladen hat.
5. Prüfe in den Überarbeitungen der Garten-Anfrage, dass Name, Datum und Zahlen erhalten geblieben sind.
Code:
```text
Lass das hier weniger nach KI klingen:
Ich freue mich riesig, euch mitzuteilen: Unser Garten ist nicht nur Erde, er ist eine Bewegung. Am 21. November pflanzen Jonas Weber und 12 Freiwillige 40 Bäume. Lass das mal sacken.

Fasse diese E-Mail in einem Satz zusammen:
Das Büro ist am 31. Okt. geschlossen.

Überarbeite diesen Absatz für unseren Newsletter:
Wir freuen uns sehr, bekannt zu geben, dass Mira als Projektleitung zu uns kommt. Ihr Weg ist ein Beweis für die Kraft des Ehrenamts.
```
Ask: Welche Anfragen haben den Humanizer geladen, verglichen mit deinen Vermutungen?

### Teste, welche Anfragen ihn laden [chatgpt]
Why: Deine KI entscheidet **in jedem Chat neu**, ob eine Anfrage zur Beschreibung passt. Deshalb kommt jede Anfrage in einen eigenen neuen Chat, und eine Anfrage schickst du zweimal, um zu sehen, ob die Entscheidung gleich bleibt.
Do:
1. Notiere, welche der drei erfundenen Anfragen den Humanizer deiner Meinung nach laden: die Garten-Anfrage, die E-Mail-Anfrage und die Newsletter-Anfrage.
2. Schicke jede Anfrage in einem eigenen neuen Chat in **Work**.
3. Schicke die Newsletter-Anfrage oder eine überraschende eigene Anfrage noch einmal in einem neuen Chat in **Work**.
4. Überfliege jede Antwort: Ein Entwurf, eine kurze Liste verbliebener KI-Muster und eine endgültige Überarbeitung bedeuten, dass der Humanizer geladen hat. Eine einzelne Überarbeitung bedeutet, dass er sehr wahrscheinlich nicht geladen hat.
5. Prüfe in den Überarbeitungen der Garten-Anfrage, dass Name, Datum und Zahlen erhalten geblieben sind.
Code:
```text
Lass das hier weniger nach KI klingen:
Ich freue mich riesig, euch mitzuteilen: Unser Garten ist nicht nur Erde, er ist eine Bewegung. Am 21. November pflanzen Jonas Weber und 12 Freiwillige 40 Bäume. Lass das mal sacken.

Fasse diese E-Mail in einem Satz zusammen:
Das Büro ist am 31. Okt. geschlossen.

Überarbeite diesen Absatz für unseren Newsletter:
Wir freuen uns sehr, bekannt zu geben, dass Mira als Projektleitung zu uns kommt. Ihr Weg ist ein Beweis für die Kraft des Ehrenamts.
```
Ask: Welche Anfragen haben den Humanizer geladen, verglichen mit deinen Vermutungen?

## Trust check
Watch for:
- Lies einen Skill, den jemand anderes geschrieben hat, bevor du ihn installierst und noch einmal nach jedem Update. Eine ZIP-Datei des ganzen Repositorys oder ein Installer bringt mehr Dateien zum Prüfen mit als nur die `SKILL.md`.
- Prüfe in jeder Überarbeitung Namen, Daten und Zahlen, bevor du sie verwendest.
- Wende den Humanizer nur dann auf deinen eigenen Entwurf an, wenn deine Organisation diesen Entwurf in dieser App erlaubt.
Ask: Ist dein eigener Entwurf in dieser App erlaubt, oder nimmst du den erfundenen Newsletter-Absatz?

## Test
Do:
1. Wenn eine Anfrage den Humanizer geladen hat, öffne einen neuen Chat und formuliere deine Anfrage mit den Worten dieser Anfrage.
2. Wenn keine Anfrage ihn geladen hat, prüfe, dass sein Schalter eingeschaltet ist, und beginne deine Anfrage dann mit „Nutze den humanizer-Skill“.
3. Füge deinen eigenen KI-Entwurf ein, wenn er in dieser App erlaubt ist, oder den erfundenen Newsletter-Absatz.
4. Vergleiche Namen, Daten und Zahlen in der Überarbeitung mit deinem Entwurf.
5. Um den Humanizer später zu entfernen: Klicke neben dem Skill auf **...**, **Delete**.
Check:
- Die Antwort zeigt einen Entwurf, eine Liste verbliebener KI-Muster und eine endgültige Überarbeitung.
- Jeder Name, jedes Datum und jede Zahl aus deinem Entwurf ist noch da.
Ask: Wie hast du den Humanizer angefragt, und sind Namen, Daten und Zahlen erhalten geblieben?

## Test [chatgpt]
Do:
1. Wenn eine Anfrage den Humanizer geladen hat, öffne einen neuen Chat in **Work** und formuliere deine Anfrage mit den Worten dieser Anfrage.
2. Wenn keine Anfrage ihn geladen hat, prüfe, dass er unter **Plugins**, **Skills**, **Created by me** steht, tippe dann `@` und wähle den Humanizer.
3. Füge deinen eigenen KI-Entwurf ein, wenn er in dieser App erlaubt ist, oder den erfundenen Newsletter-Absatz.
4. Vergleiche Namen, Daten und Zahlen in der Überarbeitung mit deinem Entwurf.
5. Um den Humanizer später zu entfernen: Die Hilfeseiten von ChatGPT beschreiben das Entfernen nicht.
Check:
- Die Antwort zeigt einen Entwurf, eine Liste verbliebener KI-Muster und eine endgültige Überarbeitung.
- Jeder Name, jedes Datum und jede Zahl aus deinem Entwurf ist noch da.
Ask: Wie hast du den Humanizer angefragt, und sind Namen, Daten und Zahlen erhalten geblieben?

## Test [gemini]
Do:
1. Wenn eine Anfrage den Humanizer geladen hat, öffne einen neuen Chat und formuliere deine Anfrage mit den Worten dieser Anfrage.
2. Wenn keine Anfrage ihn geladen hat, prüfe, dass der Skill aktiv ist (**More**, **Activate**), tippe dann `/` oder `@` und wähle den Humanizer.
3. Füge deinen eigenen KI-Entwurf ein, wenn er in dieser App erlaubt ist, oder den erfundenen Newsletter-Absatz.
4. Vergleiche Namen, Daten und Zahlen in der Überarbeitung mit deinem Entwurf.
5. Um den Humanizer später zu entfernen: **More**, **Delete**.
Check:
- Die Antwort zeigt einen Entwurf, eine Liste verbliebener KI-Muster und eine endgültige Überarbeitung.
- Jeder Name, jedes Datum und jede Zahl aus deinem Entwurf ist noch da.
Ask: Wie hast du den Humanizer angefragt, und sind Namen, Daten und Zahlen erhalten geblieben?

## Done when
- Der Humanizer ist in deiner KI installiert und eingeschaltet.
- Du hast notiert, welche Anfragen den Humanizer geladen haben, und eine Anfrage zweimal geschickt.
- Ein Entwurf ist durch den Humanizer gelaufen, und du hast Namen, Daten und Zahlen mit dem Original verglichen.

## Practice
- Nimm einen Post oder eine E-Mail, die du vor Kurzem mit KI entworfen hast, frag den Humanizer mit den Worten an, die ihn geladen haben, und vergleiche Namen, Daten und Zahlen.
- Schreib eine Anfrage zu einem Absatz, der nach KI klingt, ohne ein Wort aus der Beschreibung zu verwenden, schick sie in einem neuen Chat und schau, ob der Humanizer lädt.
- Öffne deine Skill-Liste, lies die Beschreibung eines anderen Skills, schreib eine Anfrage, von der du erwartest, dass sie ihn lädt, und eine, von der du erwartest, dass sie es nicht tut, und probiere beide in neuen Chats aus.

## Glossary
- Beschreibung (des Skills): der kurze Text in der `SKILL.md` eines Skills, den deine KI in jedem Chat sieht und mit dem sie entscheidet, ob sie die Anweisungen liest.
- Laden: Deine KI liest die Anweisungen eines Skills und befolgt sie für deine Anfrage.
- KI-Anzeichen: eine Schreibgewohnheit, durch die ein Text nach KI klingt, etwa „Lass das mal sacken“ oder „ist nicht nur X, sondern Y“.

## Sources
- [Agent Skills, Specification](https://agentskills.io/specification): Deine KI sieht von jedem Skill Namen und Beschreibung und liest die Anweisungen nur, wenn die Beschreibung passt (Progressive Disclosure, also schrittweise Offenlegung).
- [blader, humanizer, GitHub repository, version 3.1.0 (commit 0ef9fe5, 28 October 2026)](https://github.com/blader/humanizer): was der Humanizer tut, seine Beschreibung, die KI-Anzeichen, seine Antwort aus Entwurf, Liste und Überarbeitung sowie die Dateien, die ein Download des ganzen Repositorys mitbringt.
- [Anthropic, Use skills in Claude, Claude Help Center](https://support.claude.com/en/articles/12512180-use-skills-in-claude): die Einstellung Create and edit files sowie Hochladen, Einschalten, Aufrufen per Name und Löschen eines Skills in Claude.
- [OpenAI, Get started with ChatGPT Work, ChatGPT documentation](https://learn.chatgpt.com/docs/get-started-with-work): das Umstellen des Eingabefelds auf Work.
- [OpenAI, Build skills, ChatGPT documentation](https://learn.chatgpt.com/docs/build-skills): einen Skill mit skill-creator erstellen und mit `@` aufrufen.
- [OpenAI, Skills in ChatGPT, OpenAI Help Center](https://help.openai.com/en/articles/20001066-skills-in-chatgpt): Tarife, die Skills unterstützen, und wo erstellte Skills aufgelistet sind.
- [Google, Create & manage skills for Gemini Apps (Computer), Gemini Apps Help](https://support.google.com/gemini/answer/17094296?hl=en&co=GENIE.Platform%3DDesktop): Voraussetzungen sowie Hochladen, Aktivieren, Aufrufen mit `/` oder `@` und Löschen eines Skills in Gemini.

## Coach notes
Arc: Diese Mission vermittelt ein Denkmodell. Die lernende Person sieht, dass die Beschreibung eines Skills entscheidet, wann er lädt, und beobachtet das dann mit echten Anfragen. Zwei Arbeitsphasen am Laptop mit einer Rückkehr in den Chat dazwischen: den Humanizer lesen und installieren, dann die Testanfragen schicken. Der Test ist ein dritter kurzer Durchlauf mit einem Entwurf.

Concept and check: Geh das Konzept durch und stell dann die Frage aus Check your understanding. Greif in jeder Antwort auf, was daran stimmt. B und C sind die häufigsten Vorstellungen: „eingeschaltet“ fühlt sich an wie „immer genutzt“. Erkläre, dass eingeschaltet bedeutet, dass die Beschreibung im Blick ist, und dass die Anfrage entscheidet. Bei D stimm zu, dass das Nennen des Skills funktioniert und später in dieser Mission ein nützlicher Ausweg ist.

Reading `SKILL.md`: Auf der Seite gibt es hier kein Ask. Warte also, bis die lernende Person im Installationsschritt berichtet. Findet sie Schritte, die Links öffnen, Dateien verschicken oder Programme ausführen, oder andere Links als den zu Wikipedia, schaut euch gemeinsam an, was sie gefunden hat, und überlass ihr die Entscheidung. Die Installation abzulehnen ist eine gültige Entscheidung, der Coach drängt nicht. Lehnt sie ab, gilt das Konzept trotzdem, und sie kann zur Installation zurückkehren, wenn sie so weit ist.

Install, evidence to await: was das Lesen ergeben hat und ob die Beschreibung in der Skill-Liste mit „Rewrite AI-sounding text“ beginnt. Nachfragen: „Wo hast du den Humanizer in deiner Skill-Liste gefunden?“ und „Ist er eingeschaltet?“. Hat sich die Beschreibung geändert (wahrscheinlich nur in ChatGPT, durch skill-creator), bittet die lernende Person skill-creator, das Original zu behalten, und prüft noch einmal. Claude: Schlägt der Upload fehl, prüfe, dass die Datei `SKILL.md` heißt und in einem Ordner namens `humanizer` liegt und dass Create and edit files eingeschaltet ist. In Enterprise muss zuerst ein Owner Skills freischalten. Gemini: Zeigt **More** den Eintrag **Deactivate**, ist der Skill aktiv.

Bevor die lernende Person die Testanfragen schickt, frag nach ihren Vermutungen und wiederhole sie, wenn sie zurückkommt, damit sie sich nicht daran erinnern muss. Gib die drei Anfragen aus dem Codeblock des Schritts einzeln heraus, wenn die lernende Person sie einzeln haben möchte.

Test requests, evidence to await: welche Anfragen einen Entwurf, eine Liste verbliebener KI-Muster und eine endgültige Überarbeitung gezeigt haben, das Ergebnis der wiederholten Anfrage und ob Name, Datum und Zahlen in den Überarbeitungen der Garten-Anfrage erhalten geblieben sind. Verbinde jede Beobachtung mit der Beschreibung: Eine Anfrage, einen Text „weniger nach KI klingen“ zu lassen oder einen Text zu bearbeiten, passt zu „Rewrite AI-sounding text“ und „editing or reviewing prose for AI tells“. Eine E-Mail-Zusammenfassung passt nicht. Bleib beim Beobachteten: Die Form der Antwort deutet darauf hin, dass der Humanizer geladen hat, beweist aber nicht, welche Anweisungen ausgeführt wurden. Hat die wiederholte Anfrage ein anderes Ergebnis gebracht, ist das nützlich: Deine KI entscheidet in jedem Chat neu, also urteile nach mehreren Durchläufen. Stimmten alle Vermutungen beim ersten Versuch, ist das ein gutes Ergebnis. Die wiederholte oder überraschende Anfrage ist der zweite Fall, und erzeuge nie künstlich einen Fehlschlag. Hat keine Anfrage den Humanizer geladen, zeigt der Test den Weg, ihn per Name aufzurufen.

Test: Gib den Einstieg „Nutze den humanizer-Skill“ (Claude) und den Newsletter-Absatz zum Kopieren heraus, wenn die lernende Person keinen eigenen Entwurf hat:
„Überarbeite diesen Absatz für unseren Newsletter:
Wir freuen uns sehr, bekannt zu geben, dass Mira als Projektleitung zu uns kommt. Ihr Weg ist ein Beweis für die Kraft des Ehrenamts.“
Evidence to await: wie sie angefragt hat und ob Namen, Daten und Zahlen erhalten geblieben sind. Hat sich ein Fakt geändert, korrigiert die lernende Person ihn in der Überarbeitung, bevor sie sie verwendet. Entfernen: Claude **...**, **Delete**; Gemini **More**, **Delete**; die Hilfeseiten von ChatGPT beschreiben das Entfernen nicht.

Levels: Lernende auf der Stufe guided bekommen jede Anweisung einzeln, und der Coach erklärt die Raw-Seite und das Zippen in einfachen Worten. Lernende auf der Stufe standard folgen der Seite und berichten bei jedem Ask. Lernende auf der Stufe fast-track können die `SKILL.md` gründlicher überfliegen und im Test eine überraschende eigene Anfrage ergänzen, etwa eine, die die Worte der Beschreibung für einen fachfremden Text verwendet.

Tools: Claude im Chat, in der Desktop-App und auf claude.ai nutzt den Standardtext. ChatGPT braucht die Desktop-App, den Work-Modus und einen Tarif, der Skills erlaubt. Erlaubt der Workspace keine Skills, kann die lernende Person nicht installieren. Sprecht dann das Konzept durch und hört dort auf. Gemini setzt voraus, dass die lernende Person mindestens 18 Jahre alt ist und Keep Activity eingeschaltet hat.

Time budget: Konzept und Verständnisfrage 3 Minuten, `SKILL.md` lesen 3, Installation 5, Testanfragen 5, Test 4.

Review, what the coach says at the end:
- What you did: Frag die lernende Person, welche Anfragen den Humanizer geladen haben und wie sie ihn für ihren Entwurf angefragt hat, und fasse dann nur auf Grundlage ihres Berichts zusammen.
- What to remember: Deine KI wählt Skills anhand der Beschreibung aus, in jedem Chat neu, also urteile nach mehreren Durchläufen. Kein Treffer? Verwende die Worte der Beschreibung oder den Namen des Skills. Lies Skills von anderen vor der Installation und nach Updates. Eine ZIP-Datei des ganzen Repositorys oder ein Installer bringt Dateien mit, die du prüfen musst.
- In one sentence: Die Beschreibung eines Skills entscheidet, wann er lädt. Nutze den Humanizer für deinen nächsten Entwurf, der nach KI klingt.
