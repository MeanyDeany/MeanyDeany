# Woosub Shin

**Systematic Trading Research · Financial Econometrics · Research Infrastructure**

I build research systems for market-data validation, volatility modeling, prospective testing, and reproducible systematic-trading research.

My current work focuses on separating **source evidence, research conclusions, policy state, and execution authority** so that a good backtest or model result cannot silently become a trading decision.

## Current Focus

- Financial econometrics and empirical asset pricing
- Systematic futures and crypto-market research
- Volatility modeling and regime diagnostics
- Immutable market-data provenance and revision history
- Prospective holdouts and anti-lookahead validation
- Reproducible research infrastructure on Linux / AWS
- Longer-term multi-asset research architecture

## Selected Work

### BTC Research Assistant

Research-only infrastructure for BTCUSDT 5-minute market research, immutable source evidence, forward validation, and operational monitoring.

**Current architecture**

- Separate Binance Spot and USD-M source evidence
- Immutable observations and append-only revision history
- Exact response-page / row provenance for canonical USD-M V2 evidence
- Historical freezer validation and reproducible research artifacts
- Prospective G1 extreme-gap geometry holdout frozen before outcome inspection
- Dedicated post-maturity USD-M V2 authority builder
- Source-only readiness monitoring and fail-closed maturity gates

**Current prospective study**

```text
G1 EXTREME_GAP_LEADER_GEOMETRY
├── G1A SPOT_LEADER_EXTREME_GAP
└── G1B PERP_LEADER_EXTREME_GAP
```

Frozen candidate window:

```text
2026-08-12T00:00:00Z → 2026-10-11T00:00:00Z
```

Final outcome maturity is not before `2026-10-11T12:00:00Z`. No interim outcome look, optional stopping, or result-driven window extension is permitted.

**Public research data**

- [btc-data.meanydeany.com](https://btc-data.meanydeany.com)
- [BTCUSDT 5m JSON](https://btc-data.meanydeany.com/public/research/btcusdt-5m.json)
- [Repository](https://github.com/MeanyDeany/btc_research_assistant)

> Research boundary: no live trading, no paper-trading approval, no broker or Binance execution, no entry/short permission, no position or leverage sizing, and no strategy approval.

### Volatility Regime Filtering in Futures Markets

MSc thesis on whether EGARCH-conditioned volatility regimes improve the risk-adjusted performance of an intraday futures framework relative to the same rules without the filter.

- Daily EGARCH(1,1) with Student's t innovations
- 5-minute NQ and ES intraday futures research
- Out-of-sample testing
- Walk-forward validation
- Bootstrap ablation tests
- Alternative volatility-filter comparisons
- Explicit transaction-cost treatment and robustness checks

Selected results from the final research specification included an OOS Sharpe of approximately **1.24**, a long-horizon walk-forward Sharpe around **0.94**, and statistically significant ablation evidence versus key baselines in the frozen analysis.

- [Project page](https://woosub-shin.vercel.app/projects/volatility-regime-filtering)
- [Thesis PDF](https://woosub-shin.vercel.app/papers/volatility-regime-filtering-thesis.pdf)

### Bitcoin Bubble Detection with GSADF

Seminar research applying explosive-root testing to Bitcoin price dynamics and bubble episodes.

- [Project page](https://woosub-shin.vercel.app/projects/bitcoin-bubble-gsadf)
- [Paper PDF](https://woosub-shin.vercel.app/papers/bitcoin-bubble-gsadf-seminar-paper.pdf)

## Research Principles

```text
profitable backtest
        ≠
predictive evidence
        ≠
strategy approval
        ≠
execution authority
```

The research workflow is designed around:

1. exact and revision-aware source evidence;
2. reproducible historical testing;
3. prospectively frozen hypotheses and holdouts;
4. immutable evidence bundles;
5. manual evidence review;
6. only later, separately reviewed execution research.

## Technical Stack

**Research:** Python · pandas · NumPy · statsmodels · ARCH/GARCH-family models · bootstrap inference · walk-forward validation · time-series econometrics

**Infrastructure:** SQLite · Linux · Git · GitHub Actions · AWS Lightsail · cron · immutable manifests · SHA-256 provenance · reproducible CLI workflows

**Web / data surfaces:** Next.js · Vercel · public research-data endpoints

## Portfolio

- [meanydeany.com](https://meanydeany.com)
- [woosub-shin.vercel.app](https://woosub-shin.vercel.app)

## Contact

- Email: **woosub815@gmail.com**
- GitHub: **[@MeanyDeany](https://github.com/MeanyDeany)**
