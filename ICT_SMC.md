# ICT / SMC COMPLETE TRADING MANUAL — XAUUSD (GOLD)

> **Scope:** This document covers every ICT (Inner Circle Trader) and Smart Money Concepts (SMC) concept exclusively applied to XAUUSD (Spot Gold). No other instruments are referenced. Every section includes a specific XAUUSD example. This is a reference document, not motivational content. Every rule stated here is a mechanical rule, not a suggestion.

---

# TABLE OF CONTENTS

1. [Foundational Market Mechanics](#1-foundational-market-mechanics)
2. [Market Structure](#2-market-structure)
3. [Liquidity — Full Taxonomy](#3-liquidity--full-taxonomy)
4. [Displacement](#4-displacement)
5. [Order Blocks — Complete Classification](#5-order-blocks--complete-classification)
6. [Fair Value Gap (FVG)](#6-fair-value-gap-fvg)
7. [Breaker Blocks](#7-breaker-blocks)
8. [Mitigation Blocks](#8-mitigation-blocks)
9. [Rejection Blocks](#9-rejection-blocks)
10. [Balanced Price Range (BPR)](#10-balanced-price-range-bpr)
11. [Liquidity Voids](#11-liquidity-voids)
12. [Premium & Discount Zones — PD Arrays](#12-premium--discount-zones--pd-arrays)
13. [Power of Three (AMD Model)](#13-power-of-three-amd-model)
14. [Interbank Price Delivery Algorithm (IPDA)](#14-interbank-price-delivery-algorithm-ipda)
15. [Kill Zones & Session Structure](#15-kill-zones--session-structure)
16. [Optimal Trade Entry (OTE)](#16-optimal-trade-entry-ote)
17. [Inducement (IDM)](#17-inducement-idm)
18. [ICT Macros](#18-ict-macros)
19. [Silver Bullet Strategy](#19-silver-bullet-strategy)
20. [Judas Swing](#20-judas-swing)
21. [Multi-Timeframe Framework (Top-Down Analysis)](#21-multi-timeframe-framework-top-down-analysis)
22. [Full Trade Execution Model — XAUUSD](#22-full-trade-execution-model--xauusd)
23. [Risk & Position Management](#23-risk--position-management)
24. [XAUUSD-Specific Characteristics](#24-xauusd-specific-characteristics)
25. [Case Studies — XAUUSD](#25-case-studies--xauusd)
26. [Pre-Trade Checklist](#26-pre-trade-checklist)
27. [Common Errors — Mechanical Breakdown](#27-common-errors--mechanical-breakdown)
28. [Glossary](#28-glossary)

---

# 1. FOUNDATIONAL MARKET MECHANICS

## 1.1 What Smart Money Actually Is

"Smart Money" is not a vague concept. It refers specifically to entities that have the position size, capital, and algorithmic infrastructure to influence price delivery:

| Entity | Role in XAUUSD |
|---|---|
| **Bullion Banks** (HSBC, JP Morgan, UBS, Goldman Sachs, Scotia) | Primary market-makers in OTC spot gold. They quote bid/ask and route interbank flow. |
| **Central Banks** (Fed, PBoC, RBI) | Buy/sell gold as reserve asset. Large accumulation periods are invisible to retail. |
| **Hedge Funds & CTAs** | Execute large directional positions, often using futures on COMEX. |
| **Algorithmic / HFT** | Execute price delivery based on time-and-price parameters. This is what ICT refers to as the IPDA (see Section 14). |
| **Liquidity Providers** | Absorb retail order flow and hedge with institutional counterparties. |

Retail traders (the entire population of individual traders worldwide) account for less than 5% of total daily XAUUSD volume. Retail positions do not move price. They are the counterparty supply that Smart Money uses to fill its own orders.

**Key mechanical conclusion:** Every stop-loss a retail trader places is a pending order in the book. When Smart Money needs to execute a large order (e.g., buy 50,000 oz), they require sell-side liquidity. The most efficient way to create that sell-side supply is to trigger retail long positions' stop-losses. Those stop-losses are market sell orders. Smart Money buys them.

---

## 1.2 The Interbank Price Delivery Model

Price does not move because supply and demand "balance." Price is delivered by an algorithm to specific price levels where liquidity is stored. The sequence is:

```
LIQUIDITY EXISTS → PRICE IS DELIVERED TOWARD IT → SWEEP EXECUTES → DISPLACEMENT OCCURS → IMBALANCE IS CREATED → REBALANCING OCCURS → NEXT LIQUIDITY TARGET IS IDENTIFIED
```

This is not theoretical. It is observable on every timeframe, every session, in XAUUSD.

**Why Gold specifically follows this model with high clarity:**
- XAUUSD is a highly liquid market with deep institutional participation
- Gold has well-defined psychological levels (round numbers: 2000, 2100, 2200, 2300, 2400, 2500, 3000) that concentrate retail stop orders
- Gold's relationship with the USD Dollar Index (DXY) creates predictable bias shifts
- Gold trades nearly 24 hours with consistent session-based volatility patterns

---

## 1.3 Price Delivery Sequence (The Core Engine)

Every significant XAUUSD move follows this 5-step sequence. There are no exceptions in a trending environment:

**Step 1 — LIQUIDITY FORMATION**
Retail traders cluster their stop-losses in predictable locations: above swing highs (Buy-Side Liquidity / BSL) and below swing lows (Sell-Side Liquidity / SSL). Equal highs and equal lows create the densest pools.

**Step 2 — LIQUIDITY SWEEP**
Price is algorithmically delivered into the liquidity pool. The wick extends beyond the high or low to trigger clustered orders. The candle body closes back inside the previous range. Duration: typically 1-3 candles.

**Step 3 — DISPLACEMENT**
Immediately following the sweep, a strong impulsive move occurs in the opposite direction. Large body candles, minimal wicks, creating Fair Value Gaps. This confirms institutional order execution has occurred.

**Step 4 — REBALANCE (FVG Fill)**
Price retraces into the imbalance created during displacement. Institutions use this retracement to add to positions or close earlier positions at better prices.

**Step 5 — CONTINUATION TOWARD DRAW ON LIQUIDITY**
Price resumes the direction of the displacement toward the next identified liquidity pool (opposing BSL if bullish, opposing SSL if bearish).

**XAUUSD Example — Full Sequence (NY Session, illustrative):**
- Gold builds equal lows at $2,285 over 3 sessions = SSL pool forms
- At 09:30 NY open, price spikes down to $2,278, triggering all sell-stops below $2,285
- Within 2 candles, Gold reverses with a strong bullish displacement candle (+$12), closing at $2,297, leaving a FVG between $2,287 and $2,291
- Price pulls back into the FVG at $2,288, finds support
- Gold continues to BSL above $2,315 (previous swing high)
- Full sequence: 5 steps, observable in real-time on M5/M15

---

# 2. MARKET STRUCTURE

## 2.1 Swing Highs and Swing Lows

All structure analysis begins with identifying swing points. ICT uses a specific definition:

**Swing High:** A candle whose high is higher than at least the 1 candle on its left and 1 candle on its right. On higher timeframes, use 2+ candles each side for significance.

**Swing Low:** A candle whose low is lower than at least 1 candle on its left and 1 candle on its right.

Classification:
- **Short-Term High/Low (STH/STL):** Swing formed on M1–M15, used for entry
- **Intermediate-Term High/Low (ITH/ITL):** Swing formed on H1–H4, used for bias
- **Long-Term High/Low (LTH/LTL):** Swing formed on D1–W1, used for macro direction

---

## 2.2 Trend Structure

**Bullish Market Structure:**
- Price creates a sequence of Higher Highs (HH) and Higher Lows (HL)
- Each pullback terminates above the previous swing low
- The most recent HL is the market structure low

**Bearish Market Structure:**
- Price creates a sequence of Lower Highs (LH) and Lower Lows (LL)
- Each rally terminates below the previous swing high
- The most recent LH is the market structure high

**XAUUSD Application:**
On D1, if Gold has printed HH at $2,450, HL at $2,380, HH at $2,480, HL at $2,410 — structure is bullish. Bias is long. Look for longs from discount.

---

## 2.3 Break of Structure (BOS)

**Definition:** Price closes beyond a previous significant swing high (bullish BOS) or swing low (bearish BOS), continuing the existing trend.

**BOS in a bullish trend:** Price breaks above a prior HH. This confirms the trend continues. The candle that causes the BOS is a structural confirmation candle.

**BOS in a bearish trend:** Price breaks below a prior LL. Trend continues.

**XAUUSD Example:**
Gold is bullish (HH/HL). Previous HH = $2,380. Price sweeps SSL at $2,330, displaces upward, and closes above $2,380. That close above $2,380 = Bullish BOS. Bias confirmed bullish, look for longs.

**Important:** BOS must occur with displacement (strong impulsive candle), not a gradual drift through the level. A slow grind through a level is not a valid BOS for ICT purposes.

---

## 2.4 Change of Character (CHoCH)

**Definition:** Price breaks the most recent swing in the opposite direction of the prevailing trend, signaling a potential reversal.

**Bullish CHoCH:** In a downtrend (LH/LL), price breaks above the most recent LH. This is the first signal that the trend may be shifting bullish.

**Bearish CHoCH:** In an uptrend (HH/HL), price breaks below the most recent HL. First signal of potential bearish shift.

**Distinction from BOS:**
- BOS = continuation of existing trend
- CHoCH = first signal of potential trend reversal

**One CHoCH alone is insufficient for full reversal confirmation.** A CHoCH followed by a BOS in the new direction confirms the reversal.

**XAUUSD Example:**
Gold has been in a downtrend: LH at $2,350, LL at $2,280, LH at $2,320, LL at $2,265. Gold then sweeps below $2,265 (SSL), displaces strongly upward, and closes above $2,320 (the most recent LH). That close above $2,320 = Bullish CHoCH. The trend has not yet reversed, but the first signal is present. Wait for subsequent BOS to confirm.

---

## 2.5 Market Structure Shift (MSS)

**MSS** is frequently used interchangeably with CHoCH in practice, but has a specific nuance:

- MSS specifically refers to a CHoCH accompanied by a displacement candle — a strong impulsive candle that closes beyond the swing high/low
- An MSS on LTF (M1–M5) is used as the entry trigger after a sweep on MTF (M15)
- Without displacement, it is not an MSS — it is a potential fake-out

**XAUUSD Entry Example Using MSS:**
1. M15: Equal lows swept at $2,300
2. M5: Strong bullish displacement candle closes above recent M5 high = MSS on M5
3. M1: Price retraces into FVG created by the MSS candle
4. Entry: Long at FVG on M1
5. SL: Below the sweep low at $2,297
6. TP: BSL above $2,335

---

## 2.6 Equal Highs (EQH) and Equal Lows (EQL)

**EQH (Equal Highs):** Two or more swing highs at approximately the same price level. These are the highest-probability BSL targets because retail traders clearly see this as "double top resistance" and cluster their short entry stops above it.

**EQL (Equal Lows):** Two or more swing lows at approximately the same price level. SSL target. Retail sees "double bottom support" and clusters long entry stops below.

**Rule:** EQH and EQL are not support/resistance levels in the conventional sense. They are **liquidity pools**. Price is drawn toward them to sweep, not to bounce.

**XAUUSD Example:**
Gold prints two highs at $2,400 on consecutive sessions. Retail traders place sell orders at $2,400 and stops above $2,402. The correct expectation is NOT "resistance at $2,400." The correct expectation is: "BSL pool exists above $2,400. Price will be delivered above $2,402 to sweep all sell-stops, then potentially reverse or continue."

---

# 3. LIQUIDITY — FULL TAXONOMY

## 3.1 Definition

Liquidity in ICT = clustered pending orders (stop-losses and limit orders) at specific price levels. Price is delivered toward these clusters to facilitate institutional order execution.

## 3.2 Buy-Side Liquidity (BSL)

**Location:** Above swing highs, equal highs, previous session highs, previous day/week highs, round numbers above current price.

**Composition:**
- Stop-losses of short sellers (placed above their entry high)
- Buy-stop orders of breakout buyers (triggered when price moves above a level)
- Pending buy orders of institutions collecting at certain levels

**In XAUUSD:** BSL above Asian session high, above previous day's high (PDH), above round numbers ($2,300, $2,350, $2,400, $2,500, $3,000), above obvious swing highs on H1/H4.

## 3.3 Sell-Side Liquidity (SSL)

**Location:** Below swing lows, equal lows, previous session lows, previous day/week lows, round numbers below current price.

**Composition:**
- Stop-losses of long buyers (placed below their entry low)
- Sell-stop orders of breakout sellers (triggered when price moves below a level)
- Pending sell orders from institutions

**In XAUUSD:** SSL below Asian session low, below previous day's low (PDL), below round numbers, below obvious swing lows on H1/H4.

## 3.4 Types of Liquidity by Category

### Internal Liquidity
Located within the current dealing range (between the most recent swing high and swing low). These are relatively weaker liquidity pools but serve as short-term draw targets.

Examples: FVG levels, order block midpoints, 50% retracements within range.

### External Liquidity
Located beyond the current dealing range — above the range high (BSL) or below the range low (SSL). These are the primary draw targets for institutional order flow.

Examples: Previous session high/low, previous week high/low, swing highs/lows on H4 and D1.

### Short-Term Liquidity (STL/STH Pools)
Liquidity at STH/STL levels. Used for intraday scalp targets. On XAUUSD, these are typically 15–50 pip targets.

### Long-Term Liquidity (LTH/LTL Pools)
Liquidity at D1/W1 swing highs/lows. Used for swing trade targets. On XAUUSD, these can be $20–$100 moves.

## 3.5 Stop Hunt Mechanics — Exact Sequence

When institutional order flow targets a liquidity pool:

1. **Price is delivered toward the pool** — gradual movement toward the level, no impulsive move yet
2. **Final candle spike (the sweep)** — price violently extends beyond the high/low. Wick extends 5–30 pips past the level in XAUUSD (typically $0.50–$3.00 past the level)
3. **Candle body closes back inside** — the body of the candle closes back within or near the previous range. The wick is the evidence of the sweep.
4. **Immediate displacement** — within 1–5 candles, a strong impulsive move occurs in the opposite direction
5. **Structural shift** — MSS or CHoCH occurs on LTF

**XAUUSD-Specific Stop Hunt Characteristics:**
- Gold performs "deep sweeps" — will frequently run 10–25 pips ($1.00–$2.50) past an obvious low or high before reversing, compared to 3–7 pips for major forex pairs
- Stop hunts in Gold are most impactful at 02:00–04:00 AM EST (London open) and 08:30–09:30 AM EST (NY session open)
- High-impact news releases (NFP, CPI, FOMC) are frequently used as the catalyst for the sweep, not the actual direction move

## 3.6 Identifying Liquidity in Practice — XAUUSD

**Step 1:** Mark all swing highs and lows on H4 and H1.

**Step 2:** Mark equal highs and equal lows (within $1–$2 of each other counts as "equal" in Gold).

**Step 3:** Mark previous day's high (PDH) and previous day's low (PDL). These are primary targets every session.

**Step 4:** Mark previous week's high (PWH) and previous week's low (PWL). These are the targets for larger moves.

**Step 5:** Mark round numbers ($2,300, $2,350, $2,400, etc.). Psychological levels concentrate retail stop orders.

**Step 6:** Label each pool as BSL (above price) or SSL (below price).

**Result:** You now have a liquidity map. Price delivery is a game of connecting these pools in sequence.

---

# 4. DISPLACEMENT

## 4.1 Definition

Displacement is a rapid, impulsive price movement characterized by:
- Large body candles relative to prior candles
- Minimal wicks
- Candles that leave Fair Value Gaps (imbalances between consecutive candles)
- Volume spike (observable in XAUUSD futures data; proxied by spread behavior in spot)

Displacement is the **proof of institutional execution**. When Smart Money has swept liquidity and is now filling its directional position, the aggressive buying/selling creates displacement.

## 4.2 What Displacement Is NOT

- Gradual trending movement (that is organic price movement, not displacement)
- A single large candle with no follow-through (could be news spike with no institutional continuation)
- Movement that occurs during low-liquidity periods (Asia session in Gold often produces false displacement)

## 4.3 Displacement Validation Criteria

For displacement to be valid in ICT:

1. **It must follow a liquidity sweep** — displacement without prior sweep = no institutional catalyst confirmed
2. **It must create at least one FVG** — the move must be fast enough to leave imbalance
3. **It must change market structure** — causes BOS or CHoCH
4. **It must occur during a Kill Zone** — London open or NY session displacement carries full weight; Asia displacement is unreliable

## 4.4 XAUUSD Displacement Magnitudes

| Timeframe | Minimum displacement size for validity |
|---|---|
| M1 | $0.80 – $1.50 move (8–15 pips) |
| M5 | $1.50 – $3.00 move (15–30 pips) |
| M15 | $3.00 – $8.00 move (30–80 pips) |
| H1 | $8.00 – $20.00 move (80–200 pips) |
| H4 | $20.00 – $50.00 move |

If the move is smaller than these ranges for the timeframe, treat it as consolidation, not displacement.

---

# 5. ORDER BLOCKS — COMPLETE CLASSIFICATION

## 5.1 Definition — ICT Standard

An Order Block (OB) is the **last opposing candle before a significant displacement move**. It represents the price zone where institutional orders were last placed in the opposite direction before Smart Money reversed.

**Precise definition:**
- **Bullish OB:** The last **down-close candle** (bearish candle, close below open) immediately before a bullish displacement that causes a BOS or CHoCH
- **Bearish OB:** The last **up-close candle** (bullish candle, close above open) immediately before a bearish displacement that causes a BOS or CHoCH

**Price zone of the OB:** From the candle's open to its close (body only). Some practitioners extend to include the full high-low range (wicks), but ICT standard uses the body.

## 5.2 Order Block Validation — 4 Required Conditions

An OB is only valid when ALL of the following are met. If any is missing, the candle is NOT a valid OB:

**Condition 1: Preceded by a Liquidity Sweep**
Before the OB forms, price must have swept a significant liquidity pool. The OB forms as part of the reversal sequence after the sweep. An OB without a prior sweep lacks the institutional catalyst.

**Condition 2: Followed by Strong Displacement**
The candle after the OB must be an aggressive displacement candle (or a series of displacement candles). The OB is the "last breath" of the opposing move before displacement.

**Condition 3: Creates Market Structure Change**
The displacement following the OB must result in at minimum a CHoCH, preferably a BOS on the relevant timeframe.

**Condition 4: Creates a Fair Value Gap**
The displacement after the OB must be fast enough to leave at least one FVG. If price moves away gradually with no imbalance, the move is not institutional-grade.

## 5.3 How to Draw the Order Block

**Bullish OB:**
- Identify the last bearish candle before the bullish displacement
- Box: From the **open** of that candle (top of body) to the **close** of that candle (bottom of body)
- The open is the top of the box, the close is the bottom of the box

**Bearish OB:**
- Identify the last bullish candle before the bearish displacement
- Box: From the **open** of that candle (bottom of body) to the **close** of that candle (top of body)
- The open is the bottom of the box, the close is the top of the box

**Optional Refinement:** If there are multiple consecutive candles of the same direction before the displacement, only the last one (closest to the displacement) is the refined OB. However, the entire zone of consecutive candles can serve as the broader OB zone.

## 5.4 OB Entry Zone — Optimal Entry Within the OB

When price returns to an OB, entry is placed at:

- **50% of the OB body** — standard ICT entry zone (equilibrium of the OB)
- **Distal edge (bottom of bullish OB / top of bearish OB)** — for maximum risk-reward, highest probability but lower fill rate
- **Proximal edge (top of bullish OB / bottom of bearish OB)** — entry on first touch, lower RR but higher fill

## 5.5 OB Invalidation

A bullish OB is invalidated when price closes below the low of the OB candle.
A bearish OB is invalidated when price closes above the high of the OB candle.

**XAUUSD Application:** In Gold, OB wicks can be violated (price temporarily dips below the OB body) without invalidation — the body must close beyond the OB low/high for invalidation.

## 5.6 Order Block Types — Full Classification

### A. Continuation Order Block

Occurs **within a trend**, at a pullback within the trend's structure. Price retraces to the OB and continues in the trend direction.

**Characteristics:**
- Forms at a HL in an uptrend (bullish continuation OB)
- Forms at a LH in a downtrend (bearish continuation OB)
- Displacement from OB points in the trend direction
- Higher win rate than reversal OBs
- Usually smaller magnitude (15–30 pip reaction in XAUUSD on M15)

**XAUUSD Example (Bullish Continuation OB on M15):**
- Gold uptrend: HH at $2,420, HL at $2,395, price rallying
- Price pulls back on M15, last bearish candle before bullish displacement is at $2,405 body = $2,409 (open) to $2,405 (close)
- Displacement follows: Gold rallies from $2,406 to $2,425, leaving FVG
- OB box: $2,405–$2,409 (M15)
- Price retraces to $2,406, holds
- Long entry at $2,406, SL below $2,402 (below OB), TP at $2,430 (BSL above)

### B. Reversal Order Block

Occurs at a **major swing high or low**, after a liquidity sweep, signaling a trend reversal.

**Characteristics:**
- Requires CHoCH confirmation after the OB-driven displacement
- Located at premium zone (bearish reversal OB) or discount zone (bullish reversal OB)
- Larger magnitude reaction (30–80+ pips in XAUUSD on M15/H1)
- Requires stronger confluence from HTF

**XAUUSD Example (Bearish Reversal OB on H1):**
- Gold uptrend, H4 showing gold in Premium zone
- H1 sweep: Gold spikes to $2,465 (BSL pool above $2,460 EQH), then reversal
- Last bullish H1 candle before bearish displacement: body = $2,458 (open) to $2,462 (close)
- OB box: $2,458–$2,462
- Bearish displacement: Gold drops from $2,461 to $2,440, CHoCH confirmed
- Short entry at $2,460 retest, SL above $2,465 (above sweep high), TP at $2,420 (SSL)

### C. Breaker Block (Failed OB)

Covered in full in Section 7. Summary: When an OB fails (price closes through it), it inverts polarity and becomes a Breaker Block — now acting as resistance (failed bullish OB = bearish breaker) or support (failed bearish OB = bullish breaker).

### D. Void Order Block / Empty OB

An OB that has not yet been "mitigated" (price has not returned to it). Unmitigated OBs are considered active. Once price returns to the OB and reacts, it is mitigated (used). An OB that has been fully traded through is no longer valid.

### E. Institutional Candle (1-Candle OB)

In some ICT models, a single candle that sweeps liquidity AND creates an imbalance simultaneously is treated as both an OB and the entry zone. This is common on M1 during macro times (see Section 18).

## 5.7 Common Order Block Errors — Mechanical Failures

**Error 1: No Prior Sweep**
Trading an OB that formed without a liquidity sweep. Price will likely continue through the OB rather than bounce.
Mechanical rule: If no sweep → no OB trade.

**Error 2: No Displacement**
The candles after the OB are small, gradual. This is not displacement. The OB is likely a consolidation zone, not an institutional entry point.
Mechanical rule: If post-OB candles are not impulsive with FVG → no OB trade.

**Error 3: Trading OB Against HTF Bias**
M15 bullish OB forming while H4 is bearish. The H4 bearish OB above will reject price before it can reach meaningful TP.
Mechanical rule: LTF OBs must align with HTF direction.

**Error 4: Stale OBs**
OBs that are many sessions old lose effectiveness as liquidity dynamics change. An OB that has been retested multiple times without a clean bounce is losing its significance.
Mechanical rule: Do not trade OBs that have been approached more than 2–3 times without a clean directional move.

**Error 5: Touching OBs vs. Closing Beyond Them**
Price that wicks into an OB but closes back inside is a valid test. Only a candle that closes beyond the OB body invalidates it.
Mechanical rule: Invalidation = body close beyond OB, not just a wick.

---

# 6. FAIR VALUE GAP (FVG)

## 6.1 Definition

A Fair Value Gap (FVG), also called an Imbalance or Liquidity Void, is a **three-candle pattern** where the middle candle moves so aggressively that the first and third candles do not overlap, leaving a gap that was never traded on both sides.

**Bullish FVG Formation:**
```
Candle 1: [Body][High]
                        ← GAP (FVG zone) = High of Candle 1 to Low of Candle 3
Candle 3: [Low][Body]
```
The High of Candle 1 is BELOW the Low of Candle 3. The space between = FVG.

**Bearish FVG Formation:**
```
Candle 1: [Low][Body]
                        ← GAP (FVG zone) = Low of Candle 1 to High of Candle 3
Candle 3: [Body][High]
```
The Low of Candle 1 is ABOVE the High of Candle 3. The space between = FVG.

**Validation:** If the wicks of Candle 1 and Candle 3 overlap, there is NO valid FVG. The gap must exist even at the wick level for maximum validity. (Note: some ICT students use body-to-body for FVGs; wick-to-wick is the more conservative/valid definition.)

## 6.2 Why Price Returns to Fill FVGs — The Mechanics

Three mechanical reasons:

**Reason 1: Algorithmic Rebalancing**
The IPDA (interbank algorithm) is programmed to return to zones of price inefficiency. A FVG represents a zone where orders were not matched on both sides. The algorithm seeks "efficient pricing" by returning to these zones.

**Reason 2: Institutional Partial Exit / Add**
Smart Money executing a large buy will displace price upward. When price retraces to the FVG, Smart Money may either (a) add more at a better average price, or (b) close a portion of their position to lock in profit. Either action requires price to return to the zone.

**Reason 3: Retail Stop Hunt Using FVG**
Retail traders often place stops at FVG edges. Price is delivered back to the FVG to sweep those stops before the continuation.

**FVG Fill Rate in XAUUSD:**
In trending conditions: 70–80% of FVGs are filled at least 50% before continuation.
In choppy conditions: 85–95% of FVGs are filled fully before price can continue.

## 6.3 FVG Measurement and Entry Points

**Full FVG Zone:** From the High of Candle 1 to the Low of Candle 3 (bullish FVG).

**50% (Equilibrium) of FVG:** Midpoint of the zone. This is the standard ICT entry zone within an FVG.

**Distal Edge:** The far edge from current price (lower edge of a bullish FVG = Low of Candle 3). Maximum risk-reward entry.

**Proximal Edge:** The near edge to current price (upper edge of a bullish FVG = High of Candle 1). First-touch entry.

**XAUUSD Example:**
Bullish FVG on M5: Candle 1 High = $2,305, Candle 3 Low = $2,309. FVG zone = $2,305–$2,309. FVG midpoint = $2,307. Limit buy at $2,307.

## 6.4 FVG Classification

### A. FVG as Point of Interest (POI) — Standard Use

Price returns to the FVG, holds, and continues in the direction of the original displacement.

**Requirements for valid FVG POI:**
- Preceded by a liquidity sweep
- Formed during displacement (not random price movement)
- Aligns with HTF bias
- Preferably at discount zone (for bullish FVG) or premium zone (for bearish FVG)

### B. Inversion FVG (IFVG)

When a bullish FVG has been fully filled (price trades through it), that same zone **flips polarity** and becomes a bearish zone. Price may now react to it as resistance.

Conversely, when a bearish FVG is fully filled, it can become support (bullish IFVG).

**XAUUSD Application:**
- Bullish FVG at $2,305–$2,309 was formed, price traded through it downward (full fill plus close below)
- This zone at $2,305–$2,309 is now an IFVG — acts as resistance
- When price retraces back up to $2,307, expect rejection and short opportunity

### C. FVG Continuation

FVG forms in the middle of a strong trend, price partially fills it and continues.

**Characteristic:** Only 20–40% fill before continuation. Do not wait for full fill in strong trend FVGs.

### D. FVG Reversal

FVG forms after a CHoCH/sweep, signals full reversal. Price returns, holds at FVG, and trends away.

### E. FVG as Liquidity Trap

FVG is visible to many traders who place limit orders inside it. Price fills the FVG, sweeps the limit orders (stops below the FVG), then actually reverses from below the FVG rather than at the FVG midpoint.

**Mechanical response:** When a clear FVG has obvious liquidity inside it (retail limits stacked at 50%), prefer to wait for the sweep of those limits before entry, rather than matching the retail entry.

## 6.5 FVG Timeframe Hierarchy

FVGs on higher timeframes carry more weight. Priority order for XAUUSD:

1. D1 FVG — Multi-day draw target, very high impact
2. H4 FVG — Major intraday POI
3. H1 FVG — Standard session POI
4. M15 FVG — Trade execution level
5. M5 FVG — Entry refinement
6. M1 FVG — Scalp entry only

When a D1 FVG and M15 FVG overlap, that is a strong confluence zone.

## 6.6 When NOT to Trade an FVG

- FVG formed without prior displacement (just gradual movement creating a gap) — not a valid institutional imbalance
- FVG that is directly opposed by a higher-timeframe OB or FVG — will be rejected before reaching its midpoint
- FVG formed during Asia session in XAUUSD — lower reliability; may fill partially then trap
- FVG that is more than 3–5 sessions old without being touched — liquidity dynamics have shifted
- FVG in the middle of a measured range expansion during high-impact news (NFP, FOMC) — news volatility creates false FVGs that do not follow normal ICT mechanics

---

# 7. BREAKER BLOCKS

## 7.1 Definition

A Breaker Block is a **failed Order Block that has been violated**. When price closes beyond an OB (the body closes through it), that OB has "failed" and is converted into a Breaker Block.

A Breaker Block operates with **inverted polarity**:
- Failed Bullish OB → Bearish Breaker Block (now acts as resistance)
- Failed Bearish OB → Bullish Breaker Block (now acts as support)

## 7.2 Mechanics — Why Breakers Form

When traders buy a bullish OB and price breaks through it, those traders are now in losing long positions. Their stop-losses are triggered (sell orders). Additionally, when price returns to that zone later, those same traders may want to exit at breakeven, adding more sell pressure at that zone. This is why a broken bullish OB becomes resistance.

**Institutional mechanism:** Smart Money used the OB level to distribute positions to retail buyers. When price breaks through, institutions have fully exited longs. The zone now serves as distribution overhead.

## 7.3 Breaker Block Validation

For a valid Breaker Block:

1. **Original OB must have been a valid OB** (had prior sweep, displacement, and FVG)
2. **Price must close the body through the OB** — wick violations are not Breaker triggers
3. **A new swing high (bullish breaker) or swing low (bearish breaker) must form** after the break
4. **Price must not have run far from the broken OB** — breakers lose strength if price has moved 100+ pips away before returning

## 7.4 Breaker Block Entry

Entry is placed when price **returns (retraces)** to the Breaker Block zone after the break.

**Bearish Breaker Block Entry (XAUUSD Short):**
- Bullish OB was at $2,350–$2,355
- Price closed below $2,350 (OB low), break confirmed
- Price rallies back to $2,352–$2,355
- Short entry at $2,353 (within breaker zone)
- SL above $2,358 (above original OB high)
- TP: Next SSL pool below

**Bullish Breaker Block Entry (XAUUSD Long):**
- Bearish OB was at $2,390–$2,395
- Price closed above $2,395 (OB high), break confirmed
- Price pulls back to $2,392–$2,395
- Long entry at $2,393
- SL below $2,388
- TP: Next BSL pool above

## 7.5 Breaker vs. Regular OB — Key Distinction

| Feature | Order Block | Breaker Block |
|---|---|---|
| Formation | Last opposing candle before displacement | Failed OB after price closes through it |
| Polarity | Trades in direction of displacement | Trades in OPPOSITE direction of original OB intent |
| Entry timing | On first retest of OB after displacement | After OB fails, on retest from opposite side |
| Strength | Moderate-High | High (trapped traders add pressure) |
| XAUUSD frequency | Very common | Moderate |

---

# 8. MITIGATION BLOCKS

## 8.1 Definition

A Mitigation Block is a **bearish candle range in a bullish context (or bullish candle in bearish context) that has been partially but not fully mitigated by returning price**.

More precisely: When price creates a displacement candle that sweeps an OB and only partially revisits the OB zone, the portion that was NOT revisited is the mitigation zone.

## 8.2 Origin of the Term

"Mitigation" = the act of institutions closing (offsetting) their earlier losing positions. When institutions bought at an OB and price moved against them, they wait for price to return to that OB to close their losing trades. When they do, the selling from their exits creates a resistance zone.

## 8.3 In PD Array Order (ICT Priority)

ICT places Mitigation Blocks high in the PD (Price Delivery) Array hierarchy:
1. Mitigation Block (highest institutional weight)
2. Bullish/Bearish Breaker
3. Liquidity Void
4. Fair Value Gap
5. Order Block
6. Rejection Block
7. Old High / Old Low (lowest weight)

## 8.4 XAUUSD Application

**Example:**
- Gold drops from $2,400 to $2,300 (bearish move). At $2,350, a bearish OB forms.
- Gold later rallies from $2,300 back upward. The rally only reaches $2,348 (does not fully enter the $2,350–$2,355 OB zone) before dropping again.
- The zone $2,348–$2,355 (un-mitigated portion) = Mitigation Block.
- Next time Gold approaches $2,348–$2,355, treat as strong resistance.

---

# 9. REJECTION BLOCKS

## 9.1 Definition

A Rejection Block is formed when a candle has a **significantly large wick in one direction** that represents concentrated institutional rejection. The wick itself — not the body — is the Rejection Block zone.

**Bullish Rejection Block:** A candle with a very long lower wick (price was violently rejected from below). The lower wick is the zone. Price may return to the lower wick level and find support.

**Bearish Rejection Block:** A candle with a very long upper wick. Price was rejected from above. Upper wick = resistance zone.

## 9.2 Distinction from Regular Support/Resistance

Rejection Blocks are not generic candle tails. They must occur:
- At a confluence of other ICT concepts (swept liquidity, at an OB, at a FVG)
- During a Kill Zone
- With sufficient wick magnitude (for XAUUSD: at least 20–30 pip wick)

Without these conditions, a long wick is simply noise.

---

# 10. BALANCED PRICE RANGE (BPR)

## 10.1 Definition

A Balanced Price Range is formed when **two opposing FVGs overlap** — a bullish FVG and a bearish FVG that share the same price zone. The overlapping area is where the market is "balanced" (traded on both sides).

## 10.2 Mechanics

When a bullish FVG forms (price $2,300–$2,310 gap) and then a bearish FVG forms that overlaps with it ($2,305–$2,315 gap), the overlapping zone ($2,305–$2,310) is the BPR. Price tends to oscillate within the BPR before a decisive directional break.

## 10.3 Trading the BPR

**Do not trade within a BPR.** A BPR signals equilibrium — price is equally balanced. Wait for price to break out of the BPR zone before entering.

**After a BPR breakout:**
- Price breaks above BPR → bullish, enter longs at retest of BPR top
- Price breaks below BPR → bearish, enter shorts at retest of BPR bottom

---

# 11. LIQUIDITY VOIDS

## 11.1 Definition

A Liquidity Void is a **large displacement that spans multiple FVGs simultaneously** — the price moved so fast that it created a vacuum of liquidity across a wide price range. The entire range from the origin of the displacement to its termination is the Liquidity Void.

Unlike a single FVG (3-candle pattern), a Liquidity Void may span 10–30 candles all moving in one direction with no meaningful retracement.

## 11.2 Behavior

Price will eventually return to fill the Liquidity Void, typically in multiple visits. A Liquidity Void acts as a "magnet" on a larger scale than a single FVG.

**XAUUSD Example:**
On D1, Gold drops from $2,450 to $2,280 in 5 days with no significant pullback. This creates a Liquidity Void from $2,280 to $2,450. When Gold starts recovering, price will likely retrace through this entire void over several weeks, filling individual FVGs within it along the way.

---

# 12. PREMIUM & DISCOUNT ZONES — PD ARRAYS

## 12.1 The Dealing Range Concept

The "Dealing Range" is the reference range from which premium and discount are measured. It is defined by the most recent significant swing high and swing low at the HTF.

**Formula:**
- Dealing Range High = Most recent significant swing high on HTF (H4 or D1)
- Dealing Range Low = Most recent significant swing low on HTF
- Range Size = High − Low

## 12.2 Premium and Discount Zones

```
100% = Dealing Range High (most recent HTF swing high)
 75% = Premium Zone (Upper Quarter)
 50% = Equilibrium / Midpoint
 25% = Discount Zone (Lower Quarter)
  0% = Dealing Range Low (most recent HTF swing low)
```

**Mechanical Rules:**
- Long entries: Only at Discount (below 50% of dealing range)
- Short entries: Only at Premium (above 50% of dealing range)
- Trading at Equilibrium: Only with strong confirmation; lowest probability entry zone
- Targets: Buy from Discount, targeting BSL above Dealing Range High; Sell from Premium, targeting SSL below Dealing Range Low

## 12.3 XAUUSD Application

**Setup Example:**
- D1 Dealing Range: Swing Low at $2,300, Swing High at $2,450
- Range Size: $150
- Equilibrium: $2,375
- Discount Zone: Below $2,375 (optimally below $2,337 — lower quartile)
- Premium Zone: Above $2,375 (optimally above $2,412 — upper quartile)

**Bias: Gold has been bullish (HH/HL on D1).**
- Look for long setups ONLY when Gold is in the Discount Zone ($2,300–$2,375)
- Specifically target entries at institutional POIs within Discount: OBs, FVGs, Breaker Blocks in the $2,300–$2,350 range
- TP target: BSL above $2,450

## 12.4 PD Array Hierarchy — Order of Strength

When multiple ICT concepts align within a Discount/Premium zone, use this hierarchy to determine which is strongest:

1. **Mitigation Block** — strongest (trapped institutional positions)
2. **Breaker Block** — very strong (failed OB, trapped retail)
3. **Inversion FVG** — strong (filled FVG that flipped polarity)
4. **Fair Value Gap** — standard
5. **Order Block** — standard
6. **Rejection Block** — moderate
7. **Old High / Old Low** — weakest on its own

When multiple PD arrays overlap (OB + FVG + Discount zone), that confluence zone is a high-probability entry.

---

# 13. POWER OF THREE (AMD MODEL)

## 13.1 Overview

The Power of Three (PO3), also called the AMD model (Accumulation-Manipulation-Distribution), describes the three phases that every trading session — and every candle on any timeframe — follows due to institutional order delivery.

This concept is directly applicable to XAUUSD's daily session behavior.

## 13.2 The Three Phases

### Phase 1: ACCUMULATION

**Definition:** Smart Money builds positions during a consolidation phase. Price moves in a narrow range. There is no clear directional momentum.

**Characteristics:**
- Low volatility, small candle bodies
- Price oscillates around the opening price (Midnight Open for New York-based ICT traders)
- Retail traders have no directional clarity
- Occurs primarily during the Asian session (00:00–07:00 NY time)

**What Smart Money is doing:**
- Accumulating long positions (if the day will be bullish) or short positions (if bearish)
- Building the "energy" for the manipulation phase

**XAUUSD Observation:** Gold's Asian session typically ranges 20–50 pips (XAUUSD). The high and low of the Asian session mark the BSL and SSL that will be targeted in the next phase.

### Phase 2: MANIPULATION (Judas Swing)

**Definition:** Price moves sharply in the **opposite direction of the true daily move** to:
1. Sweep liquidity on the wrong side
2. Trap retail traders into positions that will be stopped out
3. Create the entry opportunity for Smart Money to build full position

**Characteristics:**
- Aggressive move against the actual daily direction
- Occurs typically at London Open (02:00–04:00 AM NY time)
- Takes out obvious liquidity: Asian session high or low, round numbers, previous session levels
- Creates a liquidity sweep + displacement sequence

**The Judas Swing in XAUUSD:**
On a bullish day: Gold drops 30–60 pips in the London open, sweeping the Asian session low and previous SSL. Retail sellers enter, longs are stopped out. Gold immediately reverses and the true bullish move begins.

On a bearish day: Gold spikes 30–60 pips at London open, sweeping Asian session high and BSL. Retail buyers enter, shorts are stopped out. Gold immediately reverses downward.

**The Midnight Open (00:00 NY Time):**
ICT uses the 00:00 NY time (Midnight Open) as the reference price for each day. The Manipulation phase moves price away from this Midnight Open price (false direction). The rule: if price trades below the Midnight Open on a bullish day, that is the Judas Swing trap. If price closes back above the Midnight Open with displacement, the true bullish move is beginning.

### Phase 3: DISTRIBUTION

**Definition:** The true directional move plays out. Smart Money delivers price toward the day's intended draw on liquidity.

**Characteristics:**
- Strong, sustained move in the true direction
- Occurs primarily during NY AM session (08:30–12:00 NY time)
- May include minor pullbacks that fill internal FVGs
- Terminates at the session's draw on liquidity (PDH, PWH, BSL above, or PDL, PWL, SSL below)

**XAUUSD Typical Profile on a Bullish Day:**
- 00:00–07:00: Asian consolidation, Gold ranges between $2,350–$2,370
- 07:00–09:00 (London): Judas Swing down to $2,338, sweeps previous SSL at $2,340. Retail bears enter.
- 09:00–09:30: Gold displacement candles back above $2,350 (Midnight Open), CHoCH on M15
- 09:30–13:00 (NY AM): Gold distributes to $2,400 (BSL at PDH target)
- Total daily range: ~$62 move on the true direction side

## 13.3 How to Trade AMD on XAUUSD

**Step 1:** Identify Midnight Open at 00:00 NY time (00:00 EST / GMT-5).

**Step 2:** Mark the Asian session high and low (00:00–07:00 NY). These are the Manipulation targets.

**Step 3:** Determine daily bias using D1/H4 analysis (bullish or bearish).

**Step 4:** If bullish bias, wait for a London/NY open sweep of the Asian session low (Judas Swing down).

**Step 5:** Look for MSS on M5/M15 after the sweep (bullish displacement, CHoCH).

**Step 6:** Enter long at FVG or OB created by the displacement.

**Step 7:** Target: BSL above Asian session high, PDH, or weekly high.

**Entry Timing Rule:** Do not enter during Accumulation (Asia). Do not enter during Manipulation (you cannot know it's the Judas Swing until displacement occurs). Enter only after Displacement confirms that Manipulation is complete.

---

# 14. INTERBANK PRICE DELIVERY ALGORITHM (IPDA)

## 14.1 What Is IPDA

The Interbank Price Delivery Algorithm (IPDA) is Michael Huddleston's framework for understanding the algorithmic system that delivers prices in interbank markets. According to ICT, price does not move randomly but is governed by a time-and-price algorithm that seeks specific liquidity pools in defined time windows.

**Core principle:** The algorithm scans back 20, 40, and 60 trading days to identify significant highs and lows within each period. These highs and lows represent liquidity pools that the algorithm targets.

## 14.2 IPDA Cycles — 20/40/60 Day Lookback

| Cycle | Lookback | Market Phase |
|---|---|---|
| 20-Day | Most recent 20 trading days | Short-term trend and retracement |
| 40-Day | Most recent 40 trading days | Intermediate trend |
| 60-Day | Most recent 60 trading days | Long-term bias and major liquidity targets |

**How to Apply:**
- On D1 chart, mark the 20-day high and low, 40-day high and low, 60-day high and low
- These highs and lows are the draw on liquidity targets
- Price will be delivered toward the most recently unswept pool within the current cycle

**XAUUSD Application:**
- If the 20-day high has not been swept, but the 20-day low was recently swept with displacement, the 20-day high is the next algorithmic draw target
- Trade in the direction of the identified IPDA draw

## 14.3 IPDA Reference Points for XAUUSD Daily Trading

Key reference prices that the IPDA algorithm respects:

- **Midnight Open (00:00 NY):** Daily reference price; used to determine if manipulation is occurring above or below
- **Previous Day's High (PDH):** Primary daily BSL target
- **Previous Day's Low (PDL):** Primary daily SSL target
- **Previous Week's High (PWH):** Weekly BSL target
- **Previous Week's Low (PWL):** Weekly SSL target
- **Opening Price of the Week (Monday open):** Weekly bias reference
- **Opening Price of the Month:** Monthly bias reference

**Rules:**
- PDH and PDL are drawn every day as mandatory levels
- PWH and PWL are drawn every week as mandatory levels
- If current price is below PDH and has bullish structure, PDH is the draw target
- If current price is above PDL and has bearish structure, PDL is the draw target

---

# 15. KILL ZONES & SESSION STRUCTURE

## 15.1 Definition of Kill Zone

A Kill Zone is a specific time window during which institutional participation is at its highest. During these windows, liquidity sweeps and displacements are most reliable and have the highest probability of follow-through.

**Outside of Kill Zones:** Price movement is lower quality, more random, more prone to fake-outs.

## 15.2 Kill Zone Schedule for XAUUSD

All times are New York Time (EST / EDT):

### London Kill Zone (Most Important for XAUUSD — London Open)
**Time:** 02:00 AM – 05:00 AM NY Time

**Characteristics:**
- London is the world's largest forex and gold trading center
- European banks come online, institutional orders flood the market
- Judas Swing typically occurs in this window (false move to sweep Asian range)
- The true directional move of the day often begins in this window
- High-impact European news (ECB meetings, European CPI) releases during this period

**What to watch:** Asian session high/low sweep, then displacement in the true direction.

### New York Kill Zone (Highest Volume for XAUUSD)
**Time:** 07:00 AM – 10:00 AM NY Time

**Sub-zones:**
- **Pre-Market (07:00–08:30):** Early institutional positioning
- **US Market Open (08:30–10:00):** Maximum XAUUSD volatility, highest volume, US economic data releases

**Characteristics:**
- Overlaps with London close; combined European + US flow creates most aggressive moves
- NFP, CPI, PPI, FOMC releases occur at 08:30 AM or 14:00 PM — Gold moves 30–150 pips in seconds
- The AMD model's Distribution phase typically occurs here
- Best window for catching the day's main move

### New York PM Kill Zone (Secondary)
**Time:** 13:30 PM – 16:00 PM NY Time

**Characteristics:**
- Lower volume than NY AM
- Opportunity: Silver Bullet setups (see Section 19)
- Institutional closing of the day's positions
- London close at 11:00 AM NY creates a volatility spike sometimes

### Asian Session (XAUUSD — Avoid or Trade Carefully)
**Time:** 18:00 PM – 23:00 PM NY Time (18:00 Sunday to open Monday is the weekly open)

**Characteristics:**
- Lowest volume in XAUUSD
- Primarily accumulation phase (AMD model)
- False sweeps common — Asian liquidity sweeps are frequently reversed in London
- Spread widens in some brokers during Asia
- **Standard ICT rule for XAUUSD: Do not trade the Asian session unless specific conditions are met (e.g., Asia trending more than 100 pips, creating a clear sweep of the previous day's level)**

## 15.3 Kill Zone by GMT+7 (Vietnam Time — for reference)

| Kill Zone | NY Time | GMT+7 |
|---|---|---|
| London Open | 02:00–05:00 AM EST | 14:00–17:00 (2PM–5PM) |
| London Close / NY Overlap | 08:30–11:00 AM EST | 20:30–23:00 (8:30PM–11PM) |
| NY AM | 07:00–10:00 AM EST | 19:00–22:00 (7PM–10PM) |
| NY PM | 13:30–16:00 PM EST | 01:30–04:00 AM next day |
| Asia | 18:00–23:00 PM EST | 06:00–11:00 AM (avoid) |

## 15.4 ICT Macros

Macros are the highest-precision time windows within Kill Zones. ICT identifies specific 20–30 minute windows where algorithmic activity is most concentrated.

**Primary XAUUSD Macros (NY Time):**

| Macro Name | Time | Description |
|---|---|---|
| **London Open Macro** | 02:33–03:00 AM | Sweep of Asian range, first significant Gold move |
| **London AM Macro** | 04:03–04:30 AM | Secondary London setup |
| **NY Open Macro** | 08:50–09:10 AM | Major — often the Gold daily high or low forms here |
| **NY AM Macro** | 10:00–10:30 AM | Continuation or reversal of AM move |
| **NY PM Macro** | 13:10–13:40 PM | Silver Bullet window (Section 19) |
| **NY Close Macro** | 14:50–15:10 PM | Daily candle range completion |

**Rule:** During a macro window, if a valid setup exists (sweep + FVG + MSS), the probability of follow-through is significantly elevated compared to the same setup outside a macro window.

---

# 16. OPTIMAL TRADE ENTRY (OTE)

## 16.1 Definition

The Optimal Trade Entry (OTE) is the highest-probability entry zone within a retracement, defined by Fibonacci levels. It represents the zone where Smart Money most frequently adds to or initiates new positions after a displacement.

**OTE Zone: 61.8% to 79% Fibonacci retracement of the displacement leg.**

The logic: Smart Money executes at the extremes (sweep, displacement origin). Retail chases price. Smart Money then waits for retail's stop-losses (above the OTE retracement) and adds to their position at the 61.8–79% retracement.

## 16.2 How to Draw OTE

**For a bullish setup:**
1. Identify the displacement leg: from the Sweep Low (point A) to the Displacement High (point B)
2. Draw Fibonacci from A (0%) to B (100%)
3. OTE Zone = 61.8% to 79% retracement levels (price zone between these two)
4. Place limit buy within this zone

**For a bearish setup:**
1. Displacement leg: from Sweep High (A) to Displacement Low (B)
2. Fibonacci from A (0%) to B (100%)
3. OTE Zone = 61.8% to 79% retracement (price zone between these two)
4. Place limit sell within this zone

## 16.3 OTE in XAUUSD — Practical Example

**Bullish OTE Setup:**
- Gold sweeps SSL at $2,280 (point A = sweep low)
- Displacement: Gold rallies to $2,320 (point B = displacement high)
- Displacement leg: $40 range
- 61.8% retracement from $2,320 = $2,320 − ($40 × 0.618) = $2,320 − $24.72 = $2,295.28
- 79% retracement from $2,320 = $2,320 − ($40 × 0.79) = $2,320 − $31.60 = $2,288.40
- OTE Zone: $2,288.40 – $2,295.28
- Place limit buy at $2,291 (midpoint of OTE zone)
- SL: Below $2,278 (below sweep low, with buffer)
- TP: BSL above — previous high at $2,350

**Invalidation:** If price closes below the OTE low ($2,288.40), the OTE entry is invalid. If price trades to $2,280 (below sweep low), the entire setup is invalid.

## 16.4 OTE + FVG Confluence

The highest-probability setup is when the OTE zone overlaps with an FVG:
- OTE zone: $2,288–$2,295
- FVG from displacement: $2,290–$2,294
- Overlap: $2,290–$2,294 = Optimal entry zone with FVG + OTE confluence

**Limit buy at $2,292 (midpoint of overlap zone).**

## 16.5 OTE Alone Is Not Sufficient

OTE requires:
1. Prior liquidity sweep
2. Displacement with FVG
3. MSS on LTF
4. HTF bias alignment
5. Kill Zone timing

Without these, a 62–79% retracement is just a retracement with no ICT edge.

---

# 17. INDUCEMENT (IDM)

## 17.1 Definition

Inducement is a **deliberate minor sweep or liquidity grab** designed to pull retail traders into the wrong side of the market before the actual setup occurs. It is a smaller Judas Swing within the larger Manipulation phase.

**Purpose:** Create counterparty positions for Smart Money to trade against. If Smart Money wants to go long, they need retail traders to be short. Inducement creates those short positions by appearing to break down.

## 17.2 Inducement vs. Real Sweep — Distinction

| Feature | Inducement | Real Sweep |
|---|---|---|
| Magnitude | Small (5–20 pips in Gold) | Larger (20–60+ pips) |
| Displacement after | None / weak | Strong and creates FVG |
| MSS after | None | Yes — BOS or CHoCH |
| Volume | Typically declining | Spike |
| Purpose | To trap retail, set up real sweep | Actual liquidity collection |

## 17.3 Identifying Inducement in XAUUSD

**Scenario:** Gold is trending down, making equal lows at $2,300. You expect a sweep of those lows before a reversal.

1. Gold dips to $2,297 (just below $2,300) — appears to sweep the equal lows
2. But: The move is only 3 pips below, no displacement, no MSS
3. This is Inducement — it triggered some retail longs (thinking the sweep is done) while simultaneously triggering some retail stop-losses
4. Gold then drops further to $2,280 — THIS is the real sweep
5. After $2,280: Strong bullish displacement, MSS on M5, FVG formed
6. Entry: Long in FVG around $2,288

**Rule:** After an apparent sweep with no displacement, treat it as possible inducement. Wait for a larger sweep with actual displacement before entering.

## 17.4 Inducement Levels

Inducement is often visible as:
- A minor higher low slightly above a key SSL (trapping longs into thinking price won't go lower)
- A minor lower high slightly below a key BSL (trapping shorts)
- A "tease" of an FVG that price enters briefly and then exits without completing the fill

---

# 18. ICT MACROS

## 18.1 What Macros Are

ICT Macros are specific **20–30 minute time windows** within each trading session where the IPDA algorithm creates predictable price delivery sequences. During these windows, the algorithm frequently executes a mini-AMD cycle (accumulation, sweep, displacement) in compressed form.

## 18.2 Trading ICT Macros in XAUUSD

**Setup during a macro window:**
1. Identify the current price relative to the nearest liquidity pool (BSL or SSL within 20–40 pip range)
2. As the macro begins, watch for a sweep of the identified liquidity level
3. Immediately after sweep: identify FVG on M1 or M2
4. Enter at FVG 50% within the macro window
5. Target: Opposing short-term liquidity (typically 15–30 pips in Gold)

**Key Macro Windows for XAUUSD (NY Time):**

**08:50–09:10 AM (NY Open Macro) — Most important for XAUUSD:**
- High-impact US data often released at 08:30
- The macro window from 08:50–09:10 shows the true institutional direction after the initial news volatility
- If Gold swept down at 08:30 news, expect bullish displacement at 08:50–09:00
- FVG formed at 08:55 on M1 = high-probability entry zone

**10:00–10:30 AM (NY AM Macro):**
- Markets open fully (US stocks open at 09:30, volume ramps by 10:00)
- Gold frequently makes a secondary move: either continuation of the AM direction or an intraday pullback to the macro's FVG
- Setup: If Gold made a bullish run from 08:30–10:00, a retracement to a M5 FVG within the 10:00–10:30 window = continuation long setup

**02:33–03:00 AM (London Open Macro):**
- Judas Swing executes here in London open
- Watch for sweep of Asian session low (bullish day) or high (bearish day)
- Displacement must follow within the macro window for validity

---

# 19. SILVER BULLET STRATEGY

## 19.1 Overview

The Silver Bullet is an ICT intraday strategy that targets specific one-hour windows three times per day. It is based on liquidity sweeps and FVG entries within tight time constraints.

**Silver Bullet Windows (NY Time):**
1. **London Open:** 03:00 AM – 04:00 AM NY Time
2. **NY AM:** 10:00 AM – 11:00 AM NY Time
3. **NY PM:** 14:00 PM – 15:00 PM NY Time

## 19.2 Silver Bullet Rules — Step by Step

1. **Identify daily bias** from H4/D1 (bullish or bearish) before the window opens
2. **When the window opens, identify the nearest liquidity pool** in the direction opposite to your bias (the sweep target)
3. **Wait for price to sweep that liquidity** (wick through the high/low, close back inside)
4. **Identify the FVG** created by the sweep candle's displacement
5. **Enter at 50% of the FVG** (limit order)
6. **SL:** Beyond the sweep wick (3–5 pip buffer in Gold)
7. **TP:** Opposing internal liquidity, typically 15–30 pips in XAUUSD for this scalp setup

## 19.3 Silver Bullet XAUUSD Example (NY AM, 10:00–11:00)

- Daily bias: Bullish (D1 uptrend, Gold at discount)
- 10:00 AM: Gold at $2,358, SSL pool at $2,352 (previous M15 low)
- 10:03 AM: Gold drops to $2,350, sweeping SSL at $2,352
- 10:04 AM: Bullish displacement candle on M1 — body from $2,350 to $2,357, creating FVG $2,353–$2,356
- Limit buy at $2,354.50 (50% of FVG)
- SL: $2,348.50 (below sweep low $2,350 + 0.50 buffer) = $6 risk = 60 pips
- TP: $2,368 (BSL at previous M15 high) = $13.50 = 135 pips
- RR: 1:2.25

**Strict rule:** If no sweep + FVG occurs within the 60-minute window, NO TRADE. Do not force a setup.

---

# 20. JUDAS SWING

## 20.1 Definition

The Judas Swing is the false directional move that constitutes the Manipulation phase of the AMD model. It is named after the biblical reference to betrayal — the market appears to move in one direction to "betray" retail traders before moving in the true direction.

## 20.2 Judas Swing Mechanics in XAUUSD

**On a bullish day:**
- Gold opens the session (London or NY) below current level
- Drops aggressively, sweeping SSL (previous session low, Asian session low, PDL)
- Retail traders see breakdown, sell or add shorts
- Gold immediately reverses: displacement upward, CHoCH on M5/M15
- True move is upward for the rest of the session

**On a bearish day:**
- Gold opens and spikes upward, sweeping BSL (Asian session high, PDH)
- Retail traders see breakout, buy or add longs
- Gold immediately reverses: displacement downward, CHoCH on M5/M15
- True move is downward for the rest of the session

## 20.3 Identifying the Judas Swing in Real Time

You cannot identify the Judas Swing until it is **over** (i.e., displacement has confirmed the reversal). This is critical: entering during the manipulation phase is the most common ICT error.

**Confirmation that Judas Swing is complete:**
1. Price swept a significant liquidity level (SSL or BSL)
2. Displacement candle(s) appear in the opposite direction
3. A CHoCH or BOS occurs on M5 or M15
4. An FVG is left by the displacement

**Only after all 4 conditions = Judas Swing confirmed = Entry zone identified.**

## 20.4 XAUUSD Judas Swing Size Reference

Gold's Judas Swing is larger than typical forex pairs:
- Typical Judas Swing in XAUUSD: 30–70 pips ($3.00–$7.00)
- During high-impact news: 50–150 pips
- During normal sessions: 25–50 pips

This means SL must be placed well beyond the Judas Swing extreme. A 10-pip SL will be almost certainly hit by the tail of the Judas Swing before the true move begins.

---

# 21. MULTI-TIMEFRAME FRAMEWORK (TOP-DOWN ANALYSIS)

## 21.1 The Principle

ICT analysis flows strictly from higher timeframe to lower timeframe. Higher timeframes define the direction and key levels. Lower timeframes define the entry timing and precision.

**Non-negotiable rule:** A lower timeframe setup that contradicts the higher timeframe bias is invalidated. Always.

## 21.2 XAUUSD Timeframe Hierarchy

| Timeframe | Role | Primary Question |
|---|---|---|
| **Monthly (MN)** | Macro direction | Is Gold in a multi-month bull or bear phase? |
| **Weekly (W1)** | Weekly bias | Where will this week's liquidity be targeted? |
| **Daily (D1)** | Daily bias | Is Gold seeking BSL or SSL today? |
| **4-Hour (H4)** | Intermediate structure | What is the current swing structure? Where are the key OBs and FVGs? |
| **1-Hour (H1)** | Confirmation | Where is the POI for entry? |
| **15-Minute (M15)** | Setup identification | Where did the sweep occur? Where is the FVG? |
| **5-Minute (M5)** | Entry trigger | Where is the MSS? What is the precise FVG or OB? |
| **1-Minute (M1)** | Entry refinement | Exact limit order placement within FVG |

## 21.3 Top-Down Analysis Workflow — Step by Step

**Step 1: Monthly/Weekly Analysis**
- Determine long-term trend (HH/HL or LH/LL on Weekly)
- Identify weekly liquidity pools (PWH, PWL, range EQH/EQL)
- Determine which pool is likely the weekly target: BSL above or SSL below
- Note major PD arrays on D1 that coincide with weekly liquidity

**Step 2: Daily Analysis**
- Confirm H4 trend structure matches D1 directional intent
- Identify daily bias: bullish (targeting PDH/BSL) or bearish (targeting PDL/SSL)
- Mark: PDH, PDL, previous session high/low, significant D1 FVGs and OBs
- Identify current premium/discount on D1 dealing range

**Step 3: H4 / H1 Analysis**
- Identify the specific OBs, FVGs, and Breaker Blocks that align with the daily bias
- These are the POIs where price will react
- Note: Are we in H4 premium (seeking H4 bearish OB for shorts) or H4 discount (seeking H4 bullish OB for longs)?

**Step 4: M15 Analysis**
- When a Kill Zone activates, watch M15 for the liquidity sweep
- Identify the sweep: has price taken a significant M15 or H1 high/low?
- Identify displacement: does a strong M15 candle follow the sweep?
- Identify the M15 FVG created by displacement

**Step 5: M5 / M1 Analysis**
- Drop to M5 for CHoCH/MSS confirmation
- Identify the M5 FVG or OB within the displacement
- Confirm entry zone overlaps with premium/discount at this level
- Place limit order at FVG 50% or OB 50%
- Set SL beyond the sweep extreme

**Step 6: Trade Management**
- TP1: Nearest internal liquidity (15–20 pips away = partial profit on 50% of position)
- Move SL to breakeven after TP1
- TP2: External liquidity target (PDH, PWH, etc.) = remaining 50% of position
- Do not move TP1 or TP2 targets once set

---

# 22. FULL TRADE EXECUTION MODEL — XAUUSD

## 22.1 Bullish Trade Execution (Long Setup)

**Prerequisites (all must be true before proceeding):**
- D1/H4 shows bullish structure (HH/HL)
- Current price is in D1 Discount Zone (below 50% of D1 dealing range)
- Daily bias is bullish (targeting BSL)
- Kill Zone is active or approaching (London or NY)

**Execution Steps:**

**Step 1 — Identify SSL Target**
Mark the nearest SSL pool: equal lows on M15/H1, PDL, session low.
Example: Equal lows at $2,295 on H1.

**Step 2 — Wait for Sweep**
Price must drop below $2,295, create a wick below it, and close back above $2,295.
Example: Gold wicks to $2,291, closes at $2,296.

**Step 3 — Confirm Displacement**
Within 1–3 candles of the sweep, a strong bullish M15 candle (or series) appears.
The candle(s) must: have a large body, close well above the sweep candle's open, create an FVG.
Example: M15 candle rallies from $2,293 to $2,308 (15 pip body), creating FVG at $2,300–$2,304.

**Step 4 — Confirm CHoCH/MSS on M5**
Drop to M5. Price must break above the most recent M5 LH (change of character on M5).
Example: M5 LH was $2,302. A M5 candle closes at $2,304. CHoCH on M5 confirmed.

**Step 5 — Identify Entry Zone**
Use M5 FVG or M1 FVG created during displacement.
OTE: Draw Fibonacci from $2,291 (A) to $2,308 (B). OTE zone = $2,308 − (17 × 0.618) to $2,308 − (17 × 0.79) = $2,297.5 – $2,294.6.
Check if FVG overlaps with OTE: FVG $2,300–$2,304 is slightly above OTE. Use FVG as primary entry.

**Step 6 — Set Orders**
Limit buy: $2,302 (50% of FVG $2,300–$2,304)
SL: $2,289 (2 pips below sweep low $2,291) = $13 risk
TP1: $2,315 (internal BSL — previous M15 high) = $13 RR 1:1 → partial close 50%
TP2: $2,335 (PDH / BSL pool) = $33 RR 1:2.5 on remaining 50%

**Step 7 — Post-Entry Management**
After TP1 hit: Move SL to $2,299 (above entry, breakeven protection).
Hold remaining 50% to TP2.
If price shows bearish CHoCH on M5 before TP2: close remaining position manually.

---

## 22.2 Bearish Trade Execution (Short Setup)

**Prerequisites (all must be true):**
- D1/H4 shows bearish structure (LH/LL)
- Current price is in D1 Premium Zone (above 50% of D1 dealing range)
- Daily bias is bearish (targeting SSL)
- Kill Zone active

**Steps:**

**Step 1 — Identify BSL Target**
Mark nearest BSL: equal highs on M15/H1, PDH, session high.
Example: Equal highs at $2,410 on H1.

**Step 2 — Wait for Sweep**
Price spikes above $2,410, creates wick above, closes back below.
Example: Gold wicks to $2,414, closes at $2,408.

**Step 3 — Confirm Displacement**
Strong bearish M15 candle(s) after the sweep, creating bearish FVG.
Example: M15 candle from $2,411 to $2,395, FVG $2,402–$2,406 (bearish FVG: High of C3 to Low of C1).

**Step 4 — CHoCH on M5**
Price breaks below most recent M5 HL. CHoCH on M5 confirmed.

**Step 5 — Entry Zone**
Limit sell at FVG 50%: $2,404
SL: $2,416 (2 pips above sweep high $2,414) = $12 risk
TP1: $2,392 (internal SSL — previous M15 low) = $12 RR 1:1
TP2: $2,370 (PDL / major SSL) = $34 RR 1:2.8

---

## 22.3 Entry Type Options

### Option A: Limit Order (Standard)

Place a limit order at the FVG/OB zone before price reaches it.

**Pros:**
- Better entry price
- Precise risk control
- Can set and step away

**Cons:**
- Price may not return to zone (missed entry)
- No additional confirmation at entry

### Option B: Market Order After Confirmation

Wait for a confirmation pattern at the FVG/OB before entering:
- M1 bullish candle body closes within the FVG = market buy
- Or: Wait for a M1 MSS within the FVG zone

**Pros:**
- Additional confirmation at point of entry
- Confirms price is respecting the zone

**Cons:**
- Entry price is worse (5–10 pips worse in Gold typically)
- Risk-reward ratio is reduced

**ICT Standard:** Limit orders within FVG/OTE for maximum RR. Market orders for confirmation entries when volatility is high.

---

# 23. RISK & POSITION MANAGEMENT

## 23.1 Core Risk Rules — Non-Negotiable

These rules do not change based on "market conditions," "high-confidence setups," or any other rationalization:

1. **Maximum risk per trade:** 1% of account balance
2. **Maximum daily loss:** 3% of account balance (after 3% drawdown, trading is stopped for the day)
3. **Maximum concurrent positions:** 2 (in the same direction = 1, opposite directions = never)
4. **Minimum Risk-Reward before entering:** 1:2 (if SL placement gives less than 1:2 to TP1, the trade is skipped)
5. **No averaging down:** Adding to losing positions is prohibited
6. **No SL movement against position:** Once SL is set, it is only moved to breakeven or partial profit, never moved further against the position

## 23.2 Position Sizing — XAUUSD Calculation

Formula:
```
Dollar Risk = Account Balance × Risk Percentage
Lot Size = Dollar Risk ÷ (SL in Pips × Pip Value per Lot)
```

**XAUUSD Pip Value Reference:**
- 1 Standard Lot XAUUSD = $10 per pip (where 1 pip = $0.10 move in Gold = 1 point)
- Note: In XAUUSD, "1 pip" = $0.01 price change by some brokers, $0.10 by others. Confirm with broker.
- Standard convention used here: 1 pip XAUUSD = $0.10 price movement. $1.00 price move = 10 pips.

**Example Calculation:**
- Account: $10,000
- Risk: 1% = $100
- SL: 13 pips ($1.30 move in Gold price)
- Pip value per lot: $10
- Lot Size = $100 ÷ (13 × $10) = $100 ÷ $130 = 0.77 lots
- Round down to 0.70 lots (conservative)

**XAUUSD Lot Size Quick Reference:**

| Account | Risk 1% | SL 10 pips | SL 20 pips | SL 30 pips |
|---|---|---|---|---|
| $1,000 | $10 | 0.10 lots | 0.05 lots | 0.03 lots |
| $5,000 | $50 | 0.50 lots | 0.25 lots | 0.17 lots |
| $10,000 | $100 | 1.00 lots | 0.50 lots | 0.33 lots |
| $25,000 | $250 | 2.50 lots | 1.25 lots | 0.83 lots |
| $50,000 | $500 | 5.00 lots | 2.50 lots | 1.67 lots |

## 23.3 Stop-Loss Placement — XAUUSD Standard

**Bullish trade:** SL is placed 2–5 pips below the sweep low (the absolute low of the sweep candle's wick).

**Bearish trade:** SL is placed 2–5 pips above the sweep high.

**Why 2–5 pip buffer specifically:**
- Gold frequently wicks 2–4 pips past the sweep low/high before reversing
- A buffer smaller than 2 pips will be hit by normal spread during volatile periods
- A buffer larger than 10 pips moves RR below acceptable levels for most setups

**If the SL placement results in RR below 1:2, the trade is skipped.**

## 23.4 Take-Profit Management

**Two-Part TP System:**

**TP1 (50% of position):** First internal liquidity target
- In XAUUSD: typically 15–30 pips from entry on M5/M15 setups
- Must be a logical ICT target (EQH/EQL, previous session high/low, minor BSL/SSL)
- After TP1 hit: Move SL to breakeven + 2 pips (protect profit)

**TP2 (remaining 50% of position):** External liquidity target
- In XAUUSD: PDH/PDL, session high/low, major swing high/low
- Typically 30–80+ pips from entry on M5/M15 setups
- Do not close early "to protect profit" — the setup's logic defined this target before entry

**Partial Profit Scaling (advanced):**
- 25% at TP1 (1:1 RR)
- 25% at TP1.5 (1:1.5 RR)
- 50% at TP2 (external liquidity)
- SL moved to breakeven after first partial close

## 23.5 Daily and Weekly Trade Limits

**Daily:**
- Maximum trades per day: 3
- After 2 consecutive stop-losses: No more trading that session (step away, review)
- After daily loss limit hit (3%): Session terminated

**Weekly:**
- After 5% account drawdown in a week: Reduce position size by 50% for the next week
- After 10% account drawdown in any period: Full stop, review all trades in journal

## 23.6 Trade Journal Requirements

Every trade is recorded with:
1. Date, time, session
2. Setup type (Sweep + FVG, OTE, Breaker, Silver Bullet, etc.)
3. HTF bias at time of trade
4. Screenshot before entry (annotated: liquidity swept, FVG marked, entry zone marked)
5. Screenshot after outcome
6. Result: Win/Loss, dollar amount, RR achieved
7. Notes: What went right, what went wrong, what was the lesson

**Minimum journal frequency:** 100 trades before evaluating the system's performance.

---

# 24. XAUUSD-SPECIFIC CHARACTERISTICS

## 24.1 XAUUSD vs. Major Forex Pairs — Key Differences

| Characteristic | XAUUSD | EUR/USD |
|---|---|---|
| **Daily Range (ADR)** | $15–$50+ | 60–130 pips |
| **Sweep Magnitude** | 10–30 pips beyond level | 3–8 pips beyond level |
| **Spread** | 2–6 pips (varies by broker) | 0.5–1.5 pips |
| **Session volatility** | Very high at London/NY | Moderate |
| **News sensitivity** | Extreme — Fed, DXY, geopolitics | High — Economic data |
| **Correlation** | Inverse to DXY, positive to VIX | Inverse to DXY |
| **Round number liquidity** | Very dense ($2,300, $2,350, $2,400) | Moderate |
| **False sweep rate** | Higher than forex | Lower |

## 24.2 Gold's Relationship with DXY (US Dollar Index)

**Core relationship:** XAUUSD and DXY are **inversely correlated** approximately 70–80% of the time.

- DXY strengthening = Gold weakening (bearish bias for Gold)
- DXY weakening = Gold strengthening (bullish bias for Gold)

**Application:**
- Before determining daily bias, check DXY direction
- If DXY is at a HTF BSL (likely to get swept and drop) → Gold likely bullish
- If DXY is at a HTF SSL (likely to get swept and rally) → Gold likely bearish
- DXY and Gold both at major liquidity zones simultaneously = highest probability setup day

## 24.3 Gold and Risk Sentiment (VIX Correlation)

Gold is a "risk-off" asset in most macro regimes:
- VIX rising (equity fear increasing) → Gold typically bullish
- VIX falling (equity markets calm) → Gold may consolidate or pull back

**However:** This is a macro background context, not an entry trigger. ICT entries are based on price action, not macro alone.

## 24.4 XAUUSD Psychological Price Levels — Liquidity Concentrations

These round numbers are where retail stop-losses cluster most densely. They are **primary liquidity targets**, not support/resistance:

| Level | Significance |
|---|---|
| $2,000 | Major psychological (first time Gold hit $2k) |
| $2,100 | Previous ATH zone |
| $2,200 | Mid-term resistance turned support |
| $2,300 | High-density current cycle level |
| $2,350 | Mid-level liquidity |
| $2,400 | Recent ATH zone (as of 2024) |
| $2,500 | Current major BSL (2024–2025) |
| $3,000 | Multi-year target, extremely dense BSL pool |

**Rule:** When Gold approaches any of these levels, do NOT assume bounce or rejection. Assume sweep. Wait for sweep + displacement before trading.

## 24.5 Gold's Unique Session Behavior

**Asian Session:** Range 20–50 pips typically. Establishes the accumulation high/low. The Asian session high and low are the primary Judas Swing targets.

**London Open (02:00–05:00 AM NY):** Most important for Gold. The Judas Swing executes here. Gold frequently takes out the Asian high or low in the first 30–60 minutes of London before reversing.

**NY AM (08:30–12:00 NY):** Maximum daily volatility. US data at 08:30 (NFP on first Friday of month, CPI monthly) creates 50–150 pip spikes. The true daily direction is often established by 10:00 AM NY.

**NY PM (12:00–17:00 NY):** Slower, lower volume. Consolidation or continuation. Silver Bullet window at 13:30–15:00.

## 24.6 High-Impact News — XAUUSD Trading Protocol

**Events that significantly impact XAUUSD:**

| Event | Impact | ICT Rule |
|---|---|---|
| NFP (Non-Farm Payrolls) | Extreme | No new entries 15 min before; trade only after 08:50 Macro |
| CPI / PPI | Very High | Same as NFP |
| FOMC Decision | Extreme | No entries 30 min before or during; wait for volatility to settle |
| Fed Chair Speech | High | Monitor, wait for sweep + displacement after |
| Geopolitical Events | Unpredictable | Reduce position size, widen SL |
| DXY Major Move | High | Align Gold bias with DXY direction |

**During high-impact news, ICT structures are often violated.** Price may sweep multiple liquidity levels simultaneously, create false displacements, and spike in both directions within seconds. The mechanical rule: **If you cannot place a stop-loss that gives 1:2 RR without being hit by the initial news spike, do not trade the news.**

## 24.7 ADR (Average Daily Range) of XAUUSD

Average Daily Range for XAUUSD (approximate, varies by market conditions):
- Low volatility periods: $15–$25
- Normal periods: $25–$45
- High volatility (news heavy weeks): $45–$100+

**Application:**
- If Gold has already moved 90% of its ADR in one direction, do not enter in that direction — the daily range is likely exhausted
- Use ADR to set realistic TP targets: a $40 ADR day is unlikely to produce a single $50+ directional run unless there is extraordinary catalyst
- ADR helps validate if a setup's TP is realistic given the day's likely range

---

# 25. CASE STUDIES — XAUUSD

## 25.1 Winning Trade — Bullish Setup (Detailed)

**Date context:** NY Session, Wednesday. Bullish bias established.

**HTF Context:**
- D1: Uptrend (HH at $2,400, HL at $2,345, new HH in progress)
- D1: Gold at discount (current price $2,362, 50% of dealing range = $2,372)
- H4: Bullish structure, last H4 OB at $2,355–$2,360 (unmitigated)
- Weekly: PWL at $2,340, PWH at $2,410 = targeting PWH as weekly draw

**Session Preparation (pre-market):**
- PDH: $2,388 (BSL target for the day)
- PDL: $2,349 (SSL below, potential sweep target)
- Asian session range: $2,359 (high) – $2,352 (low)
- SSL pool: Equal lows at $2,352 (Asian session low matching a previous H1 low)

**London Open (02:00–04:00 AM NY Time):**
- 02:45 AM: Gold drops from $2,359 to $2,348 — sweeps Asian session low $2,352 and PDL-adjacent SSL $2,349
- The wick reaches $2,347 (3 pips below PDL)
- 02:47 AM: Bullish displacement begins on M5 — large body candle $2,348 → $2,360 (+12 pips)
- FVG formed on M5: Candle 1 High = $2,352, Candle 3 Low = $2,357 → FVG zone $2,352–$2,357
- 02:48 AM: M5 CHoCH confirmed — price closes above most recent M5 LH at $2,358

**Entry Calculation:**
- OTE: Fib from $2,347 (A) to $2,363 (B, displacement high). Range = $16
- 61.8% = $2,363 − ($16 × 0.618) = $2,363 − $9.89 = $2,353.11
- 79% = $2,363 − ($16 × 0.79) = $2,363 − $12.64 = $2,350.36
- OTE zone: $2,350–$2,353
- FVG zone: $2,352–$2,357
- **Confluence zone: $2,352–$2,353** (OTE + FVG overlap)
- Limit buy: $2,352.50

**Stop-Loss:**
- Sweep low: $2,347.00
- SL: $2,344.50 (2.5 pips below sweep) = $8 risk = 80 pips

**Take-Profit:**
- TP1: $2,368 (previous M15 high, internal BSL) = $15.50 = 155 pips → RR 1:1.9
- TP2: $2,388 (PDH = BSL target for the day) = $35.50 = 355 pips → RR 1:4.4

**Execution:**
- 02:51 AM: Gold pulls back, limit order fills at $2,352.50
- 03:20 AM: TP1 hit at $2,368 → 50% position closed, SL moved to $2,351 (BE+)
- 09:45 AM (NY AM): TP2 hit at $2,388 → remaining 50% closed

**Result:** Full RR = 1:4.4 on 50% position, 1:1.9 on other 50% = blended RR ~1:3.2

**Why this trade worked:**
- All 4 HTF conditions met (uptrend, discount, bullish bias, unmitigated H4 OB nearby)
- SSL swept at PDL level (institutional significance)
- Displacement was strong (12 pip body on M5)
- FVG + OTE confluence for entry
- Kill Zone timing (London open)
- Risk defined precisely, SL below sweep

---

## 25.2 Winning Trade — Bearish Setup (Detailed)

**Context:** NY AM session, Thursday. Bearish bias.

**HTF Context:**
- D1: Downtrend established (LH at $2,440, LL at $2,360, LH forming at $2,415)
- D1: Gold at premium zone ($2,405, above 50% of dealing range $2,400)
- H4: Last H4 bearish OB at $2,410–$2,418 (unmitigated)

**Session Preparation:**
- PDH: $2,418 (BSL = primary sweep target for today's manipulation phase)
- PDL: $2,390 (SSL = draw target for today's distribution)
- Asian session: Range $2,402–$2,412

**NY Open (08:30–10:00 AM NY):**
- 08:30 AM: CPI release — Gold spikes to $2,419, sweeping PDH $2,418 and Asian session high $2,412
- Sweep: Wick reaches $2,421, closes at $2,412
- 08:34 AM: Bearish displacement — M5 candle drops from $2,416 to $2,403, FVG $2,409–$2,413 (bearish FVG)
- 08:35 AM: M5 CHoCH confirmed (closes below most recent M5 HL at $2,407)

**Entry:**
- Limit sell at FVG 50%: ($2,409 + $2,413) / 2 = $2,411
- SL: $2,423 (2 pips above sweep high $2,421) = $12 risk
- TP1: $2,397 (internal SSL — previous M15 low) = $14 → RR 1:1.2
- TP2: $2,378 (PWL / major SSL cluster) = $33 → RR 1:2.75

**Execution:**
- 08:38 AM: Retracement to $2,411 — limit sell fills
- 09:10 AM: TP1 hit at $2,397 → 50% closed, SL moved to $2,413 (BE-)
- 11:30 AM: TP2 hit at $2,378 → remaining 50% closed

**Result:** Blended RR ~1:2.0

---

## 25.3 Losing Trade — Analyzing the Error

**Scenario: Trading an OB without displacement**

**Setup:**
- H4: Uptrend
- M15: Previous bearish candle at $2,310–$2,314 (appeared to be a bullish OB)
- Entry: Long at $2,311, SL $2,307, TP $2,330

**What happened:**
- Price returned to $2,311, filled the long limit
- No prior displacement from this OB — the OB formed without a sweep
- Price continued grinding lower to $2,304, stopped out at $2,307
- After the stop-out, Gold actually swept $2,301 (the real SSL), then displaced to $2,330

**Root cause:**
- The "OB" at $2,310–$2,314 had no prior sweep
- The move from it was gradual, not displacement
- The actual setup was the sweep at $2,301 + displacement that followed
- Entry was taken on an invalid OB — skipping Checklist Step: "Was there a prior sweep?"

**Correction rule:** Always verify that the OB was preceded by a liquidity sweep. If the candle forming the "OB" occurred without a sweep, skip the trade regardless of how the zone looks.

---

## 25.4 Losing Trade — Trading Against HTF Bias

**Scenario: LTF OB against H4 bearish bias**

**Setup:**
- H4: Bearish structure, price in premium zone
- M15: A bullish OB visible at $2,380–$2,384 (formed with M15 displacement)
- Entry: Long at $2,381 based on M15 bullish OB
- SL: $2,377, TP: $2,398

**What happened:**
- Price briefly touched $2,381, appeared to hold
- But H4 had an unmitigated bearish OB at $2,390–$2,396 directly above
- Price rallied to $2,387, hit the H4 bearish OB, rejected hard
- Gold dropped through $2,381, hit SL at $2,377

**Root cause:**
- The M15 bullish OB was valid in isolation (had prior sweep, displacement, FVG)
- But H4 bearish OB directly above $2,390 prevented price from reaching the TP
- The H4 context was not fully checked before entry

**Correction rule:** Before entering any LTF OB, identify all HTF PD arrays between entry and TP. If any HTF PD array opposes the trade direction and sits between entry and TP, the trade is skipped or TP is moved to before that HTF level.

---

# 26. PRE-TRADE CHECKLIST

This checklist must be completed in sequence before any XAUUSD trade is executed. No trade is taken unless every mandatory item is confirmed.

---

## LEVEL 1 — MACRO CONTEXT (Daily preparation, done once per session)

- [ ] **Daily bias identified:** Is D1 structure bullish or bearish? ____________
- [ ] **DXY direction checked:** DXY bullish = Gold bearish, DXY bearish = Gold bullish
- [ ] **PDH and PDL marked** on chart
- [ ] **PWH and PWL marked** on chart
- [ ] **Significant HTF liquidity pools identified** (EQH, EQL on H4/D1)
- [ ] **High-impact news scheduled today?** If yes, note time and avoid trading 15 min before
- [ ] **Premium or Discount on D1?** Current price position: ____________
- [ ] **Kill Zone active?** (London 02:00–05:00 AM / NY 07:00–11:00 AM NY Time)

---

## LEVEL 2 — SETUP IDENTIFICATION (For each potential trade)

- [ ] **Liquidity pool identified:** What pool is being targeted? BSL at $ _____ or SSL at $ _____
- [ ] **Sweep occurred?** Yes / No
  - If No → **DO NOT PROCEED. Wait.**
  - If Yes → Document: Sweep low/high at $ _____, time _____
- [ ] **Displacement followed?** Yes / No
  - If No → **DO NOT PROCEED. Wait.**
  - If Yes → Candle size: _____ pips, FVG created: Yes / No
- [ ] **FVG formed?** FVG zone: $ _____ to $ _____
- [ ] **MSS/CHoCH on M5?** Yes / No. Level broken: $ _____
- [ ] **Setup aligns with D1/H4 bias?** Yes / No
  - If No → **Skip. Do not rationalize.**
- [ ] **Discount (for longs) or Premium (for shorts)?** Confirmed: Yes / No
- [ ] **Kill Zone timing?** Setup occurred during: London / NY AM / NY PM / Macro time

---

## LEVEL 3 — TRADE PARAMETERS (Before order entry)

- [ ] **Entry price:** $ _____
- [ ] **SL price:** $ _____ (must be below sweep low for longs, above sweep high for shorts)
- [ ] **SL distance in pips:** _____ pips
- [ ] **TP1 price:** $ _____ (internal liquidity) — RR: _____
- [ ] **TP2 price:** $ _____ (external liquidity) — RR: _____
- [ ] **Minimum RR 1:2 confirmed?** Yes / No. If No → **Skip trade.**
- [ ] **Position size calculated:** _____ lots (based on 1% risk rule)
- [ ] **Any HTF PD array between entry and TP that opposes trade?** Yes / No. If Yes → Adjust TP or skip.
- [ ] **Daily loss limit not yet hit?** Yes / No. If limit already hit → **No trade today.**
- [ ] **Less than 3 trades already taken today?** Yes / No. If 3 trades already done → **No trade today.**

---

## LEVEL 4 — POST-TRADE MANAGEMENT RULES (Set before entry, do not modify)

- [ ] **SL is set and will NOT be moved further against the trade**
- [ ] **TP1 is set — close 50% when hit**
- [ ] **SL moved to breakeven after TP1 hit**
- [ ] **TP2 is set — close remaining 50% when hit**
- [ ] **Journal screenshot taken before entry**

---

# 27. COMMON ERRORS — MECHANICAL BREAKDOWN

## 27.1 Error: Entering Before the Sweep

**Description:** Price is approaching a liquidity pool. The trader enters before the sweep occurs, anticipating the bounce.

**Why it fails:** Smart Money must sweep the liquidity to collect the orders needed to power the actual move. If you enter before the sweep, you become part of the liquidity that will be swept.

**Mechanical fix:** Entry is only placed after: (1) Sweep confirmed, (2) Displacement confirmed, (3) MSS confirmed. No entry before all three.

---

## 27.2 Error: No Displacement After Sweep

**Description:** Sweep occurs (wick below SSL), but the candles following are small, gradual, indecisive. The trader enters anyway.

**Why it fails:** Without displacement, institutional entry has not been confirmed. The sweep may have only collected partial liquidity. A second, deeper sweep frequently follows.

**Mechanical fix:** Displacement requirement = minimum candle size for the timeframe (see Section 4.4). If displacement criterion is not met → no trade.

---

## 27.3 Error: Entering at Every FVG

**Description:** Trader marks all FVGs and places limit orders at all of them, regardless of context.

**Why it fails:** FVGs without displacement context are just gaps. Not all gaps are institutional imbalances. Many will be fully traded through with no reaction.

**Mechanical fix:** FVG is only traded if: preceded by a sweep, formed by displacement, within a Kill Zone, aligns with HTF bias.

---

## 27.4 Error: Wide SL to "Give Room"

**Description:** Trader sets SL far below the sweep low "just in case" Gold goes deeper.

**Why it fails:** If the SL is set wider than the sweep extreme, the risk per trade increases without a corresponding increase in RR. The math no longer supports positive expectancy.

**Mechanical fix:** SL = 2–5 pips beyond sweep extreme only. If this results in a position size too small to be practical, it means the setup's SL is too wide relative to account size. Use a smaller lot or skip the trade.

---

## 27.5 Error: Moving TP Prematurely

**Description:** Trade is running in profit toward TP2. Trader closes early because they fear a reversal.

**Why it fails:** Early TP closure systematically reduces the average RR of the system below what was planned. A system planned at 1:2.5 average RR performs at 1:1.2 due to premature exits. This destroys edge.

**Mechanical fix:** TP1 and TP2 are set before entry. They are not changed unless the setup's structure is violated (e.g., price makes a bearish CHoCH on M15 before reaching TP2 in a long trade). Structural violation = only acceptable reason for early exit.

---

## 27.6 Error: Trading During Asia Session

**Description:** A sweep occurs during the Asian session (00:00–06:00 NY). Trader enters based on the sweep.

**Why it fails:** Asian session in XAUUSD has the lowest volume. Sweeps during Asia are frequently false — the real sweep occurs later in London. The "displacement" in Asia is often not institutional.

**Mechanical fix:** Asian session setups require much higher confluence to be valid. Standard rule: do not trade Asian session in Gold. Exception: Asia moves more than 80–100 pips with a clear sweep of a weekly level.

---

## 27.7 Error: Revenge Trading

**Description:** After a stop-loss, the trader immediately enters a new trade to "recover" the loss.

**Why it fails:** Revenge trades are made without proper setup identification. They are emotional decisions, not mechanical ones. They result in further losses.

**Mechanical fix:** After any stop-loss, a mandatory minimum 15-minute waiting period before looking at any new setup. After 2 consecutive stop-losses in a session: session is terminated, platform is closed.

---

## 27.8 Error: Choosing OB Over Sweep Logic

**Description:** Trader marks an OB on a previous session. A new session begins. Price approaches the OB from above (for a bullish OB). Trader enters long immediately as price touches the OB, without waiting for a sweep of the SSL below the OB.

**Why it fails:** The proper sequence is: liquidity sweep → displacement → OB/FVG entry. If price approaches an OB from above and there has been no sweep, the SSL below the OB is still intact. Smart Money may sweep that SSL first before bouncing from the OB.

**Mechanical fix:** Even at an OB, check whether there is SSL between current price and the OB distal edge. If yes, wait for that SSL to be swept first.

---

# 28. GLOSSARY

| Term | Full Definition |
|---|---|
| **AMD** | Accumulation-Manipulation-Distribution — the three phases of price delivery per ICT |
| **ADR** | Average Daily Range — the average high-low range for XAUUSD in a given period |
| **BE** | Breakeven — moving SL to entry price, eliminating dollar risk |
| **BOS** | Break of Structure — price closes beyond a previous structural high (bullish BOS) or low (bearish BOS) |
| **BPR** | Balanced Price Range — overlapping bullish and bearish FVGs creating equilibrium zone |
| **BSL** | Buy-Side Liquidity — stop-losses and pending orders clustered above highs |
| **CHoCH** | Change of Character — first structural break opposite to prevailing trend, signaling potential reversal |
| **DXY** | US Dollar Index — inversely correlated to XAUUSD approximately 70–80% of the time |
| **EQH** | Equal Highs — two or more swing highs at approximately the same price level = BSL pool |
| **EQL** | Equal Lows — two or more swing lows at approximately the same price level = SSL pool |
| **FVG** | Fair Value Gap — three-candle imbalance where Candle 1 and Candle 3 do not overlap |
| **H4** | 4-Hour Timeframe |
| **HH** | Higher High — structural high above the previous swing high in an uptrend |
| **HL** | Higher Low — structural low above the previous swing low in an uptrend |
| **HTF** | Higher Timeframe — a timeframe above the one being used for entry |
| **IDM** | Inducement — small false sweep designed to trap retail before the real sweep |
| **IFVG** | Inversion Fair Value Gap — a FVG that has been fully filled and now acts with reversed polarity |
| **IPDA** | Interbank Price Delivery Algorithm — the algorithmic system that delivers price in interbank markets per ICT |
| **ITH/ITL** | Intermediate-Term High / Low — swing formed on H1–H4 |
| **Kill Zone** | Specific high-volume time window during which ICT setups carry the highest reliability |
| **LH** | Lower High — structural high below the previous swing high in a downtrend |
| **LL** | Lower Low — structural low below the previous swing low in a downtrend |
| **LTF** | Lower Timeframe — a timeframe below the one being used for context |
| **LTH/LTL** | Long-Term High / Low — swing formed on D1–W1 |
| **Macro** | ICT Macro — specific 20–30 minute precision windows within Kill Zones for algorithmic price delivery |
| **MSS** | Market Structure Shift — CHoCH accompanied by displacement, used as LTF entry trigger |
| **MTF** | Mid-Timeframe — typically M15/H1 in the XAUUSD framework |
| **OB** | Order Block — last opposing candle before a significant displacement; institutional order zone |
| **OTE** | Optimal Trade Entry — 61.8%–79% Fibonacci retracement of a displacement leg |
| **PDH** | Previous Day's High — primary daily BSL target |
| **PDL** | Previous Day's Low — primary daily SSL target |
| **POI** | Point of Interest — a specific price zone (OB, FVG, Breaker) where price is expected to react |
| **PO3** | Power of Three — synonym for AMD model |
| **Premium** | Above 50% of dealing range — zone for short entries |
| **Discount** | Below 50% of dealing range — zone for long entries |
| **PWH** | Previous Week's High — weekly BSL target |
| **PWL** | Previous Week's Low — weekly SSL target |
| **RR** | Risk-Reward Ratio — the ratio of profit target to stop-loss distance |
| **SL** | Stop-Loss — the price at which the trade is exited at a loss |
| **SMC** | Smart Money Concepts — the broader framework of ICT concepts |
| **SSL** | Sell-Side Liquidity — stop-losses and pending orders clustered below lows |
| **STH/STL** | Short-Term High / Low — swing formed on M1–M15 |
| **TP** | Take-Profit — the price at which the trade is exited at a profit |
| **XAUUSD** | Spot Gold / US Dollar — the instrument this entire document is focused on |

---

# APPENDIX: QUICK REFERENCE — TRADE DECISION TREE

```
START: Is there an active Kill Zone (London 02:00–05:00 or NY 07:00–11:00 NY Time)?
├─ NO → Wait. Do not trade.
└─ YES
    ↓
    Has price swept a significant liquidity pool (SSL or BSL)?
    ├─ NO → Wait. Do not trade.
    └─ YES — sweep confirmed at $ ___
        ↓
        Was there displacement (large body candles, FVG formed) after the sweep?
        ├─ NO → Wait. Could be inducement. Do not trade.
        └─ YES — FVG at $ ___ to $ ___
            ↓
            Has MSS/CHoCH occurred on M5 after displacement?
            ├─ NO → Wait for MSS.
            └─ YES — MSS confirmed
                ↓
                Does this align with D1/H4 HTF bias?
                ├─ NO → Skip. Do not rationalize.
                └─ YES
                    ↓
                    Is entry zone in Discount (long) or Premium (short) on D1?
                    ├─ NO (entering in wrong zone) → Skip.
                    └─ YES
                        ↓
                        Is RR minimum 1:2 from FVG/OTE entry to TP1?
                        ├─ NO → Skip or adjust SL (only if sweep extreme allows).
                        └─ YES
                            ↓
                            ENTER TRADE:
                            Limit order at FVG 50% or OTE zone
                            SL: 2–5 pips beyond sweep extreme
                            TP1: Internal liquidity (50% close)
                            TP2: External liquidity (50% close)
                            Position size: 1% risk rule
                            ↓
                            POST-ENTRY: Do not touch SL until TP1 hit.
                            After TP1: Move SL to breakeven.
                            After TP2: Trade complete. Journal entry made.
```

---

*This document is based on ICT (Inner Circle Trader) methodology developed by Michael J. Huddleston, cross-referenced with published SMC research, community backtesting data, and XAUUSD-specific market behavior analysis. All examples use illustrative price levels representative of XAUUSD market conditions. No section of this document constitutes financial advice. All trading involves risk of capital loss.*
