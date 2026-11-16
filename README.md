# Hiring Funnel Math

A free, single-page calculator for recruiters. Tell it how many hires you need and by when, and it works backwards to the outreach volume, daily targets and pipeline you need at every stage.

**Live tool:** https://isaacthekiosk.github.io/hiring-funnel-math/

## What it does

- **Answer first:** "Reach out to 404 people by Dec 12, about 21 a working day, to make 1 hire by Jan 30."
- **Feasibility check:** flags when the plan exceeds your daily outreach capacity, or when the date is too soon, and gives the realistic hire date.
- **Full pipeline:** contacted → replied → in process → screened → onsite → offer → hire, with totals and weekly targets.
- **Your rates vs. benchmark:** every conversion rate is pre-filled from 2025 benchmarks and editable, with a +/- comparison.
- **Presets** for 14 departments and three candidate sources (sourced, inbound, all).
- **Copy plan:** a plain-text summary to paste into Slack or send to a hiring manager.

## How the math works

1. Hires ÷ offer acceptance = offers needed, and so on up the funnel to candidates in process.
2. For sourced candidates, in process ÷ (contacted → in process rate) = people to contact.
3. Pipeline cutoff = hire-by date − median days to hire. Outreach closes earlier still, by the reply lag.
4. Contacts ÷ working days in the window = daily outreach target.

The model assumes every candidate enters the process by the cutoff and moves at the median pace. Use it for planning and capacity conversations, not as a guarantee.

## Benchmark data

Default rates come from Gem's *2026 Recruiting Benchmarks Report* (data from June 2024 to May 2025):

| Source | App → Screen | Screen → Onsite | Onsite → Offer | Offer → Hire | Median days |
|---|---|---|---|---|---|
| All sources | 8% | 19% | 39% | 82% | 24 |
| Inbound | 6% | 16% | 37% | 81% | 24 |
| Sourced | 86% | 18% | 22% | 73% | 41 |

Email outreach (sourced): 23% reply rate and 8% converted to process, both as a share of everyone contacted.

Department rates cover all sources. When you pick **Sourced** with a department, the first-screen rate uses the sourced benchmark (86%) and later stages use the department's rates. That blend is an estimate.

This project is independent and not affiliated with or endorsed by Gem.

## Run it

No build step and no dependencies. Open `index.html` in a browser, or serve it with GitHub Pages:

**Settings → Pages → Deploy from a branch → `main` / root**

## Contributing

Ideas and pull requests are welcome: new presets, a capacity planner across multiple reqs, or saved scenarios.

## Author

Built by **Isaac Kironde**, founder of TheKiosk. Executive search and embedded talent partner.
[LinkedIn](https://www.linkedin.com/in/isaackironde)

MIT License.
