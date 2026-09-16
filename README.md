# Woosub Shin

**Probabilistic Market Research · Market Microstructure · Systematic Trading**

I build quantitative research systems that turn market hypotheses into reproducible evidence.

My current work is moving below repeated bar-level strategy search into **event-level Bitcoin market microstructure and high-frequency research**. The focus is not simply to make forecasts faster, but to study whether observable order-flow and liquidity states change fill probability, post-fill markouts, adverse selection, and ultimately cost-adjusted passive-execution payoff.

Prior probabilistic, volatility, and bar-based studies remain retained as frozen evidence rather than being rewritten around the new direction.

## Current Research Direction

```text
5m / 1m market context and retained evidence
    ↓
Event-level trades, quotes and order-book updates
    ↓
Local order-book reconstruction
    ↓
OFI · microprice · spread · depth · trade imbalance
    ↓
Fill probability + adverse-selection analysis
    ↓
1s / 5s / 10s / 30s / 60s markouts
    ↓
Cost-aware passive-execution payoff
    ↓
Strategy / execution consideration only after validation
```

The engineering track is moving toward a **C++ event-driven market-data and deterministic replay core**, with Python retained for statistical analysis, experiment design, payoff studies, and validation.

The key separation remains deliberate:

```text
predictive evidence
        ≠
economic utility
        ≠
strategy approval
        ≠
execution authority
```

## ASRA — Probabilistic Market Research

ASRA is my private research framework for studying Bitcoin market states, forecast decomposition, distributional prediction, and decision-making under uncertainty.

The research evolved from asking **“Which strategy works?”** to asking:

- **Will the market make a meaningful move?** → `P(MOVE)`
- **If it moves, which direction is more likely?** → `P(Direction | MOVE)`
- **How large could the move be?** → conditional magnitude distribution
- **What does the full signed return distribution look like?** → structured probabilistic forecast

### Latest frozen evidence

In the current 1-hour full-return-distribution study:

- **22,573** unique hourly forecast origins were evaluated.
- The structured return distribution outperformed a training-only unconditional empirical distribution on **CRPS in all 11/11 chronological evaluation folds**.
- The registered **7-day and 30-day block intervals were both entirely favorable**.
- Conditional magnitude information added incremental distributional value.
- The registered **left-tail score also improved** versus the unconditional baseline.

Just as importantly, some hypotheses did **not** survive:

- A separate direction-specific magnitude model did not add robust value over the pooled-magnitude structure.
- The derived conditional mean did not establish lower MSE than a zero-return forecast.

Those nulls are retained rather than tuned away. The next active research layer moves into event-level market microstructure rather than extending bar-based strategy search.

> Current evidence is retrospective and based on reused history. It is not expected-profit evidence, strategy approval, or trading permission.

## Selected Research

### Volatility Regime Filtering in Futures Markets

MSc thesis on whether EGARCH-conditioned volatility regimes improve the risk-adjusted performance of an intraday futures framework relative to the same rules without the filter.

- Daily EGARCH(1,1) with Student’s t innovations
- 5-minute equity-index futures research
- Out-of-sample and walk-forward validation
- Bootstrap ablation tests
- Alternative volatility-filter comparisons
- Explicit transaction-cost and drawdown analysis

Selected results from the final research specification included an OOS Sharpe of approximately **1.24** and a long-horizon walk-forward Sharpe around **0.94**.

- [Project summary](https://meanydeany.com/projects/volatility-regime-filtering)
- [Thesis PDF](https://meanydeany.com/papers/volatility-regime-filtering-thesis.pdf)

### Bitcoin Bubble Detection with GSADF

Seminar research applying explosive-root testing to Bitcoin price dynamics and bubble episodes.

- GSADF explosive-root testing
- Bubble / non-bubble return and volatility comparison
- Explicit separation between statistical bubble detection and trading signals

- [Paper PDF](https://meanydeany.com/papers/bitcoin-bubble-gsadf-seminar-paper.pdf)

## Research Workflow

I use AI-assisted development tools such as **Codex** and **Claude** to accelerate implementation, testing, and review, while keeping the research question, evaluation criteria, interpretation, and scientific boundaries explicit.

Typical workflow:

1. define the hypothesis and comparison before inspecting outcomes;
2. freeze data, features, models, horizons, and decision rules;
3. authenticate source and lineage identities;
4. run causal / anti-lookahead validation;
5. preserve successful and failed results;
6. separate forecast quality from economic and execution claims.

## Technical Stack

**Quantitative research**  
Python · pandas · NumPy · scikit-learn · statsmodels · ARCH/GARCH-family models · bootstrap inference · walk-forward validation · probabilistic forecasting

**Research infrastructure**  
SQL / SQLite · Git · GitHub Actions · Linux · AWS Lightsail · reproducible CLI workflows · immutable manifests · SHA-256 provenance

**Systems direction — current build**  
C++ · event-driven market data · order-book reconstruction · deterministic replay · timestamp / sequence validation · latency measurement · microstructure feature generation

**AI-assisted workflow**  
Codex · Claude · structured protocol generation · code review · test generation · reproducibility audits

## Current Interests

- Market microstructure and high-frequency research
- Passive execution, fill probability and adverse selection
- Order flow, liquidity and short-horizon markouts
- Probabilistic forecasting and distributional prediction
- Systematic / quantitative trading research
- Decision-making under uncertainty
- Multi-asset systematic research

## Portfolio

- [meanydeany.com](https://meanydeany.com)

## Contact

- Email: **woosub815@gmail.com**
- GitHub: **[@MeanyDeany](https://github.com/MeanyDeany)**

> Core research and execution repositories are private. Public pages summarize methodology and selected validated results without exposing strategy or execution internals.
