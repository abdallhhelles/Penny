# Penny Research: the financial health model

**Edition 2026.10** (Penny 1.0.7) · maintained by the Penny Research team

Penny's Financial Health Report, the Overview's Money health card, Insights and every "?" explanation hold your numbers against one set of benchmarks. This page explains each benchmark, the evidence behind it, and the analysis the team ran before changing it. The app shows the benchmarks as Penny Research guidelines without citations; the evidence lives here.


## 1. What the latest evidence says

| Finding | Evidence (most recent available) |
|---|---|
| About **31%** of US households are financially healthy (score 80+), unchanged for five years; **17%** are vulnerable, the joint-highest since 2018. Only **47%** spend less than they earn, **68%** pay all bills on time, **31%** say their debt is unmanageable. | Financial Health Network, *Financial Health Pulse 2026 U.S. Trends Report* (survey April–May 2026); 2025 report: 31% healthy, 15% vulnerable |
| **63%** of US adults would cover a $400 emergency with cash or its equivalent, flat for four years and down from 68% in 2021. | Federal Reserve, *Economic Well-Being of U.S. Households in 2025* (SHED, May 2026) |
| Worldwide, about **56%** of adults could reliably raise emergency money within 30 days; 79% now have an account. | World Bank, *Global Findex Database 2025* (July 2025) |
| **24%** of UK adults have low financial resilience; 21% have under £1,000 for an emergency. | FCA, *Financial Lives 2024* (published 2025) |
| Having at least **$2,000** of emergency savings is linked to **21% higher** financial well-being, the largest effect measured, after controlling for income and wealth (correlational). | Vanguard, emergency savings and financial well-being (12,443 investors, CFPB scale, April 2025) |
| About **six weeks of take-home pay** covers a simultaneous income dip and expense spike; a dip alone needs ~2.8 weeks, a spike ~2.6. | JPMorgan Chase Institute, *Weathering Volatility 2.0* (2019; still the reference study, no newer edition) |
| Long-run saving guidance converges on about **15% of pre-tax income**, including employer contributions; more if you start late. | Fidelity; T. Rowe Price (2026 guidance) |
| Safe starting withdrawal rate **3.9%** for 2026 (30 years, 90% success), up from 3.7% for 2025; flexible spending allows more. | Morningstar, *The State of Retirement Income for 2026* |
| 10-year return outlooks are modest: US equities about **3.9–5.9%** a year, non-US 4.9–6.9%, US bonds about 4–5%, core inflation about 2.6%. A balanced portfolio therefore expects roughly **2.5–3% after inflation**. | Vanguard, *2026 Economic and Market Outlook* and capital-markets model (Jan 2026); Morningstar experts' forecasts, 2026 edition |
| Average interest on credit-card balances that accrue interest: **21.5–22.4%** in 2026. | Federal Reserve G.19 (accounts assessed interest), Q1–Q2 2026 |
| Half of US renters spend more than **30%** of income on housing (cost-burdened), 27% more than **50%** (severely). | Harvard JCHS, *State of the Nation's Housing 2025* |
| The 43% debt-to-income cap was removed from the US Qualified Mortgage rule in 2021 (now price-based); 36% remains the common guideline for total debt payments. | CFPB, General QM final rule (Dec 2020) |
| Concentrating repayments on one debt at a time keeps people going; highest-rate-first costs least. No newer behavioural study supersedes this. | Gal & McShane, *Journal of Marketing Research* (2012) |

## 2. The model

Four pillars, each scored 0–100; the total is their average. Tiers follow the Financial Health Network's: **80+ healthy, 40–79 coping, under 40 vulnerable**. Each measure scores linearly between a "weak" end (0) and a "good" end (100).

