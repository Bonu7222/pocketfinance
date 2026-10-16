# 💎 pocket

> personal finance tracker that doesn't suck

a chill little app to track your money — income, expenses, charts, the whole vibe. built it for **snowglobe** and honestly it's the biggest thing i've made so far.

## what it does

- 💸 add income + expenses with categories, dates, and notes
- 📊 see where your money goes with a **doughnut chart** (by category)
- 📈 watch your **cash flow** over the last 7 / 30 / 90 days
- 🔍 search + filter transactions (by type, category, date range)
- 🌗 dark & light mode that actually looks good in both
- 💾 everything saves to localStorage, so it's still there when you come back
- 🎨 glassmorphism UI with an animated aurora background

## what i learned

this project was a whole journey ngl. here's the stuff that actually stuck:

- **chart.js** — first time using it. learned how to build doughnut + line charts, make them theme-aware, and update them live when data changes. the trick was destroying and re-creating them when the theme flips 🌗
- **state management** — no framework, just plain JS. keeping `transactions` as the single source of truth and re-rendering from it made life way easier
- **localStorage** — saving + loading JSON, handling the case where it's empty or corrupted
- **CSS custom properties** — using `--var` for theming meant i could switch dark/light with one attribute on `<html>`
- **glassmorphism** — `backdrop-filter: blur()` + semi-transparent backgrounds is the cheat code for pretty UI
- **debugging my own typos** — genuinely learned more from fixing dumb mistakes like `localCompare` vs `localeCompare` than from writing new code lol

## stack

- plain **html + css + js** (no frameworks, no build step)
- **chart.js** via CDN for the graphs
- **inter** + **jetbrains mono** from google fonts
- data lives in **localStorage**

## shortcuts

- `n` — new transaction
- `/` — focus search (not wired yet, coming soon lol)
- `esc` — close modal

## what's next (maybe)

- [ ] monthly budget limits with warnings
- [ ] custom categories (right now they're hardcoded)
- [ ] csv export / import
- [ ] recurring transactions
- [ ] multi-currency

---

made with too much coffee and a lot of `console.log()` ☕

btw, i ofc used ai but not for a whole thing, partly. ah whatever, it was so helpful cuz i learned a lot as i mentioned. 