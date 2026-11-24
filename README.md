## Jacques Tseng

Statistics & Machine Learning at Carnegie Mellon, class of 2029.

I build systems that have to keep running after I stop looking at them.

**[hindcast.ai](https://hindcast.ai)** — a public scoreboard for how accurately prediction markets resolve. A Python pipeline scores 11,000+ resolved Polymarket markets on Brier score and calibration, and a statically-exported Next.js site republishes itself daily with no manual step. Current finding: Polymarket is well calibrated at the tails, and the error sits at the coin-flip band, where markets priced 40–60% resolve YES 10–17 points less often than their price.

**Automated trading system on Kalshi** *(private)* — 8 strategy modules behind a shared interface, real-time WebSocket market data, position reconciliation against exchange state, and an automated kill-switch that disables a module after three consecutive losing weeks on rolling Sortino, hit rate and return. It ran live with real capital. It did not find an edge, and the kill-switch is what caught that, on its own, before I did. That turned out to be the part worth building.

**Closing line value model** — Flask over a 20-table SQLite warehouse with four scheduled collectors, an XGBoost model with SHAP attribution and a calibration table, and a vectorized Monte Carlo bankroll simulator.

The thread is calibration: how you know whether a forecast, a model, or a strategy is actually any good, and what you do the moment the evidence says it isn't.

jacquestseng1@gmail.com
