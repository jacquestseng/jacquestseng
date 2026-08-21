<!-- Repo: jacquestseng/jacquestseng — renders at the top of your GitHub profile.
     Rewrite in your own voice. Short is better than complete. -->

## Jacques Tseng

Statistics & Machine Learning + Behavioral Economics @ Carnegie Mellon, class of 2029.

I build systems that have to keep running after I stop looking at them.

**[hindcast.ai](https://hindcast.ai)** — a public scoreboard for how accurately prediction
markets resolve. A Python pipeline grades 30,000+ resolved Polymarket markets on Brier
score and calibration, and a statically-exported Next.js site republishes itself daily
with no manual step. Current finding: Polymarket is well calibrated at the tails
(markets priced ~1% resolve YES about 1% of the time) and mildly underconfident in the
middle of the distribution.

**Automated prediction-market trading system** *(private)* — 8 strategy modules behind a
shared interface, real-time WebSocket market data, position reconciliation against
exchange state, and an automated kill-switch that disables a module after three losing
weeks on rolling Sortino / hit-rate / return. It ran live with real capital. It did not
find an edge — and the kill-switch is what caught that, on its own, before I did. That
turned out to be the part worth building.

**Quantitative research dashboard** — Flask over a 20-table SQLite warehouse with nine
scheduled collectors, an XGBoost closing-line-value model with SHAP attribution, and a
vectorized Monte Carlo bankroll simulator (10k × 500 paths in 0.4s).

The thread is calibration: how you know whether a forecast, a model, or a strategy is
actually any good — and what you do the moment the evidence says it isn't.

📧 jacquestseng1@gmail.com · [LinkedIn](https://www.linkedin.com/in/jacques-tseng-492645316)