| Pillar | Measure | Weak → good | Why |
|---|---|---|---|
| Spend | Spending vs income | spending 5% above income → 5% below | Living within your means is the base of every other goal; half of households fail it |
| | Essentials share of income | 65% → 50% | 50/30/20 split; above 65% leaves little room for anything else |
| | Bills you confirm yourself, paid on time | each overdue bill −34 | On-time payment is one of the eight FinHealth indicators; only 68% manage it |
| Save | Savings rate | 0% → 15% | Long-run saving guidance |
| | Cash buffer, months of essentials | 0 → target (3 / 4.5 / 6) | The single habit most tied to well-being; target rises with income volatility |
| Borrow | Debt payments / gross income | 43% → 36% | Lender guideline; 43% was the old QM cap |
| | Debt owed / a year of income | 100% → 20% | Debt load relative to what you earn |
| | Average interest rate | 20% → 8% | Expensive debt outruns any saving |
| | Cap | 70 while any debt costs 15%+ a year | Card debt at ~22% should be cleared before investing |
| Plan | Years until savings alone cover spending | 70 → 40 years | See finding 4 below |
| | Dated goals covered by usual monthly savings | 0% → 100% | A goal your savings can carry is one you reach |
| | Spending covered by budgets | 20% → 80% | Planning ahead, measured by behaviour |

Other benchmarks used across the app: savings tiers 5 / 10 / 15 / 20%; housing 30% (burdened) and 50% (severe); buffer target 3 months for steady income (variation under 10%), 4.5 for variable (under 25%), 6 for irregular or unknown; first rung six weeks of take-home pay; withdrawal rate 3.9%; real return 3%.

## 3. Analysis: what the team found in the 1.0.6 model

We scored five reference households (six months of transactions each) with the old and new models.

| Household | Old total | New total | New tier |
|---|---|---|---|
| Meets every benchmark (15% saved, 3 months' buffer, invests, budgets, goal on pace) | 75 | **97** | healthy |
| Typical: 2.5% margin, under 1 month's buffer, $6,200 card debt at 22% | 24 | **47** | coping |
| Spends more than it earns, two overdue bills, card + car loan | 14 | **20** | vulnerable |
| High saver with irregular income (28% saved, 6.7 months' buffer) | 85 | **96** | healthy |
| Debt-free, 6 months' buffer, saves under 3% | 51 | **57** | coping |

1. **The old model counted one number twice.** Spend scored "income minus spending" from 0 to 15%, and Save scored the savings rate, the same quantity, from 0 to 15%. A household saving little lost on both pillars, which is a large part of why the typical household fell to "vulnerable" (24) even though survey data puts most such households in "coping". Spend now asks only whether you live within your means (full credit at a 5% margin) and adds on-time bills; Save measures how much you keep.
2. **Debt was measured against assets Penny cannot see.** Debt ÷ assets uses only the accounts in Penny; for renters the biggest assets (car, home contents) are missing, so modest card debt read as insolvency. Debt is now measured against a year of income, which Penny knows well.
3. **Screens disagreed.** The Overview wanted a 6-month buffer and a 20% savings rate; the Report wanted 3–6 months depending on income stability and gave full credit at 15%. Every screen now reads the same targets.
4. **The independence clock was a "retire early" yardstick.** At today's expected returns (3% after inflation) and a 3.9% withdrawal rate, a household saving 15% from zero needs about **57 years** before savings *alone* could cover its spending. The 15% guideline works because a state pension or social security carries part of retirement, which Penny does not count. The old model gave full credit only at 25 years, reachable with savings rates near 40%, so a household doing everything right scored 0 on Plan. Full credit now starts at 40 years (about what saving 25% from zero reaches), none at 70, and Plan also counts goals and budgets.
5. **The return assumption was above current forecasts.** 4% after inflation sits above every major 2026 outlook for a balanced portfolio; the default is now 3% (2–5% selectable). People who never changed it move to 3%; a choice made in the Report is kept.
6. **Housing used a mortgage-underwriting line (28%).** The cost-burden lines used in housing research are 30% and 50%.
7. **The first emergency step was arbitrary.** It was "one month of essentials"; it is now six weeks of take-home pay, the amount that covers a simultaneous income dip and expense spike.

## 4. Limits

- Benchmarks are guidelines, not advice; several come from US data. Penny marks country-specific rules and shows dollar thresholds only for US dollars.
- The model sees only what is in Penny: no credit score, no insurance, no pensions, no employer contributions.
- The reference households are synthetic. They check that the model ranks situations sensibly; they are not a population survey.

