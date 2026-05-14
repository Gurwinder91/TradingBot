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
| 4 | VIX determines which trade TYPE is allowed — see **VIX Decision Table** below |
| 5 | OI must CONFIRM chart direction. If they conflict → see **OI vs EMA Conflict Rule** below |
| 6 | Never hold PE below max Put OI strike — strong bounce zone |
| 7 | Never hold CE above max Call OI strike — strong rejection zone |

---

## VIX DECISION TABLE — TRADE TYPE FILTER

> **Check VIX before every trade. VIX determines WHICH trade type is allowed — not just position size.**

| VIX Level | Market State | ✅ Allowed | ❌ Blocked | Reason |
|---|---|---|---|---|
| **Below 15** | Calm / Complacent | **PE Buy** (bearish trend), CE Buy (bullish trend) | Put Sell, Call Sell | VIX is low = options are cheap to buy. As market falls, VIX rises = put buyer benefits from both direction AND expanding IV. Selling premium collects too little to justify the risk. |
| **15 – 20** | Normal | All trade types | Nothing blocked | Standard zone. All 4 trade types valid. Apply full 4-filter checklist normally. |
| **Above 20** | Panic / Fear spike | **Put Sell** — only if OI Conflict Rule (Improvement 1) is ALSO met: PCR > 1.2 + heavy Put OI floor visible on Sensibull | CE Buy, PE Buy | VIX spike = elevated IV = put premiums are inflated. Sell puts to collect high premium and profit from VIX cooling (IV crush). Do NOT buy calls — a cooling VIX will rapidly crush call premium even if price rises. **Both conditions must be true simultaneously — VIX alone is not enough.** |

### VIX Logic — Why It Works This Way

**VIX > 20 → Put Sell — but ONLY when OI Conflict Rule is ALSO met:**
Both conditions must be true at the same time:
1. VIX > 20 (panic spike, IV inflated — put premium is high, VIX cooling will crush it = seller profits)
2. PCR > 1.2 + heavy Put OI floor visible on Sensibull (institutional support below price — big players are defending the level)

VIX alone is not enough to sell puts. You need OI confirmation that the market has institutional support below. If PCR is below 1.0 and there is no visible put OI floor, the market may continue falling through any level — do not sell puts regardless of VIX. Buying calls in a VIX > 20 environment is dangerous — even if price bounces, the falling VIX crushes call premium and you lose despite being right on direction.

**VIX < 15 → PE Buy (not Put Sell):**
Market is calm and complacent — options are cheap. When a bearish trend begins, fear returns and VIX rises, expanding IV. The put buyer benefits from both the directional move DOWN and the expanding IV. Selling puts here collects very little premium and leaves you exposed if a sudden VIX spike occurs.

---

## OI VS EMA CONFLICT — RESOLUTION RULE

> **When OI and EMA disagree, do not skip blindly — use this decision table.**

| Situation | Allowed Trades | Blocked Trades |
|---|---|---|
| All EMAs BEARISH + PCR > 1.2 + Heavy Put OI at support below price | **ITM Put Sell** ✅ | PE Buy ❌ |
| All EMAs BULLISH + PCR < 0.8 + Heavy Call OI at resistance above price | **ITM Call Sell** ✅ | CE Buy ❌ |
| EMAs and OI fully agree on direction | All trade types allowed | — |
| EMAs and OI conflict with no clear Put/Call OI wall | **Skip — no trade** | All ❌ |

### ITM Put Sell in a Bearish EMA Trend (OI Conflict Setup)

> Use when: All 3 EMAs are BEARISH but PCR > 1.2 and heavy Put OI exists at a support level below current price. VIX has recently spiked and may be cooling.

**Why this works:** Big players have sold puts at key support levels — they are betting price stays above those strikes. A VIX spike followed by a cooling phase means IV is elevated and about to fall, which directly benefits the put seller. Selling an ITM put here captures all three:
- **Delta** — put premium falls as price stabilises or bounces
- **Theta** — time decay works in your favour every hour
- **Vega (VIX)** — IV crush from cooling VIX rapidly reduces premium

| Step | Rule |
|---|---|
| **Strike selection** | Sell ITM Put — target a strike where premium is **minimum ₹300** |
| **Why ITM, not OTM** | ITM puts have high delta + high premium. OTM puts collect too little to justify the risk on a bearish-EMA day |
| **Entry condition** | PCR > 1.2 **AND** visible heavy Put OI floor on Sensibull **AND** RSI showing divergence (higher lows) near support |
| **VIX check** | VIX must have spiked recently and be stabilising or declining. If VIX is still rising — **wait** |
| **Stop Loss** | Nifty spot closes a 15min candle BELOW the Max Put OI floor strike |
| **Target** | 40–50% premium decay. Do not hold to expiry. Exit if VIX spikes again. |
| **Avoid** | VIX still rising, price crashing through put OI floor on heavy volume, bad overnight global news |

