---
name: meeting-recap
description: Turn meeting notes, a voice memo transcript, or a messy bullet list into a follow-up email written in the user's own voice, with decisions, action items (who, what, by when), and open questions. Use this whenever the user pastes notes or a transcript and wants a recap, a follow-up, a summary email, "send this to the team", "write up what we decided", or any message that reports back on a meeting, site walk, owner call, or subcontractor meeting. Trigger even if they only paste the notes and say "clean this up".
---

# Meeting Recap

Turn raw notes into the follow-up email a busy contractor would actually send. The reader was probably in the meeting or will skim it on a phone, so the email earns its keep by being short, specific, and clear about who owes what.

## Before you write

1. Read the whole input first. Notes and transcripts bury the decision under the discussion. Find what was decided, what is still open, and who agreed to do something.
2. If the notes name people only by first name or initials, keep them exactly as written. Do not invent last names, titles, or email addresses.
3. If a due date is missing for an action item, leave it as "date TBD" rather than guessing. A made-up date in a recap becomes a real commitment.
4. Fill in the voice section below the first time the user runs this skill. Ask the user for one or two emails they have actually sent and copy the patterns you see. If they skip that, use the default voice.

## The user's voice

Edit this section so the recap sounds like the person sending it. Keep whatever is true and delete the rest.

- Greeting: "Hi all," or first names only, no "Dear"
- Sentences: short, plain, one idea each
- Tone: direct and friendly, no hype, no corporate filler
- Sign-off: first name only
- Never use em dashes. Use a comma, a period, or a colon instead.
- Things this person would never write: "I hope this email finds you well", "circle back", "synergy", "leverage"

If the user gives you sample emails, add three to five specific habits here (how they open, how they ask for things, favorite phrases, how they close).

## Output format

Produce one email, ready to paste. Use this structure every time so readers learn where to look.

```
Subject: [Meeting name] recap, [date]

[One or two sentences: what the meeting was and the single most important outcome.]

Decisions
- [Decision 1]
- [Decision 2]

Action items
- [Who]: [what], by [date or "date TBD"]
- [Who]: [what], by [date or "date TBD"]

Open questions
- [Question, and who is expected to answer it]

Next meeting: [date, time, place, or "not set"]

[Sign-off]
```

Rules that keep the recap useful:

- Lead with the outcome. If the room decided to hold the pour until the inspector signs off, that is sentence one.
- Every action item has a name. "Someone will follow up with the owner" is not an action item. If the notes do not say who, put it under Open questions as "Who owns the follow-up with the owner?"
- Keep each bullet to one line where you can. Two lines at most.
- Leave out the discussion. The reader wants the result, not the path to it. If the path matters (for example, why a change was rejected), give it one sentence under the decision.
- Drop any section that would be empty. An "Open questions" header with "None" under it is noise.
- Numbers, dates, and dollar amounts come from the notes, never from memory or inference. If the notes say "about 40k", write "about $40K".

## Examples

**Example 1**

Input (pasted notes):
```
OAC mtg 10/14 - owner (Dana), arch (Luis), us (me, Sam)
roof delay, Dana ok w/ 2 wk ext if we hold price
Luis to issue ASI for the door hardware change by fri
Sam get updated schedule out monday
still waiting on city for the fire alarm permit??? who is on that
next OAC 10/28 9am trailer
```

Output:
```
Subject: OAC recap, 10/14

Quick recap from today's OAC. Main outcome: Dana approved a two week extension on the roof as long as we hold price.

Decisions
- Two week extension on the roof, no price change (Dana approved)

Action items
- Luis: issue the ASI for the door hardware change, by Friday 10/17
- Sam: send the updated schedule, by Monday 10/20

Open questions
- Fire alarm permit is still with the city. Who owns the follow-up?

Next meeting: OAC on 10/28, 9:00 AM, job trailer

Thanks,
[Name]
```

**Example 2**

Input: a 40 minute transcript of a subcontractor coordination call with a lot of back and forth about sequencing.

Output: the same structure, with the sequencing agreement stated in one sentence under Decisions ("Mechanical rough-in starts on level 2 Monday; electrical follows on Wednesday") and each sub's commitment listed by company name under Action items. The back and forth is left out entirely.

## When the input is thin

If the notes are three words and a date, say so and ask one question instead of inventing content: "I have the date and the topic but no decisions or action items. What was decided?" A short honest recap beats a long invented one.
