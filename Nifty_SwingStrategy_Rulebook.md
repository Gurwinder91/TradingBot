# NIFTY 50 — SWING TRADING STRATEGY RULEBOOK
**Trader:** GS | **Instrument:** Nifty 50 (Swing Trades) | **Style:** Swing (Multi-day holds)

---

## HOW TO USE THIS FILE WITH CLAUDE
> Share this rulebook in any Claude conversation and say:
> *"This is my Nifty swing trading strategy. I will share charts — analyse using these rules and suggest trades."*
> Then share your **1H/2H + Daily + Weekly + Monthly charts** (with 21 EMA + RSI visible) and current Nifty spot price.

---

## RULE 1 — DETERMINE MARKET DIRECTION (Higher Timeframe Bias)

**Check all 3 higher timeframes FIRST before anything else.**

| Timeframe | Check | Result |
|---|---|---|
| Monthly Chart | Is price ABOVE or BELOW 21 EMA? | Above = Bullish / Below = Bearish |
| Weekly Chart | Is price ABOVE or BELOW 21 EMA? | Above = Bullish / Below = Bearish |
| Daily Chart | Is price ABOVE or BELOW 21 EMA? | Above = Bullish / Below = Bearish |

| Outcome | Rule |
|---|---|
| ✅ All 3 aligned BULLISH | Only LONG trades allowed |
| ✅ All 3 aligned BEARISH | Only SHORT trades allowed |
| ⚠️ 2 of 3 aligned | Proceed with caution — lower confidence |
| ❌ All 3 conflicting | NO TRADE — no clear direction |

> **Key Principle:** The higher timeframe bias is the compass. Never trade against it on a swing setup.

---

## RULE 2 — FIND THE TRADE SETUP (Execution Timeframe)

**Use 1HR or 2HR chart to find entry. It MUST align with Rule 1 direction.**

| Step | Action |
|---|---|
| 1 | Open the 1HR chart (or 2HR for cleaner signals) with 21 EMA plotted |
| 2 | Confirm price is on the SAME SIDE of 21 EMA as the higher timeframe bias |
| 3 | If 1HR/2HR direction CONFLICTS with Daily/Weekly/Monthly → **NO TRADE** |
| 4 | If 1HR/2HR direction CONFIRMS Daily/Weekly/Monthly → Proceed to Rule 3 |

> **Example:** Daily/Weekly/Monthly all bullish → 1HR price must also be above 21 EMA or pulling back towards it from above.

---

## RULE 3 — ENTRY NEAR 21 EMA (Pullback Entry)

**Wait for price to pull back TO the 21 EMA — never chase extended moves.**

| Step | Rule |
|---|---|
| 1 | Do NOT enter when price is far away from 21 EMA (extended move) |
| 2 | Wait for price to PULL BACK towards the 21 EMA on the 1HR/2HR chart |
| 3 | Look for price to **touch or come very close** to the 21 EMA |
| 4 | In a BULLISH setup: price pulls back to 21 EMA from above → look for bounce |
| 5 | In a BEARISH setup: price pulls back to 21 EMA from below → look for rejection |
| ✅ | Entry signal = Rejection candle forming AT or near the 21 EMA |
| ❌ | Price breaking THROUGH the 21 EMA decisively = Setup invalidated, wait |

> **Key Principle:** The 21 EMA is your entry zone. Patience is the edge — wait for price to come to you.

---

## OI CONFLICT RULE — WHEN NOT TO ADD SHORTS (BEARISH SWING)

> **Use when:** All HTF timeframes are BEARISH but Sensibull PCR > 1.2 and heavy Put OI exists below current price.

This means big players have sold puts at support levels — the market is institutionally defended from below even in a bearish trend. Adding fresh shorts at the current price means fighting the OI wall.

| Situation | Rule |
|---|---|
| Bearish EMA + PCR > 1.2 + Heavy Put OI visible below price | **Do NOT add short here.** Wait for price to rally. |
| Price rallies back to 1HR/2HR 21 EMA | **Watch for rejection candle → SHORT entry** |
| Price rallies back to 1HR/2HR EMA + RSI reaches 45–55 | **Ideal short entry — use this as your trigger** |
| PCR drops below 1.0 after the rally | Additional confirmation that OI support has weakened |

