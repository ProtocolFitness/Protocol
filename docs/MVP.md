# MVP Notes

## Working name

Protocol

Tagline: Private hormone and peptide tracking.

## Core principles

- 100% local-first with no account required
- Fast, minimal-friction logging
- Optional AI insights
- Data to trends to insights

## MVP screens

1. Home / Dashboard
- Daily overview
- Protocol taken checkbox
- Quick log actions for mood, energy, sleep, and libido
- Cards for next injection, last lab summary, and weekly averages

2. Protocols
- Manage TRT, peptides, and supplements
- Show dose, frequency, and next dose time
- Add, edit, and delete protocols

3. Log / Calendar
- Calendar markers for injection days, missed doses, and logged days
- Day detail view for protocols, metrics, and notes

4. Labs Tracker
- Add lab entries with value, unit, and date
- Graph common markers over time

5. Insights
- Analyze recent logs, labs, and protocol data
- Return observations, possible explanations, and things to watch

6. Settings
- Export and import data
- Clear local data
- Privacy information

## Data model

- `protocols`
- `logs`
- `daily_metrics`
- `labs`
- `symptoms`
- `ai_insights`

## Notifications

- Injection due reminder
- Daily log reminder
- Missed dose reminder

Use local notifications only.

## AI constraints

- No medical advice
- Observations instead of prescriptions
- Short, practical output

## Non-goals

- Social features
- Cloud sync
- Wearables
- Auto lab parsing
- Community stacks

## Delivery focus

Ship a clean offline tracker first. Avoid scope creep.
