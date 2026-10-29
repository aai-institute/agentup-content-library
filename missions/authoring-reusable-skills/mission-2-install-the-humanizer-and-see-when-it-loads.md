---
# source: 630139131db840fb
id: mission-2-install-the-humanizer-and-see-when-it-loads
number: 2
title: Install the humanizer and see when it loads
summary: Check and install a popular skill that takes the AI sound out of your drafts, then test which requests make your AI use it, so you know how to ask for it next time.
artefact: the humanizer skill, installed and tested
---

Track: Integrating Agents
Level: foundation
Time: 20 minutes
Tools: Claude in the desktop app or at claude.ai, the ChatGPT desktop app, or Gemini in the Mac app or at gemini.google.com
Artefact kind: text
Artefact file: SKILL.md

## Context
You let AI draft **newsletters, posts or emails**, then fix phrases like "isn't just X, it's Y" by hand. The **humanizer**, a skill from an outside author, rewrites a draft so it no longer sounds like AI and keeps what the draft says. In this mission you check it, install it and find out, step by step, **which requests** make your AI use it.

## Your task
**Check and install** the humanizer, test **which requests** make your AI use it, and use it on an **AI-sounding text**.

## After this, you can
The humanizer is switched on in your AI, and you have a note of which requests made your AI use it and how you asked for it on a draft.

## You need
- **Claude** in the desktop app or at claude.ai, with **Create and edit files** switched on under **Settings**, **Capabilities**. On an Enterprise plan, an owner enables skills first.
- The humanizer's **GitHub page**: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- An **AI-drafted text** of your own, if your workplace allows it in this app, or the made-up newsletter paragraph in this mission.

## You need [chatgpt]
- The **ChatGPT desktop app** on a Business, Enterprise, Healthcare or Edu plan, if your **workspace allows skills**.
- The humanizer's **GitHub page**: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- An **AI-drafted text** of your own, if your workplace allows it in this app, or the made-up newsletter paragraph in this mission.

## You need [gemini]
- **Gemini** in the Mac app or at gemini.google.com, aged 18 or over, with **Keep Activity** on.
- The humanizer's **GitHub page**: [github.com/blader/humanizer](https://github.com/blader/humanizer).
- An **AI-drafted text** of your own, if your workplace allows it in this app, or the made-up newsletter paragraph in this mission.

## You should already
- **Download** a file from a website.
- **Zip** a folder.
- Know that a **skill** is a folder with a `SKILL.md` file holding its name, description and instructions.

## You should already [chatgpt]
- **Copy** text from a website.
- Know that a **skill** is a folder with a `SKILL.md` file holding its name, description and instructions.

## You should already [gemini]
- **Download** a file from a website.
- Know that a **skill** is a folder with a `SKILL.md` file holding its name, description and instructions.

## Concept
Heading: How your AI decides to use a skill
Lead: In every chat, your AI sees only each skill's **name** and **[[description|Skill description]]**, and reads the skill's **instructions** only when the description fits your request.
- Name and description: always in view, so the humanizer's description, starting "Rewrite AI-sounding text so it reads like the writer without changing what it says", is what your request gets matched against.
- Instructions: read only when the description fits, which is when the skill **[[loads|Load]]**.
- [[AI tells|AI tell]]: the habits the description names, such as "It's not just a feature, it's a shift" (not-X-but-Y), "Let that sink in" (one-line closer), "Here's the thing" (staged opener) and "delve" (stock AI word).
Close: Because your AI sees the name and description up front and decides afresh in every chat, the words of your request decide whether the humanizer's instructions load.
Toggle: What does the humanizer's description say in full? | "Rewrite AI-sounding text so it reads like the writer without changing what it says. Use when editing or reviewing prose for AI tells: not-X-but-Y contrasts, one-line closers, staged openers, forced triads, dashes everywhere, inflated claims, sales language, stock AI words, bold labels, or filler. Based on Wikipedia's "Signs of AI writing.""
Toggle: Why not read every skill's instructions in every chat? | Your AI keeps only the name and description of each skill in view and reads the instructions when they fit. The description is the part that has to carry the decision.

## Check your understanding
Question: The humanizer is switched on, and you ask "Summarise this email in one sentence". What do you think your AI does with the humanizer?
- A: It sees the humanizer's name and description, and most likely leaves the instructions unread, because summarising an email doesn't fit the description.
- B: It reads the instructions of every switched-on skill before each answer, so it reads the humanizer's too.
- C: It runs the humanizer on the summary, because the skill is switched on.
- D: It can't see the humanizer at all unless you name the skill in your request.
Answer: A
Why: Your AI sees only each skill's name and description in every chat and reads the instructions only when the description fits the request; a one-sentence email summary isn't editing or reviewing prose for AI tells. B is tempting because a switched-on skill feels "active", but the instructions are read only on a fit. C mixes up "switched on" with "used": switching a skill on puts its description in view, and the request still decides. D has a true core, since naming the skill is one way to ask for it, but the description is in view without naming it.

