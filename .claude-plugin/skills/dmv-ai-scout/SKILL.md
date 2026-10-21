---
name: dmv-ai-scout
description: Finds upcoming core AI/ML conferences, summits, meetups and trainings in the DC/Maryland/Virginia (DMV) area and emails a report of only NEW events via Gmail. Use when asked to run the DMV AI scout, check for new AI events in the DMV, or send the AI events digest.
---

# DMV AI Conference Scout

## Goal
Every run, find AI events in the DMV that haven't been reported before,
and email them to me as a short digest.

## 1. Check memory (what's already been reported)
- In Gmail, search: `subject:"DMV AI Scout"`.
- Read the past digests and note every event name already reported.
- Those events are "already reported". Skip them later.

## 2. Search
Run separate web searches. Don't combine them into one query.
- "AI conference Washington DC", "AI summit Northern Virginia",
  "machine learning conference Maryland", "generative AI meetup DC"
- Meetup.com and Eventbrite AI events in DC, Arlington, Reston,
  Tysons, Bethesda, Baltimore
- University calendars: GMU, UMD, Georgetown, GWU, JHU, UMBC, Virginia Tech (Alexandria)

## 3. Filter rules
- Location: DC, Maryland, or Virginia (in person or hybrid only).
- Topic: CORE AI/ML only (AI, ML, generative AI, LLMs, agents, data science).
  Exclude events where AI is only a side topic (cybersecurity, data centers, general GovTech).
- Include free meetups AND paid trainings/workshops.
- Date: drop any event whose end date is before today.
- Drop anything on the "already reported" list.

## 4. Collect for each new event
Name, date(s), city + venue, format (in person/hybrid), registration fee
(early-bird or student price if listed), organizer, official registration link.
- Open the event's OFFICIAL page or registration page. Don't rely on
  aggregator sites for the fee or the link.
- If the fee isn't on the official page, write "Not listed". Never guess.

## 5. Send the email
- Use Gmail to send to: - Use Gmail send_message to the user's own Gmail address (the account connected to Gmail)
- Subject: `DMV AI Scout – New events – <today's date>`
- Body: a table sorted by date with the fields above, then one line
  saying how many events were checked and how many were new.
- If nothing is new, still send a short email: "No new DMV AI events today."
