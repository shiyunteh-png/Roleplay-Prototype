# Roleplay practice plan

The biggest drop-off in the data is advisors who come back to the app after a session, then leave without starting another one. This prototype gives them a clear next step: a personal practice plan built from their lowest-scoring skill, which becomes the first thing they see when they return.

## Running it

Open `index.html` in a browser. There's no build step and nothing to install.

Or use the live version: **[https://shiyunteh-png.github.io/Roleplay-Prototype/roleplay-practice-plan/]**

## What to try

1. Start any roleplay and end the call. The conversation and scores are simulated.
2. On the result screen, scroll to **What to work on next**, choose a pace and build a plan.
3. Edit the plan if you like (swap, remove or add sessions), pick a practice time and save.
4. Press **Close and reopen app** to see what an advisor sees when they come back.

The buttons above the phone are demo controls, so you can show several weeks of use in a few seconds:

| Control | What it does |
| --- | --- |
| Close and reopen app | Shows the app as a returning advisor sees it |
| Jump a week ahead | Moves the date forward a week, so you can see missed sessions roll over |
| Finish the plan | Completes every remaining session and shows the end-of-plan summary |
| Reset | Clears everything and starts again |

## What's in it

- **After a call:** the lowest-scoring section becomes the focus. The advisor can add other areas and choose 1 to 5 sessions a week.
- **The plan:** 4 weeks, getting harder as it goes, with a reason shown for every session. It can be edited at any time and added to Google Calendar or Outlook.
- **Returning:** "My plan" replaces the full list as the first screen, with this week's sessions one tap away. "All practice" keeps the full library.
- **Missed sessions** move to the next week and the plan shifts back, so a week never holds more than the advisor chose.
- **End of plan:** a summary of how the focus skill moved, every section before and after, and a next plan built from the latest result.

Progress is private to the advisor. There are no leaderboards, streaks or manager views.

## Notes

- Everything is in one file: HTML, CSS and plain JavaScript, no frameworks.
- The 33 scenarios and 4 rubrics come from the case data pack.
- Progress is saved in the browser (localStorage), so it stays when you refresh but not across browsers or devices.
- The recommendation is rule-based rather than a model, so each suggestion can be explained: same conversation type as the weak skill, a new customer each time, and a harder level in weeks 3 and 4.
