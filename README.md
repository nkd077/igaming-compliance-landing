# Compliance-ready landing page (iGaming)

A landing page for a fictional licensed online casino, built for paid traffic such as
YouTube Masthead, which opened to certified online gambling advertisers on
21 October 2026. The page changes by visitor country and keeps the rules an
ad platform and a regulator check for in plain view.

**Live demo:** `https://nkd077.github.io/igaming-compliance-landing/`

## Try it

Use the bar at the top of the page:

- **United Kingdom:** sign-up open, welcome offer with its key terms right under it, GAMSTOP and the national helpline
- **Netherlands:** Dutch, `.nl` domain, KSA licence, the monthly deposit thresholds that trigger an affordability check, and CRUKS self-exclusion
- **Brazil:** closed, with the reason shown: Provisional Measure 1.394/2026 banned betting and online gambling, and licensed sites went offline on 6 October 2026
- **Germany, United States, Russia:** no licence, so sign-up and games are switched off

**Create account** runs the full flow: date-of-birth check (under 18 locks sign-up for the session),
a required deposit limit (daily, weekly or monthly, in £ or €), then the hand-off point for identity checks (KYC).

Dashed labels on the page (G1, A1, R1 …) point to the compliance map at the bottom.

## Compliance map

| ID | Requirement | How the page handles it |
|---|---|---|
| G1 | Serve only licensed markets | country check before any call to action renders; Brazil closed after its 2026 ban |
| A1 | Age verification before play | date-of-birth gate on sign-up, then KYC |
| A2 | Clear 18+ signal | persistent 18+ mark in the header |
| T1 | Significant terms beside the offer | key conditions directly under the headline offer |
| M1 | Market-specific rules | Dutch build shows the €300 (18–24) / €700 (25+) monthly deposit check |
| R1 | Responsible gambling information | limits, reality checks, time-out, self-exclusion, helpline |
| I1 | Game information before play | RTP and house edge on every game tile |
| L1 | Licence disclosure | regulator and licence reference per market |
| C1 | Cookie consent | reject and accept carry equal weight |

Requirements differ by market and change over time. In a real project they come from the
operator's compliance team; this page shows how they are implemented and tested.

## Tech

One static `index.html`: HTML, CSS and vanilla JavaScript, no build step and no tracking.
The roulette wheel is drawn on a canvas with the real European pocket order.

## Related projects

- [Paid media payback dashboard](https://github.com/nkd077/igaming-marketing-dashboard): which channels pay back, and when
- [Acquisition KPI Telegram bot](https://github.com/nkd077/igaming-kpi-telegram-bot): daily digest and anomaly alerts

---

Fictional brand built as a portfolio demo by **nkd077**. No real-money play.