**Key principle:** In a bearish swing, let the market rally to your EMA entry zone. The OI wall below protects against you getting stopped on a short entered too early. The 1HR/2HR 21 EMA pullback is always your entry — never the current price after a big drop.

---

## RULE 4 — AVOID SUPPORT & RESISTANCE ZONES

**Never enter a trade when price is sitting at a key S&R level.**

| Scenario | Rule |
|---|---|
| Price AT a key resistance level | WAIT — do not enter long. No edge. |
| Price AT a key support level | WAIT — do not enter short. No edge. |
| Price breaks ABOVE resistance | Wait for a **rejection/retest candle** after the breakout, then enter long |
| Price breaks BELOW support | Wait for a **rejection/retest candle** after the breakdown, then enter short |
| Price in middle of S&R range | NO TRADE ZONE — no edge in mid-range |

### How to Identify Key S&R Levels
- Previous swing highs and lows (Daily/Weekly chart)
- Round numbers (24,000 / 23,500 / 23,000 etc.)
- Previous consolidation zones
- Monthly and weekly chart pivot areas

> **Key Principle:** Wait for the market to PROVE the level has been broken. Enter on the retest/rejection, not the initial touch.

---

## RULE 5 — RSI CONFIRMATION BEFORE ENTRY

**Check RSI on the 1HR or 2HR chart before every entry.**

| RSI Reading | Action |
|---|---|
| RSI near or below **30** (oversold) | ⚠️ WAIT — do not enter short. Wait for RSI to recover back towards 40–50 |
| RSI near or above **70** (overbought) | ⚠️ WAIT — do not enter long. Wait for RSI to pull back towards 50–55 |
| RSI **40–55**, declining or flat after relief rally | ✅ **Short entry zone** — momentum confirming bearish continuation |
| RSI **45–60**, recovering from oversold | ✅ **Long entry zone** — momentum turning bullish, energy returning |
| RSI below 40 and still falling | ❌ Do NOT short — momentum exhausted, reversal or bounce risk high |
| RSI above 60 and still rising | ❌ Do NOT long — momentum extended, pullback risk high |

### RSI Entry Zones for Swing Trades

**Short Entries — RSI 40–55 (declining or flat after relief rally)**
In a bearish swing, price pulls back to the 1HR/2HR 21 EMA and RSI recovers partially from oversold. The ideal short window is when RSI is between 40–55 and has stopped rising or is starting to roll over. This confirms the relief rally is exhausting and bearish momentum is resuming. RSI does not need to reach 50 exactly — 40–55 is the valid window.

**Long Entries — RSI 45–60 (recovering from oversold)**
In a bullish swing, price pulls back to the 21 EMA and RSI has recovered from an oversold dip. The ideal long window is when RSI is between 45–60 and is rising — confirming buying momentum is returning. Entering when RSI is still below 40 risks catching a falling knife before the bounce is confirmed.

> **Key Principle:** RSI does not need to hit exactly 50. The zone matters more than the exact number — look for RSI to be in the right range AND moving in the right direction.

---

## RULE 6 — STOP LOSS & RISK REWARD

**Stop loss is based on the 21 EMA rejection candle. Minimum 1:2 R:R always.**

| Step | Rule |
|---|---|
| 1 | Identify the **rejection candle** at the 21 EMA (the entry signal candle) |
| 2 | Place Stop Loss **just beyond the low of the rejection candle** (for longs) |
| 3 | Place Stop Loss **just beyond the high of the rejection candle** (for shorts) |
| 4 | Add a small buffer of 5–10 points beyond the candle wick |
| 5 | Calculate Risk = Entry Price minus Stop Loss |
| 6 | Calculate minimum Target = Entry Price + (2 × Risk) → **1:2 minimum** |
| 7 | If 1:2 target hits a major S&R level before being reached → **skip or reduce size** |
| ❌ | Never enter if 1:2 R:R is not achievable with a logical stop |

### Partial Profit Booking
| Action | Rule |
|---|---|
| Target 1 (1:2 R:R) | Book **50–60% of position** here |
| Move SL to breakeven | After T1 hit, move SL to entry price |
| Target 2 (1:3 or 1:4 R:R) | Let remaining position run to next key level |
| Trailing SL | Trail below each successive 1HR swing low (for longs) |

> **Key Principle:** The rejection candle tells you where the market proved direction. Your stop goes just beyond that proof point.