---

## REVERSAL STRATEGY — PUT SELL AT SUPPORT

> Use when: Price has tested a key support level 2–3 times and is bouncing

| Step | Detail |
|---|---|
| **Setup** | Price at key support level. Tested 2+ times already |
| **Signal** | Price going DOWN SLOWLY (not crashing). 5min RSI starts curling UP while price still flat/falling |
| **Confirm** | 2 consecutive green 5min candles forming near support |
| **Entry** | Sell Put 50–100 points below current support (e.g. at 23,900, sell 23,850 PE) |
| **Stop Loss** | Nifty spot breaks support on 15min candle CLOSE basis |
| **Target** | 40–50% premium decay. Exit before next session or if VIX spikes |
| **Avoid** | VIX still rising, big red crash candle through support, RSI still falling with no divergence, bad global news, PCR below 1.0 |

---

## TRADING HOURS — NO TRADE ZONES (Intraday Only)

> Swing trades are NOT subject to these time rules — swing entries can be taken at any time as long as the 6 rules are met.

| Time Window | Rule | Reason |
|---|---|---|
| **9:00 AM – 9:30 AM** | ❌ NO new trades | Spreads are wide, EMAs not yet formed, gap fills and reversals common. Price often moves violently with no follow-through. |
| **9:30 AM – 1:00 PM** | ✅ Primary trading window | Best time. EMAs formed, volume active, clean trends develop. All 4 filters apply normally. |
| **1:00 PM – 2:30 PM** | ⚠️ Caution zone | Low volume, EMAs often flat, choppy price action. Only trade if setup is very clean (all 8 checklist YES). Reduce to half lot. |
| **3:00 PM – 3:30 PM** | ❌ NO new trades | Closing volatility, wide spreads, unpredictable spikes. Any open position should be managed — no new entries. |

**Rule:** If your setup triggers inside a NO TRADE window — wait. If the setup is still valid after 9:30 AM or before 3:00 PM, take it then.

### Gap Day Protocol

| Gap at Open | Rule |
|---|---|
| **Gap down > 0.5%** | Skip the first 30 minutes entirely. Let the gap fill attempt play out. Only trade after 10:00 AM with confirmed direction on the 15min chart. |
| **Gap up > 0.5%** | Same rule — skip first 30 minutes. Wait for gap fill attempt or breakout confirmation. Only trade after 10:00 AM. |
| **Gap < 0.5% either direction** | Normal session rules apply from 9:30 AM. |

**Why:** Large gaps attract immediate gap-fill attempts. Price often reverses sharply in the first 15–30 minutes before finding real direction. Entering before 10:00 AM on a gap day means trading noise, not trend.

---

## RISK MANAGEMENT — NON-NEGOTIABLE RULES

1. **Minimum 1:2 Risk:Reward** on every trade — no exceptions ever. If 1:2 is not achievable from the entry level, skip the trade entirely.
2. **Book 60% at Target 1** — trail stop loss to entry for remaining position
3. **Maximum 2-3 trades per day** — do not overtrade. Quality over quantity. If 3 trades are done, the day is closed regardless of outcome.
4. **Never average** a losing options position — exit at SL, reassess fresh
5. **Book profits BEFORE** major S&R levels — never hold hoping for more
6. **1 lot** as default unless setup is perfect across all 4 filters

### Daily Loss Limits — Stop Trading Immediately When Hit

| Account State | Daily Loss Limit | Rule |
|---|---|---|
| **Fresh account (no prior profit)** | ₹2,500 | If loss reaches ₹2,500 in a day → stop all trading immediately. No revenge trades. |
| **After a profitable previous day** | 50% of previous day's profit | Example: Made ₹6,000 yesterday → max loss today is ₹3,000. Protects prior gains. |

### Daily Profit Target — Close the Day When Hit

| Target | Rule |
|---|---|
| **₹5,000 – ₹6,000 profit** | Close all positions and stop trading for the day — even if achieved in a single trade. Do not look for more setups. Log the trade and walk away. |

> **Why a profit target matters:** Overtrading after a big win is one of the most common ways to give back profits. Once the daily target is hit, the risk:reward of continuing is poor — you have more to lose than to gain. A winning day is a winning day.

---

## PRE-TRADE CHECKLIST (All 8 Must Be YES)

