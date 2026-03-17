# Quantitative Backtesting Engine

I wanted to understand how money actually moves at an institutional 
level — not as a user of financial systems, but as someone who 
builds the infrastructure underneath them.

This project is that pursuit made concrete.

---

## What This Is

A systematic trading strategy simulator built in Python and C++.

Fetches and processes real OHLCV market data. Implements modular 
trading strategies. Evaluates performance through quantitative 
metrics including Sharpe ratio and maximum drawdown. Integrates 
LLM-powered natural language strategy input and AI-driven 
results analysis.

---

## Architecture
```
┌─────────────────────────────────────┐
│         Python Interface Layer       │
│   Strategy input, analysis, viz      │
├─────────────────────────────────────┤
│         LLM Integration Layer        │
│   Natural language → strategy logic  │
├─────────────────────────────────────┤
│         C++ Computation Engine       │
│   Performance-critical processing    │
├─────────────────────────────────────┤
│         Data Handler                 │
│   OHLCV ingestion, cleaning          │
└─────────────────────────────────────┘
```

---

## Build Phases

- [x] Phase 0 — Repository foundation and domain study
- [ ] Phase 1 — OHLCV data handling and basic Python engine
- [ ] Phase 2 — First strategy and portfolio tracker
- [ ] Phase 3 — C++ computation core
- [ ] Phase 4 — LLM natural language strategy input
- [ ] Phase 5 — AI-driven results analysis and regime detection
- [ ] Phase 6 — Documentation, writeup, signal creation

---

## Honest Limitations

Updated as limitations are discovered during development.

- **Survivorship bias** — engine tests only currently existing 
  assets, which inflates historical performance
- **Transaction costs** — not yet modeled
- **Look-ahead bias** — under active scrutiny during development

Understanding what a system gets wrong is more important than 
showing what it gets right.

---

## Progress Log

- 2026-03-14 — Repository initialized. Project foundation 
  complete. Domain study begun.

---

## Setup
```bash
git clone https://github.com/yourusername/quantitative-backtesting-engine
cp .env.example .env
# Fill in your API keys in .env
pip install -r requirements.txt
```

---

## Why This Matters

The engineers who built the financial infrastructure that moves 
capital globally didn't start with access or advantage. They 
started with understanding systems deeply enough that the 
systems had no choice but to let them in.

This project is my version of that bet.
