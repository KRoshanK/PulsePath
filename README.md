# PulsePath

Personal habit and health tracker — *Small habits. Better health. Brighter days.*

Built 25 September 2026. This public repo is the project home for PulsePath.

> PulsePath is a habit tracker, not a diagnosis tool. Logs stay on the device (browser storage). No shared server database and no auth in the current build.

## What it does

- **Dashboard** — greeting, day score, sleep / water / exercise / meds rings, stress, screen time, steps, resting heart rate, 7-day trend, action alerts
- **Daily check-in** — sleep hours, water glasses, exercise minutes, steps, resting HR, screen time, stress, mood, medication doses, notes
- **Goals** — targets and medication schedule
- **History** — past days
- **Health Vault** — lab reports, prescriptions, visit notes, scans, emergency card (blood type, allergies, meds, conditions, contact)
- **Profile & settings**

Day score is computed from the log versus goals and active doses.

Dashboard alerts can open:
- Breathe (elevated stress)
- Set Limit (screen time over target)
- Tips (tired / low mood / short sleep)

## Routes

| Route | Screen |
| --- | --- |
| `/` | Dashboard |
| `/check-in` | Daily log (supports `?date=` and `?focus=`) |
| `/goals` | Goals and med schedule |
| `/history` | History |
| `/vault` | Records and emergency info |
| `/profile` | Profile |
| `/settings` | Settings |

## Stack

React 19, TanStack Start / Router, Zustand, Tailwind CSS v4, Lucide icons.

## Source workspace

Full generated app source from the 25 Sep 2026 App Builder session:

https://github.com/KRoshanK/umbra-garden-velvet-ivory

That workspace repo is currently **private**. Flip it to public in GitHub → Settings → General → Danger Zone if you want the complete source visible, or copy the `src/` tree into this repo.

## Privacy

- Auth: off
- Database: off
- Persistence: local to the browser
- Sample profile, goals, and meds are pre-filled so the dashboard looks complete; overwrite them anytime
