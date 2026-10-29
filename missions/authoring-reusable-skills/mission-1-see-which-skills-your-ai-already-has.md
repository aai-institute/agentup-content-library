---
# source: 7f154216ab2506b2
id: mission-1-see-which-skills-your-ai-already-has
number: 1
title: See which skills your AI already has
summary: Find the skills that came with your AI app, see how your AI reads one, and call one by name or with a matching request the next time a task fits.
artefact: none
---

Track: Integrating Agents
Level: foundation
Time: 20 minutes
Tools: Claude (desktop app or claude.ai), the ChatGPT desktop app, or the Gemini app (Mac app or gemini.google.com)
Artefact kind: none
Artefact file: none

## Context
You **explain the same tasks** to your AI again and again, while your app already holds **ready-made steps** for some of them. In this mission you find them, see how your AI reads one and call one, a step at a time.

## Your task
Find the **ready-made [[skills|Skill]]** in your AI app, read one, and **call one in two ways**: by name, and with a plain request that fits what the skill is for.

## After this, you can
Show where your app lists its skills and call one by name and with a plain request.

## You need
- **Claude** (desktop app or claude.ai) with **Create and edit files** switched on under **Settings**, **Capabilities**
- or the **ChatGPT desktop app** on a Business, Enterprise, Healthcare or Edu plan
- or the **Gemini app** (Mac app or gemini.google.com), if you are 18 or over and have **Keep Activity** on
- A **browser**

## You should already
- **Start a new chat** in your AI app
- Find your app's **settings or sidebar**
- **Search a web page** with **Cmd+F** (Mac) or **Ctrl+F** (Windows)

## Concept
Heading: What a skill holds, and what the AI reads when
Lead: A **skill** is a folder with a `SKILL.md` file, like this made-up **meeting-agenda** skill.
- [[Header]]: the lines between two `---` lines at the top of `SKILL.md`, which hold the name and the description.
- Name: a short label for the skill, such as `meeting-agenda`.
- [[Description]]: what the skill does and when to use it, such as "Turns a list of topics into a one-page meeting agenda. Use when the user asks for an agenda or wants to prepare a meeting."
- Steps: the instructions the AI follows, after the header, such as "1. Ask for the meeting's date, time and length if they're missing. 2. Give each topic a time slot and an owner."
- Further files: other files in the folder, which the AI reads only when the steps send it there.
Close: At the start of a chat the AI sees only the name and description of each switched-on skill; it reads the steps when the description fits your request, and further files only when the steps point to them.
Toggle: Why does the description say when to use the skill? | At the start of a chat, the name and description are all the AI sees of a skill. Your request has to fit the description before the AI reads the steps, so the "when to use" part decides whether the skill comes into play.

## Check your understanding
Question: The meeting-agenda skill is switched on. In a new chat you write "Translate this email into German." What do you think the AI reads of the meeting-agenda skill?
- A: Only its name and description, because the request doesn't fit the description
- B: Its whole file, steps included, because every switched-on skill is read in full at the start of a chat
- C: Nothing at all, because you didn't name the skill
- D: Its steps and every further file in its folder
Answer: A
Why: The AI sees the name and description of every switched-on skill at the start of a chat, and reads the steps only when the description fits the request. A translation request doesn't fit "Use when the user asks for an agenda or wants to prepare a meeting", so the steps stay unread. B is tempting because the skill is switched on, but being switched on only puts the name and description in front of the AI. C is tempting because naming a skill does make sure the AI uses it, but the name and description are there even when you don't name it. D mixes up the order: further files come last, and only when the steps send the AI there.

## Working example
Situation: You want a one-page PDF of a team meeting agenda, a task one of your app's ready-made skills fits. You can use a task from your own week instead.
Input: A made-up agenda for a team meeting on Thursday, 10:00 to 11:00, with three topics.
- The AI sees the name and description of each switched-on skill.
- Your request, "Make a one-page PDF of this agenda", fits the PDF skill's description.
- The AI reads the PDF skill's steps.
- The AI follows those steps to make the PDF.
Result: A one-page PDF of the agenda, made by following the skill's steps instead of your explanation.

## Steps
### Read a real skill
Why: The AI decides from the **description** whether to read a skill's steps, so the "when to use" part is the first thing to look for in any skill.
Do:
1. Open Anthropic's **pdf** skill in your browser: [raw.githubusercontent.com/anthropics/skills/main/skills/pdf/SKILL.md](https://raw.githubusercontent.com/anthropics/skills/main/skills/pdf/SKILL.md).
2. Skip its Python code: you only read this file.
3. Press **Cmd+F** (Mac) or **Ctrl+F** (Windows) and find the `description` line in the header.
4. Find the heading `Quick Start`, where the steps start.
5. Find the line that mentions `FORMS.md`.
Ask: In your own words, when should the AI use the pdf skill?