---

## INSTRUMENT SELECTION — MONTHLY SYNTHETIC FUTURES

> Nifty Futures (FUT) cost has increased in India (higher margin + STT). Swing trades now use **Monthly Synthetic Futures** to replicate the same payoff at lower cost. Two structures are available — choose based on conviction and margin availability.

### Option A — Two-Leg Synthetic Future (True Futures Payoff)

| Direction | Structure | When to Use |
|---|---|---|
| **Long (Bullish swing)** | Buy ATM Monthly Call + Sell ATM Monthly Put (same strike, same expiry) | High conviction bullish setup. Want delta ~1 with zero net theta drag. |
| **Short (Bearish swing)** | Buy ATM Monthly Put + Sell ATM Monthly Call (same strike, same expiry) | High conviction bearish setup. Want delta ~1 with zero net theta drag. |

**Advantages:** Behaves exactly like Nifty Futures. Theta on the bought leg is offset by the sold leg — no net time decay. Delta ~1.
**Disadvantage:** Requires margin for the short leg. Two brokerage charges.
**Best for:** Strong trending setups (Grade A) where you want full point-for-point capture.

---

### Option B — Single Deep ITM Option (Simple Futures Proxy)

| Direction | Structure | When to Use |
|---|---|---|
| **Long (Bullish swing)** | Buy deep ITM Monthly Call — delta ~0.90–0.95 | When margin is limited or trend is developing. Simpler to manage. |
| **Short (Bearish swing)** | Buy deep ITM Monthly Put — delta ~0.90–0.95 | When margin is limited or trend is developing. Simpler to manage. |

**Advantages:** Single leg. No margin required for a short leg. Lower brokerage. Easy to exit.
**Disadvantage:** Small theta cost over the hold period. Slightly less than delta 1.
**Best for:** Standard setups (Grade B) or when margin capacity is being conserved.

---

### Which to Choose — Decision Guide

| Situation | Use |
|---|---|
| Grade A setup, all 6 rules met, strong trending market | Option A — Two-leg Synthetic |
| Grade B setup, or trend still developing | Option B — Deep ITM Single Leg |
| Margin capacity is limited | Option B — Deep ITM Single Leg |
| Overnight gap risk is high (news, events) | Option B — Single Leg (easier to exit quickly) |
| High conviction, want to hold 5–10 days | Option A — Full synthetic for zero theta drag |

### Expiry Selection for Swing

Always use **current month's expiry** (or next month if less than 7 days remain in current month). Monthly expiry gives sufficient time for the swing to play out without aggressive theta decay.

---

## RULE 7 — TRADE JOURNAL LOGGING

**Log every trade in the Trading Journal Excel — Swing Trades tab.**

File: `Nifty_Trading_Journal.xlsx` → **"Swing Trades" tab**

### Fields to Log

| Field | What to Record |
|---|---|
| Date | Entry date |
| Exit Date | Date trade was closed |
| Direction | Long / Short |
| Entry Price | Nifty spot or option strike + premium |
| Stop Loss | Price level (from rejection candle) |
| Target 1 | First target (1:2 R:R) |
| Target 2 | Second target (1:3 or 1:4 R:R) |
| Exit Price | Actual exit level |
| P&L | Profit or Loss in points/₹ |
| Higher TF Bias | Monthly/Weekly/Daily alignment (e.g. All Bullish) |
| 1HR/2HR Bias | Execution timeframe direction |
| RSI at Entry | RSI reading on 1HR/2HR at time of entry |
| S&R Check | Was S&R clear? (Yes/No) |
| Setup Quality | A / B / C grade |
| Notes | What worked or what to improve |

> **Why log every trade:** Pattern recognition over time. You will see which setups have the highest hit rate and where losses come from.

---

## PRE-TRADE CHECKLIST (All Must Be YES Before Entering)