## Working example
Situation: You let AI draft a newsletter paragraph, then fix phrases like "isn't just X, it's Y" by hand before sending it.
Input: The humanizer's `SKILL.md` on GitHub, three made-up test requests and the made-up newsletter paragraph.
- You read the humanizer's `SKILL.md` and install the skill in your AI.
- You send three requests, each in its own new chat, and your AI decides from the description whether to load the humanizer.
- When the humanizer loads, your AI answers with a draft, a short list of AI patterns left, and a final rewrite.
- You ask for the humanizer on a draft in words that loaded it, and check names, dates and numbers.
Result: The humanizer is switched on, you have a note of which requests loaded it, and a draft reads less like AI with its facts intact.

## Steps
### Read the humanizer before installing
Why: A skill acts with your AI's **access**, so a step in its instructions that opens links, sends files or runs programs would do that with your access; reading `SKILL.md` first shows you what you are switching on.
Do:
1. Open [github.com/blader/humanizer](https://github.com/blader/humanizer) and click **SKILL.md**.
2. Click **Raw** to see the plain text.
3. Read the part headed *How to work*: check it has no steps that open links, send files or run programs.
4. Search the page for `http` with **Cmd+F** or **Ctrl+F**: the only link should be Wikipedia's.
5. Found other links or such steps? Ask in the chat before you install. You decide whether to install it.

### Install the humanizer
Why: Installing puts the humanizer's **name and description** in view in every chat, and checking the description afterwards shows that it arrived **unchanged**.
Do:
1. Back on the `SKILL.md` page, click **Download raw file** (the download icon).
2. Check the file is named `SKILL.md`, put it in a new folder named `humanizer`, and zip the folder.
3. In Claude, go to **Customize**, **Skills**, **+**, **Create skill**, **Upload a skill**, and choose the ZIP.
4. Find the humanizer in your skills list and check its toggle is on.
5. Check the description still starts "Rewrite AI-sounding text".
Ask: What did your read of `SKILL.md` turn up, and does the description in your skills list start the same way?

### Install the humanizer [chatgpt]
Why: Installing puts the humanizer's **name and description** in view in every chat, and checking the description afterwards shows that it arrived **unchanged**.
Do:
1. On the **Raw** page of `SKILL.md`, copy all the text.
2. In the ChatGPT desktop app, switch the composer to **Work**.
3. Type `@skill-creator`, then send the request in the code block with the copied text pasted after it.
4. Go to **Plugins**, **Skills**, **Created by me**, and find the humanizer.
5. Check the description still starts "Rewrite AI-sounding text". Changed? Ask skill-creator to keep the original.
Code:
```text
Create a skill from exactly this SKILL.md, unchanged. It needs no scripts.
```
Ask: What did your read of `SKILL.md` turn up, and does the description in your skills list start the same way?

### Install the humanizer [gemini]
Why: Installing puts the humanizer's **name and description** in view in every chat, and checking the description afterwards shows that it arrived **unchanged**.
Do:
1. Back on the `SKILL.md` page, click **Download raw file** (the download icon), and check the file is named `SKILL.md`.
2. In Gemini, go to **Customize** (under **More** if hidden), **Skills**, **Create**, **Upload**.
3. Choose the file and click **Create**.
4. Find the humanizer in your skills list: **More** shows **Deactivate** when it is active.
5. Check the description still starts "Rewrite AI-sounding text".
Ask: What did your read of `SKILL.md` turn up, and does the description in your skills list start the same way?

### Test which requests load it
Why: Your AI decides **afresh in every chat** whether a request fits the description, so each request goes into its own new chat, and one request goes in twice to see whether the choice holds.
Do:
1. Note which of the three made-up requests you think will load the humanizer: the garden request, the email request and the newsletter request.
2. Send each request in its own new chat.
3. Send the newsletter request, or a surprising one of your own, again in a new chat.
4. Skim each answer: a draft, a short list of AI patterns left, and a final rewrite mean the humanizer loaded; a single rewrite means it most likely didn't.
5. In the garden rewrites, check that the name, the date and the numbers survived.
Code:
```text
Make this sound less like AI:
I'm thrilled to share that our garden isn't just soil, it's a movement. On 21 November, Jonas Weber and 12 volunteers will plant 40 trees. Let that sink in.

Summarise this email in one sentence:
The office is closed on 31 Oct.

Tidy up this paragraph for our newsletter:
We are thrilled to announce that Mira joins us as project lead. Her journey is a testament to the power of volunteering.
```
Ask: Which requests loaded the humanizer, next to your guesses?

### Test which requests load it [chatgpt]
Why: Your AI decides **afresh in every chat** whether a request fits the description, so each request goes into its own new chat, and one request goes in twice to see whether the choice holds.
Do:
1. Note which of the three made-up requests you think will load the humanizer: the garden request, the email request and the newsletter request.
2. Send each request in its own new chat in **Work**.
3. Send the newsletter request, or a surprising one of your own, again in a new chat in **Work**.
4. Skim each answer: a draft, a short list of AI patterns left, and a final rewrite mean the humanizer loaded; a single rewrite means it most likely didn't.
5. In the garden rewrites, check that the name, the date and the numbers survived.
Code:
```text
Make this sound less like AI:
I'm thrilled to share that our garden isn't just soil, it's a movement. On 21 November, Jonas Weber and 12 volunteers will plant 40 trees. Let that sink in.

Summarise this email in one sentence:
The office is closed on 31 Oct.

Tidy up this paragraph for our newsletter:
We are thrilled to announce that Mira joins us as project lead. Her journey is a testament to the power of volunteering.
```
Ask: Which requests loaded the humanizer, next to your guesses?

## Trust check
Watch for:
- Read a skill from someone else before you install it and again after it updates; a whole-repo ZIP or an installer adds more files to check than `SKILL.md`.
- Check names, dates and numbers in every rewrite before you use it.
- Run the humanizer on your own draft only if your workplace allows that draft in this app.
Ask: Is your own draft allowed in this app, or will you use the made-up newsletter paragraph?

## Test
Do:
1. If a request loaded the humanizer, open a new chat and ask in that request's words.
2. If no request loaded it, check its toggle is on, then start your request with "Use the humanizer skill".
3. Paste your own AI draft, if allowed in this app, or the made-up newsletter paragraph.
4. Compare the names, dates and numbers in the rewrite with your draft.
5. To remove the humanizer later: next to the skill, click **...**, **Delete**.
Check:
- The answer shows a draft, a list of AI patterns left and a final rewrite.
- Every name, date and number from your draft is still there.
Ask: How did you ask for the humanizer, and did the names, dates and numbers come through?

## Test [chatgpt]
Do:
1. If a request loaded the humanizer, open a new chat in **Work** and ask in that request's words.
2. If no request loaded it, check it is under **Plugins**, **Skills**, **Created by me**, then type `@` and choose the humanizer.
3. Paste your own AI draft, if allowed in this app, or the made-up newsletter paragraph.
4. Compare the names, dates and numbers in the rewrite with your draft.
5. To remove the humanizer later: ChatGPT's help pages don't describe removal.
Check:
- The answer shows a draft, a list of AI patterns left and a final rewrite.
- Every name, date and number from your draft is still there.
Ask: How did you ask for the humanizer, and did the names, dates and numbers come through?

## Test [gemini]
Do:
1. If a request loaded the humanizer, open a new chat and ask in that request's words.
2. If no request loaded it, check the skill is active (**More**, **Activate**), then type `/` or `@` and choose the humanizer.
3. Paste your own AI draft, if allowed in this app, or the made-up newsletter paragraph.
4. Compare the names, dates and numbers in the rewrite with your draft.
5. To remove the humanizer later: **More**, **Delete**.
Check:
- The answer shows a draft, a list of AI patterns left and a final rewrite.
- Every name, date and number from your draft is still there.
Ask: How did you ask for the humanizer, and did the names, dates and numbers come through?

## Done when
- The humanizer is installed and switched on in your AI.
- You have a note of which requests loaded the humanizer, with one request run twice.
- A draft went through the humanizer, and you compared its names, dates and numbers with the original.

## Practice
- Take a post or email you drafted with AI recently, ask for the humanizer in the words that loaded it, and compare names, dates and numbers.
- Write a request for an AI-sounding paragraph that uses none of the description's words, send it in a new chat, and see whether the humanizer loads.
- Open your skills list, read another skill's description, write one request you expect to load it and one you expect not to, and try both in new chats.

## Glossary
- Skill description: the short text in a skill's `SKILL.md` that your AI sees in every chat and uses to decide whether to read the instructions.
- Load: your AI reads a skill's instructions and follows them for your request.
- AI tell: a writing habit that makes text sound AI-written, such as "Let that sink in" or "isn't just X, it's Y".

## Sources
- [Agent Skills, Specification](https://agentskills.io/specification): your AI sees each skill's name and description, and reads the instructions only when the description fits (progressive disclosure).
- [blader, humanizer, GitHub repository, version 3.1.0 (commit 0ef9fe5, 28 October 2026)](https://github.com/blader/humanizer): what the humanizer does, its description, the AI tells, its draft, list and rewrite answer, and the files a whole-repo download adds.
- [Anthropic, Use skills in Claude, Claude Help Center](https://support.claude.com/en/articles/12512180-use-skills-in-claude): the Create and edit files setting, uploading, switching on, calling by name and deleting a skill in Claude.
- [OpenAI, Get started with ChatGPT Work, ChatGPT documentation](https://learn.chatgpt.com/docs/get-started-with-work): switching the composer to Work.
- [OpenAI, Build skills, ChatGPT documentation](https://learn.chatgpt.com/docs/build-skills): creating a skill with skill-creator and calling it with `@`.
- [OpenAI, Skills in ChatGPT, OpenAI Help Center](https://help.openai.com/en/articles/20001066-skills-in-chatgpt): plans that support skills and where created skills are listed.
- [Google, Create & manage skills for Gemini Apps (Computer), Gemini Apps Help](https://support.google.com/gemini/answer/17094296?hl=en&co=GENIE.Platform%3DDesktop): requirements, uploading, activating, calling with `/` or `@` and deleting a skill in Gemini.

## Coach notes
Arc: this lesson is a mental model. The learner sees that a skill's description decides when it loads, then watches that happen with real requests. Two laptop periods with a return to chat between them: reading and installing the humanizer, then sending the test requests. The Test is a third short run on a draft.

Concept and check: walk through the Concept, then ask the Check your understanding question. Pick up what is right in any answer. B and C are the most common ideas: "switched on" feels like "always used". Explain that switched on means the description is in view, and the request decides. For D, agree that naming the skill works and is a useful fallback later in this mission.

Reading `SKILL.md`: no Ask on the page, so wait for the learner to report in the install step. If the learner finds steps that open links, send files or run programs, or links other than Wikipedia's, look at what they found together and leave the decision to them. Declining to install is a valid decision; the coach doesn't push. If they decline, the Concept still holds, and they can return to the install when they're ready.

Install, evidence to await: what the read found, and whether the description in the skills list starts "Rewrite AI-sounding text". Follow-up questions: "Where did you find the humanizer in your skills list?" and "Is it switched on?". If the description changed (likely only in ChatGPT, through skill-creator), the learner asks skill-creator to keep the original and checks again. Claude: if the upload fails, check the file is named `SKILL.md` inside a folder named `humanizer`, and that Create and edit files is on; on Enterprise an owner enables skills first. Gemini: **More** showing **Deactivate** means active.

Before the learner sends the test requests, ask for their guesses and repeat them back when they return, so they don't need to recall them. Hand over the three requests from the step's code block if the learner asks for one at a time.

Test requests, evidence to await: which requests showed a draft, a list of AI patterns left and a final rewrite, the result of the repeated request, and whether the name, date and numbers survived in the garden rewrites. Connect each observation to the description: a request asking to make text "sound less like AI" or to edit prose fits "Rewrite AI-sounding text" and "editing or reviewing prose for AI tells"; an email summary doesn't. Keep to what was observed: the answer's shape suggests the humanizer loaded, but it doesn't prove which instructions ran. If the repeated request gave a different result, that is useful: your AI decides afresh every chat, so judge by several runs. If every guess matched on the first try, that's a good result; the repeated or surprising request is the second case, and never manufacture a failure. If no request loaded it, the Test gives the route to call it by name.

Test: hand over the opening "Use the humanizer skill" (Claude) and the newsletter paragraph, ready to copy, if the learner has no draft of their own:
"Tidy up this paragraph for our newsletter:
We are thrilled to announce that Mira joins us as project lead. Her journey is a testament to the power of volunteering."
Evidence to await: how they asked, and whether names, dates and numbers came through. If a fact changed, the learner corrects it in the rewrite before using it. Removal: Claude **...**, **Delete**; Gemini **More**, **Delete**; ChatGPT's help pages don't describe removal.

Levels: guided learners get each instruction one at a time, and the coach explains the Raw page and zipping in plain words. Standard learners follow the page and report at each Ask. Fast-track learners can skim `SKILL.md` more fully and add a surprising request of their own in the test, such as one using the description's words for an unrelated text.

Tools: Claude chat, desktop and claude.ai use the default text. ChatGPT needs the desktop app, Work mode and a plan that allows skills; if the workspace doesn't allow skills, the learner can't install, so talk through the Concept and stop there. Gemini needs the learner to be 18 or over with Keep Activity on.

Time budget: Concept and check 3 minutes, reading `SKILL.md` 3, install 5, test requests 5, Test 4.

Review, what the coach says at the end:
- What you did: ask the learner which requests loaded the humanizer and how they asked for it on their draft, then summarise from their report only.
- What to remember: your AI picks skills by description, afresh every chat, so judge by several runs. No match? Use the description's words or the skill's name. Read others' skills before installing and after updates; a whole-repo ZIP or installer adds files to check.
- In one sentence: a skill's description decides when it loads; use the humanizer on your next AI-sounding draft.
