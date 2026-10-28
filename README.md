# AEC Skills

A library of skills for architecture, engineering, and construction firms. A skill is a prompt on a shelf: a procedure written once, in plain text, that your AI reads before it starts. Recall it, reuse it, share it.

Everything here is generic by design. Nothing from any one company is inside. Take a skill, change the voice and the minimums to yours, and build off it.

Started at the Association of Women Contractors of Minnesota session "AI for Business: A Practical Intro" (October 28, 2026, Peyton Kringlie, LS Black Constructors). More skills get added as they are written.

## The library

| Skill | What it does |
|---|---|
| `meeting-recap` | Notes or a transcript in, a follow-up email out, in your voice. Decisions, action items with a name and a date, open questions. |
| `coi-checker` | A subcontractor's certificate of insurance against your minimums. Lists every gap and what to ask the agent for. |
| `bid-letter-polish` | A bid or proposal letter in your company's voice, plus a pre-send checklist. |

Coming as they are written: submittal-review, rfi-draft, pay-app-check, daily-report, owner-update, prequal-packet, lessons-learned, punch-list.

## The short way

Open your AI assistant and say:

> Download the skills from https://github.com/pkringlie/aec-skills and install them.

If it can reach the web and your account allows skills, it will do the rest. If it cannot, use the steps below.

## The manual way (claude.ai)

1. Download `aec-skills-starter.zip` (all three starters) or one skill's zip from this page. Unzip it so you have one zip per skill.
2. Sign in at claude.ai with your company email. Click your initials, then Settings, then Capabilities, and make sure Code execution and file creation is on. On a Team or Enterprise plan an owner also turns on Skills under Organization settings.
3. Go to claude.ai/customize/skills. Click +, Create skill, Upload a skill, and pick one skill's zip.
4. Start a new chat. Type / and pick the skill, or just say what you want: "Recap these notes." Read the result and fix what it got wrong. That fix is the training.

If the Skills page is not on your plan, open Projects, create a project, and paste the text of `SKILL.md` into the project instructions. Same result, different door.

## Make it yours

Each `SKILL.md` has a short voice or minimums section near the top. Edit it in Notepad, re-zip the folder (the folder must sit at the root of the zip and match the skill name), and upload again.

## Add one

Wrote a skill your crew would use? Open a pull request with the folder and its `SKILL.md`, or email it. Keep it generic: no company names, no job numbers, no pricing, nothing personal.

## Ground rules

No SSNs, pay data, bank information, or client confidential material in a free tool. Company work on a company account. Someone who knows what right looks like reviews the output before it leaves the building.

Questions: pkringlie@lsblack.com
