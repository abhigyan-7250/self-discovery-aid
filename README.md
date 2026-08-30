# Journal Insights

Build a fully functional, presentation-ready MVP called AI Journal Coach.

CRITICAL REQUIREMENT

This MVP must be built and hosted entirely within Lovable.

I want to keep this project completely FREE.

Do NOT require:

Gemini API

OpenAI API

Anthropic API

Supabase

Firebase

Vercel

Any paid API

Any external backend

Any external database

Any external service that requires an API key or payment

The final result must be a working web application that I can open through a public Lovable link during a presentation.

The application should work reliably without requiring me to configure an API key immediately before the presentation.

Use client-side/local logic and realistic predefined AI responses to simulate the AI experience.

The goal is a convincing functional MVP/demo, not a production AI system.

PRODUCT

Product name:

AI Journal Coach

Core promise:

“Write about your day. We’ll help you understand it.”

This is an interactive AI journaling and reflection experience.

It is NOT:

A traditional journal that only stores entries

A generic chatbot

A consultant/problem-solving bot

A therapy application

A mental-health diagnosis tool

The experience should feel like:

“I wrote my journal, and the journal responded intelligently.”

The core workflow is:

JOURNAL → UNDERSTAND → EXPLORE → ACT

TARGET USER

Growth-oriented, habit-struggling self-reflectors.

These are users who:

Value self-reflection

Sometimes journal but aren't always consistent

Experience everyday stress, overthinking or difficult situations

Want more than simply storing their thoughts

Want to understand their experiences and identify a practical next step

CORE PROBLEM

Users can record and reflect on their day but often struggle to turn those reflections into meaningful self-understanding and actionable next steps.

A single journal entry can contain multiple situations.

The product should identify those multiple themes but should NOT attempt to solve all of them simultaneously.

IMPORTANT PRODUCT FLOW

Create exactly this primary flow:

1. JOURNAL

User writes freely about their day.

↓

2. UNDERSTAND

The application analyzes the entry and identifies meaningful themes.

↓

3. REFLECTION MAP

The application displays the themes it identified.

↓

4. EXPLORE

User chooses one theme.

The application asks contextual follow-up questions.

↓

5. INSIGHT

The application summarizes what it understood.

↓

6. ACTION

The application suggests one small, practical next step.

SCREEN 1 — WELCOME

Create a polished, modern landing page.

Headline:

Understand your day.

Subheadline:

Write freely. We’ll help you make sense of what happened.

Primary button:

Start today’s reflection

Small supporting text:

A private space to reflect, understand, and take your next step.

The design should feel:

Calm

Premium

Personal

Minimal

Modern

Do not make it look like a generic AI chatbot.

SCREEN 2 — JOURNAL

Heading:

How was your day?

Supporting text:

Write about whatever is on your mind — the good, the difficult, the confusing, or anything that stayed with you today.

Large journal textarea.

Placeholder:

“Today was…”

Primary button:

Reflect on my day

Secondary button:

Try an example

The user must be able to type their own journal.

Do NOT use a questionnaire.

Do NOT ask for a mood score.

The experience must feel like real journaling.

DEMO MODE

Because this MVP must work without an external AI API, create a reliable demo mode.

When the user clicks:

Try an example

populate the journal with:

“Today was pretty stressful. I had a presentation and kept worrying about whether people thought I was prepared. Then my friend was quiet at lunch and I kept thinking maybe she’s upset with me. I also procrastinated on my assignment again. But I went to the gym and felt much better afterwards.”

This is the primary demonstration journal.

When this exact or substantially similar journal is submitted, produce the predefined Reflection Map described below.

SCREEN 3 — REFLECTION MAP

After submission, show a short loading animation.

Example:

Reading your reflection…

Then:

A few things stood out today

Display four attractive theme cards:

Presentation

Fear of being judged

Friendship

Uncertainty and overthinking

Assignment

Procrastination and overwhelm

Workout

Improved mood

Use subtle visual differentiation between challenging, uncertain and positive themes.

Below:

What would you like to explore?