```
HIGHER TIMEFRAME BIAS
☐ 1. Monthly chart price above/below 21 EMA — direction confirmed?
☐ 2. Weekly chart aligned with Monthly direction?
☐ 3. Daily chart aligned with Monthly/Weekly direction?

EXECUTION TIMEFRAME
☐ 4. 1HR or 2HR chart on same side of 21 EMA as higher TF bias?
☐ 5. Price has pulled back TO the 21 EMA (not extended far away)?
☐ 6. Rejection candle formed AT or near the 21 EMA?

SUPPORT & RESISTANCE
☐ 7. Price is NOT sitting at a key S&R level right now?
☐ 8. If near S&R — has price broken through AND retested with rejection?

RSI
☐ 9. RSI on 1HR/2HR is NOT at extreme (not below 30 or above 70)?
☐ 10. RSI in valid entry zone? (Short: 40–55 declining/flat | Long: 45–60 recovering)

RISK MANAGEMENT
☐ 11. Stop loss placed just beyond the rejection candle wick?
☐ 12. Minimum 1:2 Risk:Reward is achievable from entry to T1?

→ ALL 12 YES = Take the trade
→ ANY NO   = Wait or skip
```

---

## TRADE SIGNAL FLOW — STEP BY STEP

```
STEP 1: Check Monthly + Weekly + Daily (21 EMA)
         → All bullish? → LONG ONLY mode
         → All bearish? → SHORT ONLY mode
         → Conflict? → STAND ASIDE

STEP 2: Check 1HR / 2HR chart (21 EMA)
         → Same direction as Step 1? → Continue
         → Conflicting? → NO TRADE

STEP 3: Is price near / pulling back to 21 EMA?
         → Yes → Watch for rejection candle
         → No (extended) → WAIT for pullback

STEP 4: Check S&R levels
         → At S&R? → WAIT
         → After breakout + retest? → Can enter
         → Mid-range? → NO TRADE

STEP 5: Check RSI on 1HR/2HR
         → Below 30 or still falling? → WAIT (do not short exhausted move)
         → Above 70 or still rising? → WAIT (do not long extended move)
         → SHORT: RSI 40–55, declining or flat after relief rally → ✅ ENTRY ZONE
         → LONG:  RSI 45–60, recovering from oversold → ✅ ENTRY ZONE

STEP 6: Confirm rejection candle at 21 EMA
         → Set SL beyond the candle
         → Confirm 1:2 R:R achievable
         → ENTER TRADE

STEP 7: Log in Journal → Swing Trades tab
```

---

## COMMON MISTAKES TO AVOID

| Mistake | Why It Causes Loss |
|---|---|
| Entering when price is far from 21 EMA | Chasing — poor R:R, likely to get pullback |
| Ignoring Monthly/Weekly direction | Trading against the dominant swing trend |
| Entering AT a S&R level | No edge — price can go either direction |
| Entering when RSI is near 30/70 extreme | Momentum exhausted — reversal risk high |
| Not waiting for rejection candle | Entering blindly — no confirmation |
| SL too tight (inside candle wick) | Getting stopped out on normal noise |
| Skipping the 1:2 R:R check | Asymmetric losses — not sustainable |
| Not logging in journal | No learning — same mistakes repeated |

---

## SETUP GRADING SYSTEM

| Grade | Criteria |
|---|---|
| **A — High Conviction** | All 3 HTF aligned + 1HR/2HR confirmed + clean pullback to EMA + RSI in valid zone (40–55 short / 45–60 long) + no S&R conflict + 1:3+ R:R possible |
| **B — Standard Setup** | 2 of 3 HTF aligned + 1HR confirmed + EMA pullback + RSI acceptable + 1:2 R:R |
| **C — Lower Quality** | HTF mixed or RSI not ideal or S&R nearby — reduce size or skip |

> **Rule:** Only trade A and B setups. Skip C setups entirely.

---

## CHARTS REQUIRED FOR ANALYSIS

When sharing charts, always provide:
1. **Monthly chart** with 21 EMA visible
2. **Weekly chart** with 21 EMA visible
3. **Daily chart** with 21 EMA + RSI visible
4. **1HR or 2HR chart** with 21 EMA + RSI visible (primary execution chart)
5. **Current Nifty spot price**
6. **Key S&R levels** you have identified (or ask Claude to identify)

Claude will respond with:
- ✅/❌ status for all 4 rules (HTF bias, Execution TF, S&R, RSI)
- Full pre-trade checklist (12 points)
- Direction: Long / Short
- Entry zone, Stop Loss level, Target 1, Target 2
- Setup grade: A / B / C
- Confidence: High / Medium / Low

---

*Last updated: May 13, 2026 | Version 2.0*
*Not SEBI-registered advice. For personal trading reference only.*
