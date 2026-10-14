# meanydeany

**Systematic Trading Research | Financial Econometrics | Market Microstructure**

I build research systems for Bitcoin trading, from market-data ingestion and interpretable signals to execution-aware backtests and reproducible experiments.

My current focus is **BTC**: studying what price, volume and observed trading behavior can tell us, then testing whether that information translates into value after fees, slippage and execution delays. My background is in financial econometrics and empirical asset pricing.

[Portfolio and papers](https://meanydeany.com) | [Email](mailto:woosub815@gmail.com)

## What I am working on

### BTC price and volume research

Interpretable strategies built from completed candles and traded volume. I turn price structure into explicit setup, entry and exit rules, then evaluate the complete trading policy rather than just a directional forecast. Price-only controls, no-trade outcomes and transaction costs are part of the comparison.

### Market microstructure and C++

Event-level trades, quotes and order-book updates; local book reconstruction; and deterministic market-data replay. The C++ track supports event-driven data processing, while Python supports statistical analysis, short-horizon price-response studies and validation. Execution research examines fillability and adverse selection separately from signal quality.

### Execution and inventory analysis

Reconstructing observed position changes from historical execution records and aligning them with contemporaneous candles and volume. I distinguish fills from orders, and separate new entries, additions, reductions, closes and reversals. A buy is not necessarily a new long position, and a fill timestamp is not an order-submission timestamp.

### ASRA and research infrastructure

ASRA is my private framework for probabilistic market research and cost-aware strategy evaluation. The supporting tooling covers source authentication, timestamp alignment, forecast evaluation, chronological testing, independent accounting checks and reproducible reporting.

Personal trading records and experimental strategy results remain separate; neither is used as a substitute for the other.

## Selected academic research

### Volatility Regime Filtering in Futures Markets

My MSc thesis investigates how daily EGARCH volatility information changes trade selection and position sizing in an intraday breakout framework for Nasdaq 100, S&P 500 and WTI crude-oil futures.

The study combines conditional-volatility modelling, five-minute market data, ablations, chronological parameter-selection exercises and alternative volatility inputs. The comparisons assess the combined filtering and exposure-control layer; they do not isolate the contribution of EGARCH asymmetry alone.

The **14 October 2026 editorial portfolio revision** clarifies the retrospective development history, information available at each decision, and execution and accounting assumptions. Historical results remain conditional research evidence: independent out-of-sample performance and several table reconciliations require a reproducible empirical rerun.

[Project summary](https://meanydeany.com/projects/volatility-regime-filtering) | [Revised thesis](https://meanydeany.com/papers/volatility-regime-filtering-thesis-revised-2026-10-14.pdf) | [Original submission](https://meanydeany.com/papers/volatility-regime-filtering-thesis.pdf) | [Revision notes](https://meanydeany.com/papers/revision-notes-2026-10-14.html)

### Bitcoin Bubble Detection with GSADF

Seminar research on right-tailed explosive-root tests and the interpretation of Bitcoin price surges. The revision distinguishes the global GSADF statistic from the BSADF sequence used to date episodes, and separates statistical explosiveness from behavioral explanations and trading signals.

The **14 October 2026 editorial portfolio revision** was reconstructed from the published PDF because the editable original was not recovered. Test specifications, episode dates and regime comparisons remain unverified pending recovery or replication of the empirical workflow.

[Revised paper](https://meanydeany.com/papers/bitcoin-bubble-gsadf-seminar-paper-revised-2026-10-14.pdf) | [Original submission](https://meanydeany.com/papers/bitcoin-bubble-gsadf-seminar-paper.pdf) | [Revision notes](https://meanydeany.com/papers/revision-notes-2026-10-14.html)

## How I work

I define the question and comparison before measuring a new experiment, preserve source and implementation identities, and keep future information out of historical decisions. Negative and inconclusive results remain part of the research record rather than being rewritten into winners.

I evaluate **prediction quality, after-cost economics and executable implementation as separate questions**. A passing test suite establishes software behavior, not an economic edge.

I use **Codex and Claude** for implementation, testing and review, with explicit specifications and independently checked calculations. Hypothesis selection and interpretation remain my responsibility.

## Background and tools

**University of Copenhagen:** MSc Economics, with a focus on financial econometrics and empirical asset pricing.  
**UC San Diego:** undergraduate economics, with a focus on quantitative economics and econometrics.

| Area | Tools and methods |
|---|---|
| Quantitative research | Python, pandas, NumPy, scikit-learn, statsmodels, volatility models, probabilistic forecasting |
| Statistical evaluation | Chronological validation, walk-forward studies, dependence-aware bootstrap inference, benchmark comparisons |
| Systems | C++, SQL / SQLite, Git, Linux, AWS Lightsail, event-driven processing, deterministic replay |
| Research integrity | Local test suites, source manifests, SHA-256 provenance, independent cash-flow checks, reproducible outputs |

## Contact

[meanydeany.com](https://meanydeany.com) | [woosub815@gmail.com](mailto:woosub815@gmail.com) | [@MeanyDeany](https://github.com/MeanyDeany)

> Core BTC research and execution repositories are private. This profile describes methods and public academic work, not private strategy internals, live strategy performance or trade signals.