Make each card clickable.

Also include:

Something else

IMPORTANT

The Reflection Map is one of the key differentiators of this product.

The user should see that the application understood the entire journal before asking questions.

Do not immediately open a chatbot.

First show the Reflection Map.

CUSTOM JOURNAL FALLBACK

If the user writes a different journal instead of using the demo example, do NOT fail.

Create a lightweight client-side analysis system.

Use keyword/context matching to identify likely themes.

Examples:

If the journal contains:

presentation

meeting

interview

speaking

prepared

judged

identify a theme such as:

Performance
Concern about how others perceived you

If it contains:

friend

relationship

ignored

distant

argument

upset

identify:

Relationships
Uncertainty or overthinking

If it contains:

assignment

homework

deadline

procrastinate

work

scrolling

identify:

Work / Procrastination
Difficulty getting started

If it contains:

gym

workout

exercise

run

walk

identify:

Wellbeing
Improved mood after activity

If none of these match, create a generic theme:

Something on your mind
An experience that may be worth exploring further

Always display 2–4 themes when possible.

This does not need to be true AI for the MVP; it needs to create a convincing demonstration of the intended product workflow.

SCREEN 4 — EXPLORE

When the user selects a theme, open an interactive reflection screen.

The UI should resemble a thoughtful conversation rather than a generic chatbot.

Show:

Let’s explore this a little further.

For the Assignment example, use:

AI:

“You mentioned that you keep postponing the assignment even though you know it’s due Friday. When you think about starting it, what feels hardest?”

Give the user a text input.

If the user answers with something similar to:

“It feels like too much work, so I end up scrolling.”

respond:

“So the difficulty may be getting started rather than actually not having enough time. Does that feel accurate?”

Then provide response buttons:

Yes, that feels right

Maybe

Not really

If the user chooses “Yes, that feels right”, continue to the Insight screen.

OTHER THEMES

Create predefined exploration paths for:

Presentation

Question:

“You mentioned worrying about whether people thought you were prepared. What part of being judged feels most uncomfortable?”

Possible responses should lead toward:

Insight:
“It sounds like the pressure may be coming less from the presentation itself and more from how you imagine others evaluating you.”

Then:

Action:
“Before your next presentation, write down what ‘prepared enough’ actually means to you and use that as your benchmark.”

Friendship

Question:

“You noticed that your friend seemed quiet and started wondering whether you had done something wrong. What made you connect their mood to yourself?”

Possible insight:

“It sounds like uncertainty quickly turned into self-questioning, even though you didn't have clear evidence that something was wrong.”

Action:

“Next time, pause before assuming the reason and give yourself one alternative explanation for their behavior.”

Workout

Question:

“You noticed that you felt much better after your workout. What do you think changed for you?”

Possible insight:

“Your mood seemed to shift after doing something physical, suggesting that movement may be a useful reset when the day feels mentally heavy.”

Action:

“On a stressful day this week, try a short 15-minute walk or workout before deciding the day is going badly.”

USER-CONTROLLED EXPLORATION

The user should only explore ONE theme at a time.

Do not try to solve all the themes simultaneously.

Include a subtle option:

← Back to reflection map

This allows the user to choose another topic.

SCREEN 5 — INSIGHT

Create a visually distinct insight card.

Heading:

What I noticed

For Assignment:

“It sounds like the main barrier isn't lack of time. The assignment feels overwhelming because you're thinking about the entire workload at once, which makes avoiding it temporarily easier.”

Use tentative, reflective language.

Do not make clinical or absolute claims.

SCREEN 6 — ACTION

Below the insight:

One thing you could try

“Tomorrow, spend 15 minutes creating only the assignment outline. The goal isn't to finish it — just to make starting easier.”

Emphasize that this is ONE small action.

Do not generate long lists of advice.

SCREEN 7 — CLOSING REFLECTION

Ask:

Would making the first step smaller make starting feel easier?

Buttons:

Yes

Maybe

Not really

Then:

Explore another part of my day

and

Start a new reflection

