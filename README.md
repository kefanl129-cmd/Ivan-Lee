# Three Brothers Investment Strategy Simulation

> In turbulent markets, discipline and patience matter more than prediction.  
> Survival is the first alpha.

Life is a game,just enjoy it.

## Introduction

This project explores decision-making under uncertainty using a Monte Carlo simulation framework.

It does not attempt to predict markets, but to compare how different risk preferences affect long-term outcomes.

Key insights:
- Survival matters more than short-term returns
- High returns are meaningless without risk control
- Compounding requires avoiding ruin



## Model Overview

Three stylized investment strategies are simulated:

### Eldest (Stability)
- Low return, low volatility
- Focus on capital preservation

### Second (Growth)
- Moderate return and risk
- Balanced compounding behavior

### Third (High Risk)
- High return, high volatility
- Subject to ruin (wealth can drop to zero)

Yesterday is a history,tomorrow is a riddle.Today is a gift.

## Model Dynamics

Wealth evolves as:

\[
W_{t+1} = W_t (1 + \mu + \sigma Z_t), \quad Z_t \sim \mathcal{N}(0,1)
\]

For the high-risk strategy:
- Wealth is absorbed at zero upon ruin

---

## Parameters

| Parameter | Value |
|----------|------|
| T | 200 |
| N | 100 |
| W0 | 1 |

### Strategy Parameters

| Strategy | μ | σ |
|----------|--|--|
| Eldest | 0.001 | 0.003 |
| Second | 0.004 | 0.015 |
| Third | 0.009 | 0.090 |

---

## Outputs

- Mean wealth trajectories
- Log-scale comparison
- Sample path simulation
- Survival probability of high-risk strategy

---

## Key Metric

```matlab
survival_rate_3 = mean(wealth_paths_3(:,end) > 0);
If you're reject,accept it;if you are default,enjoy if.It's a interesting period.





Conclusion:

Risk Preference Archetypes in Capital Allocation Behavior

In financial decision-making and behavioral modeling, individuals can be broadly categorized into distinct archetypes based on their risk tolerance, time preference, and response to market volatility. These archetypes can be interpreted as different capital allocation philosophies under uncertainty.

The “Conservative Archetype” prioritizes capital preservation and stability. This profile aligns closely with risk-free asset allocation strategies, where the objective function is the minimization of return volatility. Utility is derived primarily from consistency and predictability, analogous to minimizing variance in outcomes.

The “Long-Term Compounding Archetype” focuses on temporal value creation and sustained growth. This approach resembles long-only investment strategies that rely on compounding effects over extended time horizons. Performance is evaluated through the slope of long-term return trajectories, emphasizing structural growth rather than short-term fluctuations.

The “Dynamic Optionality Archetype” embraces volatility as a source of opportunity. This profile is structurally similar to options-based strategies, where payoff functions are nonlinear and asymmetric. Value is generated through exposure to distributional extremes, convexity, and market dislocations, but accompanied by elevated downside risk.

Modern markets evolve at high frequency, and the impact of such evolution on individual outcomes is largely determined by three core capabilities: structural understanding of underlying mechanisms, depth of system-level reasoning, and execution quality in decision environments.

In highly volatile asset classes such as cryptocurrencies, the “dynamic optionality” profile may experience both significant upside from convex payoff structures and extreme downside due to path dependency and tail risk. Conversely, conservative strategies avoid exposure to such volatility, while long-term compounding strategies seek to neutralize short-term fluctuations through systematic, time-driven accumulation.

Ultimately, heterogeneous risk preferences give rise to diverse capital behaviors across market participants. The notion of “alpha” in this context can be interpreted as the ability to align personal risk architecture with market structure, thereby achieving superior risk-adjusted outcomes.

	​

