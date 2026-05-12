# NIFTY 50 OPTIONS — PERSONAL TRADING STRATEGY RULEBOOK
**Trader:** GS | **Instrument:** Nifty 50 Options (Weekly + Monthly) | **Lot Size:** 65

---

## HOW TO USE THIS FILE WITH CLAUDE
> Paste this entire file content into any new Claude conversation and say:
> *"This is my Nifty trading strategy. I will share charts — analyse using these rules and suggest trades."*
> Then share your 15min + 1H + Daily charts and Claude will auto-analyse using all 4 filters below.

---

## FILTER 1 — 21 EMA TREND (Primary Trend Filter)

| Step | Rule |
|---|---|
| 1 | Check 15min chart first — is price clearly ABOVE or BELOW 21 EMA? |
| 2 | Confirm SAME direction on 1 Hour chart |
| 3 | Confirm SAME direction on Daily chart |
| ✅ | All 3 aligned BEARISH = Only PE Buy or Call Sell allowed |
| ✅ | All 3 aligned BULLISH = Only CE Buy or Put Sell allowed |
| ❌ | If any 2 of 3 timeframes conflict = NO TRADE |

---

## FILTER 2 — RSI ENTRY TIMING

| Step | Rule |
|---|---|
| 1 | Check RSI on **5min AND 15min** before every entry |
| 2 | RSI near or below **30 (oversold)** = WAIT. Do NOT buy PE. Wait for RSI to recover above 35 first |
| 3 | RSI near or above **70 (overbought)** = WAIT. Do NOT buy CE. Wait for RSI to pull back below 65 first |
| 4 | Best entries: RSI moving directionally between 40–60 zone |
| 5 | 15min RSI above 50 = bullish momentum. Below 50 = bearish momentum |

### RSI Divergence — Reversal Signal
> **Price making Lower Low + RSI making Higher Low** at a strong support level
> = High confidence **Put Sell** entry signal (bounce expected)

---

## FILTER 3 — SUPPORT AND RESISTANCE

| Step | Rule |
|---|---|
| 1 | Mark key S&R levels BEFORE market open using OI data and previous session |
| 2 | NEVER enter when price is sitting AT a S&R level — always wait |
| 3 | Wait for price to **break and reject** from the level |
| 4 | Rejection candle at resistance + bearish EMA = **PE Buy** entry |
| 5 | Bounce at support + RSI divergence = **Put Sell** entry |
| 6 | Support tested 2–3 times = stronger bounce signal |
| ❌ | Price in middle of range between S&R = NO TRADE ZONE |

---

## FILTER 4 — OI CONFIRMATION (Sensibull)

| Step | Rule |
|---|---|
| 1 | Max **Call OI strike = ceiling** (strong resistance) |
| 2 | Max **Put OI strike = floor** (strong support) |
| 3 | **PCR below 0.8** = bearish bias. **PCR above 1.2** = bullish bias |
| 4 | **VIX rising above 20** = avoid selling premium. High loss risk |
| 5 | OI must CONFIRM chart direction. If they conflict = skip the trade |
| 6 | Never hold PE below max Put OI strike — strong bounce zone |
| 7 | Never hold CE above max Call OI strike — strong rejection zone |

---

## REVERSAL STRATEGY — PUT SELL AT SUPPORT

> Use when: Price has tested support (23,800 or 23,900) 2–3 times and bouncing

| Step | Detail |
|---|---|
| **Setup** | Price at key support level. Tested 2+ times already |
| **Signal** | Price going DOWN SLOWLY (not crashing). 5min RSI starts curling UP while price still flat/falling |
| **Confirm** | 2 consecutive green 5min candles forming near support |
| **Entry** | Sell Put 50–100 points below current support (e.g. at 23,900, sell 23,850 PE) |
| **Stop Loss** | Nifty spot breaks support on 15min candle CLOSE basis |
| **Target** | 40–50% premium decay. Exit before next session or if VIX spikes |
| **Avoid** | VIX > 20, big red crash candle through support, RSI still falling, bad global news |

---

## RISK MANAGEMENT — NON-NEGOTIABLE RULES

1. **Minimum 1:2 Risk:Reward** on every trade — no exceptions ever
2. **Book 60% at Target 1** — trail stop loss to entry for remaining position
3. **Maximum 2 losing trades per day** — if hit, STOP trading for the day
4. **Never average** a losing options position — exit at SL, reassess fresh
5. **Book profits BEFORE** major S&R levels — never hold hoping for more
6. **1 lot** as default unless setup is perfect across all 4 filters

---

## PRE-TRADE CHECKLIST (All 8 Must Be YES)

```
☐ 1. All 3 EMA timeframes (15min, 1H, Daily) confirmed in same direction?
☐ 2. 5min RSI NOT at extreme (not below 30 or above 70)?
☐ 3. 15min RSI confirming direction (above 50 = bullish, below 50 = bearish)?
☐ 4. Price NOT sitting at a key S&R level right now?
☐ 5. Entry is on rejection or confirmed breakout — not mid-zone?
☐ 6. PCR and OI data confirms chart direction?
☐ 7. VIX NOT spiking above 20 (especially if selling premium)?
☐ 8. Risk:Reward is minimum 1:2 on this trade?

→ ALL 8 YES = Take the trade
→ ANY NO   = Wait or skip
```

---

## TRADE SIGNAL ZONES

```
🔴 STRONG RESISTANCE  →  Max Call OI Strike (ceiling)
─────────────────────────────────────────────────────
🟠 WEAK RESISTANCE    →  Previous S&R level
─────────────────────────────────────────────────────
⚪ NO TRADE ZONE      →  Middle of range — no edge
─────────────────────────────────────────────────────
🟡 WEAK SUPPORT       →  Previous S&R level
─────────────────────────────────────────────────────
🟢 STRONG SUPPORT     →  Max Put OI Strike (floor)
```

---

## HOW TO SHARE CHARTS FOR ANALYSIS

When sharing charts, always provide:
1. **15min chart** (mandatory — primary timeframe) with 21 EMA + RSI visible
2. **1 Hour chart** with 21 EMA + RSI visible
3. **Daily chart** with 21 EMA + RSI visible
4. **OI screenshot** from Sensibull (optional but very helpful)
5. **Current Nifty spot price**
6. **Expiry trading** (weekly/monthly)

Claude will then respond with:
- ✅/❌ status for all 4 filters
- CE or PE direction
- Entry zone, Stop Loss, Target 1, Target 2
- Confidence level: High / Medium / Low

---

## COMMON MISTAKES TO AVOID

| Mistake | Why It Causes Loss |
|---|---|
| Entering without all 3 EMA confirmation | Trading against the trend |
| Entering at S&R level | Price can go either way — no edge |
| Ignoring RSI extreme at entry | Price exhausted, reversal imminent |
| Ignoring OI data | Fighting smart money |
| Not booking at Target 1 | Giving back profits |
| Trading after 2 losses | Revenge trading — emotionally driven |
| Averaging losing trade | Multiplies the loss |
| Holding through major S&R | Gets stuck, premium decays |

---

## KEY LEVELS REFERENCE (Update Daily)

| Level | Zone | Notes |
|---|---|---|
| Max Call OI Strike | Strong Resistance | Update from Sensibull daily |
| Max Put OI Strike | Strong Support | Update from Sensibull daily |
| Previous Day High | Resistance | Key intraday level |
| Previous Day Low | Support | Key intraday level |
| Round numbers (24000, 23800 etc.) | Strong S&R | Psychological levels |

---

*Last updated: May 11, 2026 | Version 1.0*
*Not SEBI-registered advice. For personal trading reference only.*
