# Perintis: Actuarial & Personal Cashflow Simulator (v0.1.2)

An interactive, zero-dependency personal finance and life-risk simulator built with vanilla HTML, CSS, and JavaScript. Designed to model daily cashflow dynamics, liquidity crunch, compounding debt, and human-capital trade-offs for a fresh graduate navigating Jakarta's cost of living.

🔗 **Live Demo:** [Insert your GitHub Pages link here]  
*(Note: The in-game UI is localized in Bahasa Indonesia to reflect real-world Jakarta economic parameters.)*

---

## 🎯 Actuarial & Quantitative Modeling Focus
As an Actuarial Science undergraduate (STMA Trisakti), I built this project to translate foundational financial mathematics and risk management concepts into a playable deterministic-to-stochastic engine:

- **Liquidity & Working Capital Risk:** Models a 22-day initial liquidity gap before the first paycheck arrives (starting Jan 4 with Rp3,000,000 cash against a Jan 25 payday), tracked via a 30-day rolling **Savings Rate** and **Emergency Runway** (cash divided by essential monthly expenses).
- **Compounding Debt Dynamics:** Automatically triggers an emergency loan (*Pinjam Darurat*) upon cash deficit with a daily compounding interest rate of **$0.4\%/\text{day}$** ($\approx 12.7\%$ over 30 days) and a strict insolvency ceiling at **Rp4,000,000**.
- **Frequency–Severity Prototype:** Implements progressive burnout penalties—depleting stamina forces a 1-day productivity loss (skipping work and XP) alongside escalating medical costs (**Rp400,000** $\rightarrow$ **Rp650,000** $\rightarrow$ **Rp1,000,000**)—serving as the structural foundation for health insurance pricing in `v0.4`.
- **Human Capital & Diminishing Returns:** Features a skill progression curve with increasing XP requirements ($10 + 5 \times \text{level}$) tied to biannual HR performance reviews (January & July, $2\%$ raise per level gained, capped at $8\%$ per cycle) and a side-hustle revenue multiplier (up to $1.50\times$).

## 📊 Economic Calibration (Jakarta 2026 Baseline)
- **Starting Net Income:** Rp6,000,000/month (calibrated slightly above the verified 2026 DKI Jakarta Provincial Minimum Wage / UMP of Rp5,729,876).
- **Fixed Monthly Obligations (1st of Month):** Boarding house / *kos* (Rp1,800,000), utilities & laundry (Rp200,000), and mobile data (Rp100,000).
- **Daily Variable Trade-offs:**
  - *Nutrition:* Budget (Rp30k, $-5$ stamina), Standard (Rp45k, neutral), or Quality (Rp75k, $+5$ stamina).
  - *Commute (Weekdays):* Public transit KRL/TransJakarta (Rp25k, $-5$ stamina) vs. Ride-hailing / *Ojol* (Rp50k, neutral).
- **Overtime Compensation:** Rp120,000 per 2-hour session ($-25$ stamina), following Indonesian labor law multipliers ($1.5\times$ first hour, $2\times$ subsequent hours on a $\frac{1}{173}$ hourly base).

## 🗺️ Development Roadmap
- [x] **v0.1.2:** Core daily cashflow engine, stamina/burnout mechanics, biannual salary reviews, and daily compounding emergency loans.
- [ ] **v0.2:** In-game smartphone investment module (Money Market Funds, IDX30 Equities, Crypto) powered by daily **Geometric Brownian Motion (GBM)** and **Max Drawdown** tracking.
- [ ] **v0.3:** Weekend micro-business simulation (*warkop* / food stall) modeling daily customer footfall via a **Poisson Distribution**.
- [ ] **v0.4:** Stochastic life shocks (illness, vehicle breakdown, layoff risk) paired with actuarial micro-insurance policies.
- [ ] **v0.5:** End-of-year scoring system, risk-profile classification, and financial summary analytics.

## 🛠️ Tech Stack
- **Frontend & Engine:** Single-file Vanilla JavaScript (ES5/ES6 compatible), CSS Custom Properties (automatic Light/Dark mode), and `localStorage` state persistence.

---
*Disclaimer: All figures and simulations in this repository are quantitative educational models and do not constitute financial or investment advice.*
