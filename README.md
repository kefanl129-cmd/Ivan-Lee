# 🍵 Matcha Quant AI · Behavioral Risk Control Agent

##  Overview

**Matcha Quant AI** is a quantitative research prototype that integrates:

*  Financial market data analysis
*  Behavioral finance (emotion-aware risk control)
*  AI Agent architecture

Unlike traditional trading systems that focus on prediction, this project emphasizes:

> **Constraining irrational human decision-making under uncertainty.**

---

##  Motivation

In real-world trading environments, three major issues frequently arise:

### 1. Emotion-Driven Decisions

* Panic selling
* Overconfidence
* Greed-driven overexposure

### 2. Misunderstanding of Risk

Most systems focus on returns while ignoring:

* Drawdowns
* Tail risks
* Blow-up probability

### 3. Fragmented Information

Market signals are scattered across:

* Price data
* News
* Macro signals

---

##  System Architecture

```text
User Input
    ↓
Behavioral Layer (Emotion Detection)
    ↓
Market Data Layer (Yahoo Finance)
    ↓
Risk Engine (VaR / CVaR / Sharpe)
    ↓
Position Sizing (Kelly-lite)
    ↓
Decision Engine (Rule-based)
    ↓
Execution Layer (Simulated Broker)
```

---

##  Core Components

###  1. Behavioral Finance Layer

The system detects emotional states using NLP + rule-based logic:

* **Panic**
* **Greed**
* **Overconfidence**

When high-risk emotional states are detected:

>  Trading decisions are restricted

---

###  2. Risk Engine

Key quantitative metrics:

* **Sharpe Ratio** → risk-adjusted return
* **VaR (Value at Risk)** → potential loss threshold
* **CVaR (Conditional VaR)** → tail risk expectation
* **Max Drawdown** → worst historical loss

Additionally:

* Monte Carlo simulation estimates probability distributions

---

###  3. Position Sizing (Kelly-lite)

Position sizing is derived from volatility:

```text
Position Size ∝ Capital × Risk Budget / Volatility
```

This ensures:

> Risk exposure is controlled systematically, not emotionally

---

###  4. Decision Engine

Rule-based logic evaluates:

* Emotional state
* Risk metrics
* Market conditions

Outputs include:

* `NO TRADE`
* `AVOID`
* `REDUCE RISK`
* `TRADE (LOW SIZE)`

---

###  5. Execution Layer (Simulated Broker)

* Paper trading environment
* Mimics real execution flow
* Easily extendable to broker APIs

---

## Features

*  Multi-market support (US / CN / HK / JP / SG)
*  Emotion-aware trading constraints
*  Quantitative risk modeling
*  Monte Carlo risk simulation
*  Kelly-based position sizing
*  Rule-based decision engine
*  Simulated trading execution

---

##  Limitations

* No real-time tick-level data
* No machine learning prediction models
* Simplified emotion analysis (rule-based + TextBlob)
* Monte Carlo assumes normal distribution

---

##  Project Positioning

This project is **NOT**:

*  A trading bot
*  A profit prediction system

This project **IS**:

> ✔ A **Quantitative Risk-Control AI Agent Prototype**
> ✔ A **Behavioral Finance Decision Constraint System**

---

##  Key Insight

Traditional systems ask:

> “What will the market do?”

This system asks:

> **“Given uncertainty, how should humans behave?”**

---

##  Future Work

Potential upgrades:

* Backtesting engine
* Multi-asset portfolio optimization
* ML-based return prediction
* LLM-driven strategy generation
* Real broker API integration

---

##  Conclusion

**Matcha Quant AI** demonstrates a shift in perspective:

> From predicting markets → to managing decision risk.

It provides a structured framework for:

* Rational decision-making
* Risk-aware trading behavior
* AI-assisted financial analysis

---

##  Author

* Independent developer
* Focus: AI systems + Quantitative modeling + Behavioral finance

---

## Acknowledgement

Built using:

* Python
* Streamlit
* yfinance
* NumPy / Pandas

---

##  License

MIT License (recommended)

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

