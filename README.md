# RupeeWise — Currency Converter & Trip Budget Planner

Convert between 10 world currencies at **live exchange rates**, and plan a whole trip's budget with expenses auto-converted to INR.

**Live demo:** https://abhiramunni.github.io/rupeewise/

## What it does

- **Currency converter** — convert any amount between INR, USD, EUR, GBP, AED, SGD, JPY, AUD, CAD and CHF, with a plain-words explanation of the result ("What this means").
- **Live rates** — exchange rates refresh automatically on every visit from free public rate feeds (open.er-api.com, with a fallback provider). A LIVE badge shows when rates were last updated; if you're offline, the app honestly says so and uses the last fetched rates.
- **Editable rates** — tap any rate to set your own (e.g. your bank's rate). Custom rates are tagged CUSTOM and never overwritten by live updates; reset individually or all at once.
- **Trip budget planner** — add trip expenses in any currency (Stay, Food, Transport, Shopping, Other), each auto-converted to INR. See totals, per-day average, and an animated spending-by-category donut chart.
- **Budget tracking** — set a trip budget and watch the progress bar fill as you add expenses.
- **Export** — copy a plain-words trip summary to share or save.

## How to use

1. **Convert tab** — enter an amount, pick the FROM and TO currencies (flags included), see the live result instantly. Tap the swap button to flip currencies.
2. **Trip Planner tab** — add each expense with its title, amount, currency and category. Set your trip length in days and an optional total budget.
3. **Rates tab** — see all live rates vs INR, refresh them manually, or tap a rate to override it with your own.

First visit shows a 30-second guided tour; every input has helper text and every result is explained in plain words.

## Tech stack

Single self-contained `index.html` — no backend, no signup, no build step. Vanilla HTML/CSS/JS with Motion One (spring animations), Three.js (3D gold coin), canvas gradient mesh, liquid-glass panels, and SVG charts. Fonts via Google Fonts, flags via flagcdn.

## Data & privacy

- All your expenses, custom rates and preferences stay in your browser (`localStorage`) — nothing is uploaded anywhere.
- Live rates are fetched from public, keyless exchange-rate APIs (open.er-api.com, fallback jsdelivr currency-api). No tracking, no cookies, no accounts.

Built as part of the daily app streak — Day 2, 14 Oct 2026.