### Find the ready-made skills in your app
Why: Your app's skills list shows which ready-made skills are **switched on**, and only those reach the AI at the start of a chat.
Do:
1. In Claude, open **Customize**, then **Skills**.
2. Look through Anthropic's own skills for Excel, Word, PowerPoint and PDF.
3. Check that the **PDF** skill's toggle is on.
4. Open one skill that fits a task from your week, and find the "when to use" part of its description.
Ask: Which ready-made skills did you find, and what is your chosen skill's "when to use" phrase?

### Find the ready-made skills in your app [chatgpt]
Why: Your app's skills list shows which ready-made skills are **switched on**, and only those reach the AI at the start of a chat.
Do:
1. In the ChatGPT desktop app, select **Plugins** in the sidebar, then the **Skills** tab. If your sidebar shows **Skills** instead, open that.
2. Look through the ready-made skills, such as **skill-creator**.
3. If you can't find skills, update the app and restart it. If they are still missing, ask your workspace admin whether your plan includes skills.
4. Open one skill that fits a task from your week, and find the "when to use" part of its description.
Ask: Which ready-made skills did you find, and what is your chosen skill's "when to use" phrase?

### Find the ready-made skills in your app [gemini]
Why: Your app's skills list shows which ready-made skills are **switched on**, and only those reach the AI at the start of a chat.
Do:
1. In the Gemini app, open **Customize**, then **Skills**. If you don't see **Customize**, open **More** first.
2. Look under **Recommended**, where Gemini keeps its ready-made skills as templates.
3. Click one that fits a task from your week to use it.
4. Read its **Description** and **Instructions**, and find the "when to use" part.
Ask: Which ready-made skills did you find, and what is your chosen skill's "when to use" phrase?

### Call the skill by name
Use: A task from your week that your chosen skill fits, or the made-up agenda for the PDF skill.
Why: Calling a skill **by name** makes sure the AI uses it, so you see what its steps produce.
Do:
1. Start a **new chat** in Claude.
2. Type "Use the [name] skill", followed by your request. For the PDF skill, you can copy the made-up agenda request in the Code box.
3. Send it, and compare the output with the skill's steps.
Code:
```text
Use the PDF skill. Make a one-page PDF of this agenda:
Team meeting, Thursday 10:00 to 11:00
1. Project Falcon: site 2 start date
2. New starter Mira: first week plan
3. Data export: who owns it?
```
Ask: Which of the skill's steps can you see in the output?

### Call the skill by name [chatgpt]
Use: A task from your week that your chosen skill fits.
Why: Calling a skill **by name** makes sure the AI uses it, so you see what its steps produce.
Do:
1. Start a **new chat** in the ChatGPT desktop app.
2. Type `@` and choose your skill.
3. Add your request and send it.
4. Compare the output with the skill's steps.
Ask: Which of the skill's steps can you see in the output?

### Call the skill by name [gemini]
Use: A task from your week that your chosen skill fits.
Why: Calling a skill **by name** makes sure the AI uses it, so you see what its steps produce.
Do:
1. Start a **new chat** in the Gemini app.
2. Type `/` or `@` and choose your skill.
3. Add your request and send it.
4. Compare the output with the skill's steps.
Ask: Which of the skill's steps can you see in the output?

## Trust check
Watch for:
- Reading the pdf skill's file in your browser: read the header and the steps, and leave its Python code alone.
- Using a recommended skill in Gemini adds it to your skills: to remove it later, open **More**, then **Deactivate** or **Delete**.
- Choosing the material for your request: use a task you are allowed to put into this AI app, or the made-up agenda.
Ask: Is the material you use with the skill fine to put into this AI app, or will you use the made-up agenda?

## Test
Do:
1. Start another **new chat**.
2. Write the same request without the skill's name, in words that match its description, such as "Make a one-page PDF of this agenda" followed by the agenda.
3. Before you send it, note whether you expect the AI to use the skill.
4. Send it, and look for the skill's steps in the output.
Check:
- The output shows the same steps you saw when you called the skill by name.
- What happened matches what you expected before sending.
Ask: What did you expect, and what came out this time?

## Done when
- You can show where your app lists its ready-made skills and point to the "when to use" part of a description.
- You've called a skill by name and with a matching request, and compared each output with the skill's steps.

## Practice
- Open a different ready-made skill in your app, read its "when to use" part, and call it by name with a small task from your week.
- For one ready-made skill, write one request that fits its description and one that doesn't, and send each in a new chat.
- The next time you start explaining a task to your AI, check your skills list for a description that fits, and call that skill instead.

## Glossary
- Skill: a folder with a `SKILL.md` file that holds a name, a description and the steps the AI follows for a task.
- Header: the lines between two `---` lines at the top of `SKILL.md`, holding the skill's name and description.
- Description: the line in a skill's header saying what the skill does and when to use it; the AI reads the steps only when a request fits it.