AI-LIKE BEHAVIOR WITHOUT AN API

The MVP should feel intelligent even though it does not use an external AI API.

Implement:

Keyword/context detection

Theme identification

Predefined contextual questions

Response-aware follow-up logic

Predefined insight generation

Predefined personalized actions

Different responses depending on selected theme

The user experience should feel like AI-guided reflection.

Do not tell the user:

“This is a simulated AI.”

The product is a prototype demonstrating the intended experience.

UI DESIGN

Use a premium modern visual language.

Design principles:

Minimal

Calm

Personal

Spacious

Rounded cards

Soft visual hierarchy

Excellent typography

Subtle transitions

Smooth page/state transitions

Mobile responsive

Desktop presentation friendly

Avoid:

Corporate dashboard aesthetics

Excessive gradients

Overly colorful interfaces

Generic ChatGPT clone styling

Excessive animations

Clutter

The Reflection Map should be visually impressive because it is the key product moment.

NAVIGATION

Keep navigation extremely simple.

Primary flow:

WELCOME
→ JOURNAL
→ REFLECTION MAP
→ EXPLORE
→ INSIGHT
→ ACTION
→ CLOSING REFLECTION

Do not add unnecessary pages.

No login required.

No account creation.

No authentication.

No dashboard.

No settings page unless absolutely necessary.

DATA

Do not use a database.

Store the current session in local React state/localStorage where useful.

The user does not need an account.

The application should work immediately after opening the link.

MVP BOUNDARIES

Do NOT build:

Long-term memory

Emotional pattern tracking

Weekly/monthly reports

Notifications

Voice journaling

Gamification

Streaks

Therapy

Mental-health diagnosis

Multiple AI agents

Social features

Personal-growth dashboard

User accounts

Complex database

Keep the product focused on the core experience.

SAFETY

This is a self-reflection and personal-growth product.

Do not diagnose users.

Do not claim to be a therapist.

Do not make medical diagnoses.

Use language such as:

“It sounds like…”

“One possibility is…”

“Based on what you shared…”

Include a small footer disclaimer:

AI Journal Coach is designed for self-reflection and personal growth, not medical or mental-health diagnosis or treatment.

PRESENTATION REQUIREMENTS

This application will be demonstrated live during a presentation.

Therefore:

It must load quickly.

It must work without an API key.

It must not depend on external services.

It must not require login.

It must not require database configuration.

It must work on desktop browsers.

It must also be responsive on mobile.

The demo flow must be deterministic and reliable.

Include a “Try an example” button.

Make the example flow polished from beginning to end.

Preserve the user's journal if they navigate backward.

Include retry/fallback behavior if something unexpected happens.

Do not leave placeholder screens or unfinished components.

Do not display developer/debug information.

Make the application feel like a complete MVP rather than a prototype wireframe.

PRIMARY PRESENTATION DEMO

The ideal presentation flow is:

Open the public Lovable link.

Click Start today's reflection.

Click Try an example.

Click Reflect on my day.

Show the four themes.

Select Assignment.

Answer the reflection question.

Select Yes, that feels right.

Show the personalized insight.

Show the practical next action.

Return to the Reflection Map.

Explain that the same workflow can be used for any part of the user's day.

The entire flow should take approximately 1–2 minutes.

FINAL QUALITY CHECK

Before considering the app complete, verify:

The welcome page works.

Journal input works.

Example journal works.

Reflection Map appears.

All four example themes are selectable.

Assignment exploration works end-to-end.

Presentation exploration works.

Friendship exploration works.

Workout exploration works.

Insight screen works.

Action screen works.

Back navigation works.

New reflection works.

The application works without external APIs.

There are no broken buttons.

There are no placeholder components.

The public Lovable deployment can be opened directly in a browser.

The most important thing is NOT the number of features.

The most important thing is that the following experience feels polished:

I write my day → the product understands it → it shows me what stood out → I choose what matters → we reflect → I leave with an insight and one next step.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://self-discovery-aid.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/de985f12-efb5-4861-91ac-b1dc26349c8c).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
