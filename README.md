# SM Radar — Smart Money Concepts indicator for crypto

[![TradingView](https://img.shields.io/badge/TradingView-Open%20Source-2962FF?logo=tradingview&logoColor=white)](https://www.tradingview.com/script/lcyOMlKP/)
[![License](https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg)](LICENSE)
[![Investisseur 2.0](https://img.shields.io/badge/By-Investisseur%202.0-7c3aed)](https://investisseur2-0.com)

A free, open source Pine Script indicator that detects Smart Money Concepts (SMC) on any crypto chart. Built for Bitcoin, Ethereum and major altcoins. Marks Order Blocks, Fair Value Gaps, liquidity zones and structural changes (BOS / CHoCH) automatically.

**Author** : Investisseur 2.0 (Cedric & Julien) — trading crypto using SMC since 2016.

---

## TL;DR

- 100% free, open source Pine Script
- Detects Order Blocks, FVG, liquidity, BOS/CHoCH on crypto charts
- Built for swing and intraday trading on BTC, ETH, large-cap alts
- Works on TradingView with any free account
- Code, documentation and methodology fully public

**Try it live on TradingView** : [https://www.tradingview.com/script/lcyOMlKP/](https://www.tradingview.com/script/lcyOMlKP/)

---

## What it does

SM Radar combines all the institutional Smart Money Concepts in one cohesive indicator, calibrated specifically for crypto markets (24/7 trading, sweep behavior, weekend liquidity hunts).

### Detected elements

| Concept | Detection logic |
|---------|----------------|
| **Order Blocks** | Last opposing candle before an impulsive move that breaks structure. Marked bullish or bearish. Mitigation status tracked. |
| **Fair Value Gaps (FVG)** | 3-candle inefficiency pattern. Auto-fill detection on revisit. |
| **Liquidity zones** | BSL (Buy Side Liquidity) above equal highs, SSL (Sell Side Liquidity) below equal lows. |
| **Market structure** | BOS (Break of Structure, continuation), CHoCH (Change of Character, reversal). |
| **Swing points** | Higher highs, higher lows, lower highs, lower lows with structural significance scoring. |

### What it does NOT do

- No buy/sell signals
- No automated alerts
- No backtest results "promised"
- No paywall, no invite-only, no upsell

It marks the structural elements you need to read the market like an institution. The decision to enter remains yours, based on confluence, context and your own risk management.

---

## How to use

1. Go to the TradingView script page : [SM Radar on TradingView](https://www.tradingview.com/script/lcyOMlKP/)
2. Click **Add to favorite indicators** (top right)
3. Open any chart (BTC/USDT 4H or Daily recommended for first use)
4. Click the **Indicators** menu → **Favorites** → **SM Radar**
5. The indicator appears on your chart with all SMC zones marked

### Recommended workflow

```
Step 1 — Higher timeframe context (Daily, Weekly)
  Identify if we are in HH/HL (bullish) or LH/LL (bearish) structure

Step 2 — Liquidity mapping
  Locate equal highs and equal lows (where retail stops accumulate)

Step 3 — Order Block identification
  Last opposing candle before BOS in the dominant direction
  Filter : fresh, preceded by sweep, followed by displacement

Step 4 — FVG confluence
  Check if a Fair Value Gap aligns with the OB zone

Step 5 — Lower timeframe entry trigger
  Wait for sweep of opposite liquidity in the OB zone
  Confirm with structural shift on 15M or 5M

Step 6 — Risk management
  Stop below OB (ATR-calibrated)
  Risk maximum 1% of capital
  TP1 next liquidity pool, TP2 major HTF level
```

---

## Why SM Radar is different

Most SMC indicators on TradingView focus on a single concept (just OB, just FVG). SM Radar combines all the institutional concepts in one cohesive view, calibrated for crypto volatility.

### Comparison vs typical SMC indicators

| Feature | Typical free indicator | SM Radar |
|---------|----------------------|----------|
| Order Blocks | Yes | Yes (with mitigation tracking) |
| Fair Value Gaps | Yes | Yes (with auto-fill detection) |
| Liquidity zones | Rare | Yes (BSL, SSL, equal highs/lows) |
| BOS / CHoCH | Sometimes | Yes (multi-timeframe) |
| Crypto-calibrated | No | Yes (24/7 sweep behavior) |
| Open source | Sometimes | Yes (MPL 2.0) |
| Active development | Rare | Yes (versioned releases) |

---

## Free education resources

If you want to learn the methodology before using this indicator, the full Smart Money Concepts framework is documented for free in French and English at **[investisseur2-0.com](https://investisseur2-0.com)** :

- [Smart Money Concepts pillar guide (10000 words)](https://investisseur2-0.com/ressources/smart-money-concepts-crypto)
- [SMC Glossary (38 terms with examples)](https://investisseur2-0.com/ressources/glossaire-smc)
- [Order Blocks complete guide](https://investisseur2-0.com/ressources/order-blocks-crypto)
- [Fair Value Gap strategy](https://investisseur2-0.com/ressources/fair-value-gap-fvg)
- [Risk management framework](https://investisseur2-0.com/ressources/gestion-du-risque-trading-crypto)
- [Free AI SMC chart analyzer](https://investisseur2-0.com/analyseur-smc-ia)

English version : [investisseur2-0.com/en](https://investisseur2-0.com/en)

---

## Source code

The Pine Script source is in [`indicator.pine`](indicator.pine).

Pine Script version : v6
TradingView compatibility : free account and above
Recommended timeframes : 15M, 1H, 4H, Daily, Weekly

---

## Versioning

- **v1.0** (April 2026) — Initial public release. OB, FVG, liquidity zones, BOS/CHoCH detection, multi-timeframe structure analysis.

Future versions will be tracked in [CHANGELOG.md](CHANGELOG.md).

---

## License

This project is licensed under the [Mozilla Public License 2.0](LICENSE) — you can use, modify and redistribute the code, with attribution to Investisseur 2.0.

For commercial use, integration in paid tools or removal of attribution, please contact us via Telegram first.

---

## About Investisseur 2.0

Investisseur 2.0 is a free educational platform specialized in Smart Money Concepts applied to crypto trading. Co-founded by Cedric and Julien in 2020.

- Website : [investisseur2-0.com](https://investisseur2-0.com)
- Telegram (free public channel) : [t.me/+fHlpmbj5OihhMDU0](https://t.me/+fHlpmbj5OihhMDU0)
- Twitter / X : [@Invest2_0](https://x.com/Invest2_0)
- TradingView : [Investisseur2_0](https://www.tradingview.com/u/Investisseur2_0/)

We provide free educational content, daily SMC analyses on Telegram, and free tools (this indicator, an AI chart analyzer, a risk calculator). No paid courses, no signal subscription. Our model is based on commission rebates from partner exchanges (XT, Pionex, BingX, BitMart).

---

## Disclaimer

This indicator is an analytical tool, not financial advice. Trading cryptocurrency involves substantial risk of capital loss. Past performance does not guarantee future results. Use at your own discretion with proper risk management. Investisseur 2.0 is not responsible for any loss incurred from the use of this indicator.

---

## Support and contributions

- Found a bug ? [Open an issue](../../issues)
- Want to suggest an improvement ? [Open a discussion](../../discussions)
- Want to contribute code ? [Submit a pull request](../../pulls)

For general trading questions, the active community is on Telegram : [t.me/+fHlpmbj5OihhMDU0](https://t.me/+fHlpmbj5OihhMDU0)