## Sources
- [Agent Skills, Specification](https://agentskills.io/specification): the format of a skill, and the order in which the AI reads the name and description, the steps and further files.
- [Anthropic, Use skills in Claude, Claude Help Center](https://support.claude.com/en/articles/12512180-use-skills-in-claude): the Create and edit files setting, where Claude lists its skills, Anthropic's own skills, and calling a skill by name or with a matching request.
- [OpenAI, Build skills, ChatGPT documentation](https://learn.chatgpt.com/docs/build-skills): the Skills entry in the sidebar, calling a skill with `@`, and ChatGPT picking a skill when a request matches its description.
- [OpenAI, Skills in ChatGPT, OpenAI Help Center](https://help.openai.com/en/articles/20001066-skills-in-chatgpt): which plans include skills, the Plugins and Skills tab, and the ready-made skill-creator.
- [Google, Create & manage skills for Gemini Apps (Computer), Gemini Apps Help](https://support.google.com/gemini/answer/17094296?hl=en&co=GENIE.Platform%3DDesktop): requirements, Customize and Skills, Recommended templates, calling with `/` or `@`, and deactivating or deleting a skill.
- [Anthropic, skills, GitHub repository](https://github.com/anthropics/skills): the real pdf skill the learner reads.

Coach notes:

Arc of the mission: the learner meets skills from the outside, as ready-made steps their app already has. Concept first (what a skill holds and the order the AI reads it), one check, then three laptop periods: reading a real skill in the browser, finding skills in their own app, and calling one by name. The Test is the second call, without the name. The learner returns to the chat after each period. The coach waits for what the learner saw, never describes what the app "will" show, and never does the laptop work for them.

Check your understanding: talk through the learner's pick using the Why. If they chose B, C or D, start with what's right in it (B: switched on does matter; C: naming does make sure the skill is used; D: further files do exist) and then explain the reading order.

Step 1, Read a real skill. Evidence to wait for: the learner's own words for when the pdf skill should be used. Follow-up questions, one at a time:
- Did you find the heading `Quick Start`? That's where the steps start.
- What does the line that mentions `FORMS.md` say? It's a further file the AI reads only when the steps send it there.
- Would "Write this agenda as a short email" make the AI read the pdf skill's steps?
Note the learner's answer to the email question: the Test may need it, and the coach repeats it to them rather than asking them to remember it. If the learner gets lost in the Python code, remind them to search only for `description`, `Quick Start` and `FORMS.md`. Guided: go through one search at a time. Fast-track: ask for all three finds in one reply.

Step 2, Find the ready-made skills. Evidence: the list of skills they found and their chosen skill's "when to use" phrase, plus its "when not to use" part if it has one. Claude: if Skills doesn't show, check that Create and edit files is on under Settings, Capabilities. ChatGPT: if the Skills tab is missing, the learner updates and restarts the app; if it's still missing, they ask their workspace admin whether their plan includes skills, and you can carry on with the reading part and finish the call later. Gemini: the ready-made skills are templates under Recommended; clicking one adds it, and More, Deactivate or Delete removes it later. If the learner can't find a skill that fits their week, suggest the PDF skill and the made-up agenda in Claude, or the closest fit in their app.

Step 3, Call the skill by name. Evidence: which of the skill's steps they can see in the output. Help them link the steps visible in the output to the steps in the skill. Stick to what the output shows: it suggests the skill was used, but doesn't prove what happened inside the app.

Test. Hand over this text, ready to copy, for learners using the made-up agenda:
```text
Make a one-page PDF of this agenda:
Team meeting, Thursday 10:00 to 11:00
1. Project Falcon: site 2 start date
2. New starter Mira: first week plan
3. Data export: who owns it?
```
For their own task, help them word the request with the description's "when to use" words, without the skill's name. Evidence: their prediction and what came out. Then pick the branch:
- It looks like it used the skill both times: repeat the learner's earlier answer about the email request, hand over "Write this agenda as a short email" to send in a new chat, and ask whether their answer holds.
- It seems to have skipped the skill without the name: the learner rewords the request with the description's "when to use" words and tries again in a new chat. If it still skips the skill, this task needs the name, and they call it by name from now on.
Never invent a failure; a successful first run still gets the email request as a second case.

Tools: Claude calls a skill by name in the request ("Use the [name] skill"), ChatGPT with `@`, Gemini with `/` or `@`. All three can pick a skill on their own when a request matches its description.

Levels: guided learners get each action one at a time and every reason explained. Standard learners follow the page. Fast-track learners can skip the check of understanding if they answer quickly, and can compare the descriptions of two ready-made skills in their app.

Time budget: Concept and check 3 minutes, reading the pdf skill 3, finding skills 5, calling by name 4, Test and second case 5.

Review, at the end:
- What you did: ask which skill they called, and what happened when they named it and when they didn't. Sum up only from what they reported.
- What to remember: the AI reads only the name and description until a request fits; then it reads the steps. A plain request works when your words match the description. Calling the skill by name makes sure the AI uses it: in the request in Claude, with `@` in ChatGPT, with `/` or `@` in Gemini.
- In one sentence: the next time a task matches a skill that came with your app, call the skill instead of explaining the task again.