```
☐ 1. All 3 EMA timeframes (15min, 1H, Daily) confirmed in same direction?
☐ 2. 5min RSI NOT at extreme (not below 30 or above 70)?
☐ 3. 15min RSI confirming direction (above 50 = bullish, below 50 = bearish)?
☐ 4. Price NOT sitting at a key S&R level right now?
☐ 5. Entry is on rejection or confirmed breakout — not mid-zone?
☐ 6. OI checked — if conflict with EMA, is it a valid Put Sell setup (PCR > 1.2 + Put OI floor)?
☐ 7. VIX checked — trade type matches VIX level (see VIX Decision Table)?
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

## PE BUY vs PUT SELL — DECISION MATRIX

> Both are bearish-side trades but they work in completely different market conditions. Choose the wrong one and you lose even when direction is right.

| Condition | PE Buy | Put Sell |
|---|---|---|
| **Price action** | Just broke a key support with momentum | At or near strong support, holding or slowing |
| **EMA** | Declining steeply across all timeframes | Bearish but price is extended below EMA |
| **RSI** | Below 45, falling with momentum | Divergence visible — RSI making higher lows while price makes lower lows |
| **PCR** | Below 0.8 — bearish, no institutional support | Above 1.2 — heavy put writing below, institutional floor present |
| **VIX** | Below 15 — cheap to buy, VIX expansion will boost premium | Above 20 — IV elevated, VIX cooling will crush premium (benefits seller) |
| **Expectation** | Sharp, fast directional move down | Consolidation or bounce — not a crash |
| **Expiry** | Next week if < 2 days to expiry, else current week | Always current week — maximum theta decay |
| **Delta** | 0.8–0.9 (deep ITM) | 0.6 (slightly ITM) |

### Quick Decision Rule

**Choose PE Buy when:**
Price just broke a key support level with a strong candle. EMA is declining steeply on all timeframes. RSI is below 45 and falling. VIX is low — cheap to buy puts and VIX expansion will add to your profit as the move develops.

**Choose Put Sell when:**
Price is sitting at or near a strong support with RSI divergence forming. You expect the level to hold and price to consolidate or bounce — not crash further. PCR is above 1.2 with visible put OI floor. VIX has spiked above 20 and may be cooling — sell elevated premium and collect IV crush + theta.

> **Key Principle:** PE Buy needs momentum and direction. Put Sell needs support and exhaustion. Never use Put Sell when price is in freefall — you will be crushed by delta even if IV helps.

---

## STRIKE SELECTION GUIDE

### PE Buy (Bearish Trend)

| Rule | Detail |
|---|---|
| **Delta** | 0.8 – 0.9 (deep ITM). High delta means the option moves almost point-for-point with Nifty — maximum directional capture. |
| **Expiry — if current expiry is LESS than 2 days away** | Buy **NEXT WEEK's** expiry strike. Current week options have aggressive theta decay in the last 2 days — avoid buying them. |
| **Expiry — if current expiry is MORE than 2 days away** | Buy **CURRENT WEEK's** expiry strike. Sufficient time for the move to play out with manageable decay. |
| **Why 0.8–0.9 delta** | Deep ITM puts behave almost like shorting Nifty directly. Minimal IV risk — premium is mostly intrinsic value. You capture the full directional move without relying on IV expansion. |

### Put Sell (Bullish OI Structure / VIX Spike)

| Rule | Detail |
|---|---|
| **Delta** | 0.6 (slightly ITM). Captures meaningful delta, strong theta, and full IV crush benefit. |
| **Expiry** | Always **CURRENT WEEK** expiry — maximum theta decay works in your favour. |
| **Why 0.6 delta** | Higher delta than a typical OTM sell — collects more premium (₹300+ as per ITM rule), captures IV crush faster, and benefits from delta as price stabilises or rises. OTM puts collect too little to justify the risk. |
| **Conditions required** | Must meet BOTH: VIX > 20 AND PCR > 1.2 with visible Put OI floor (Improvement 1 + Improvement 3 combined). |

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
| Trading in first 30 mins after a gap > 0.5% | Trading noise not trend — wait until 10:00 AM |
| PE Buy when VIX > 20 | Cooling VIX crushes put premium even if direction is right |
| Put Sell when VIX > 20 without checking OI/PCR | No institutional support = market may keep falling through your strike |
| Taking a 4th trade after daily target hit | Giving back profits — walk away at ₹5,000–6,000 |

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

*Last updated: May 13, 2026 | Version 2.0*
*Not SEBI-registered advice. For personal trading reference only.*
