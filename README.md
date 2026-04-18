# Financial Independence Calculator

A clean, interactive FI calculator built with vanilla HTML, CSS, and JavaScript.
No frameworks. No build tools. Just open the file and it works.

---

## What it does

Enter your monthly expenses and the calculator tells you:

- How much corpus you need today to retire (using the 4% rule)
- How much that corpus will be worth after inflation
- How much you need to invest every month to reach that number
- A live chart showing nominal vs inflation-adjusted corpus over time

---

## Features

- **3% / 4% / 5% SWR toggle** — compare conservative vs aggressive withdrawal strategies
- **Inflation slider** — 0% to 12%, default 6%
- **Years to project** — 5 to 40 years
- **4 metric cards** — corpus today, inflation-adjusted corpus, yearly expense, monthly SIP needed
- **Dual-line chart** — nominal corpus vs inflation-adjusted corpus over time
- **Copy result** — copies a clean summary to clipboard for sharing

---

## The Math

**Required Corpus**
```
Corpus = (Monthly Expense × 12) / SWR
```

**Inflation-Adjusted Corpus**
```
Adjusted = Corpus × (1 + inflation_rate) ^ years
```

**Monthly SIP Needed** (at 12% CAGR)
```
SIP = (Target × monthly_rate) / ((1 + monthly_rate)^n - 1)
```

---

## Tech Stack

- HTML5
- CSS3 (CSS Variables, Grid, Flexbox)
- Vanilla JavaScript (no frameworks)
- Chart.js 4.4.1 (via CDN)
- Fonts: Syne + JetBrains Mono (Google Fonts)

---

## How to run locally

Just open `index.html` in any browser. No server needed.

---

## Live Demo

[nischayb99.github.io/fi-calculator](https://nischayb99.github.io/fi-calculator)

---

## Based on

- Bengen (1994) — original 4% rule research
- Trinity Study — safe withdrawal rate analysis

> Not financial advice. For educational purposes only.
