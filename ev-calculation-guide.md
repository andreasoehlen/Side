# Expected Value (EV) Calculation Guide

## Assumptions
- **RTP (Return to Player)**: 94% for both casino and sports
- This means house edge is 6%

## EV Calculation Formulas

### 1. Casino Deposit Bonus
**Formula**: `EV = (Deposit + Bonus) × RTP - Deposit`

**Example**: 100% bonus up to 500kr with 10x wagering
- Deposit: 500kr
- Bonus: 500kr
- Total to wager: (500 + 500) × 10 = 10,000kr
- Expected return: 10,000 × 0.94 = 9,400kr
- **EV = 9,400 - 500 = +8,900kr** ❌ WRONG

**Correct Formula for Wagering Requirements**:
`EV = Bonus × RTP^(wagering_multiplier) - 0`

**Corrected Example**:
- Bonus: 500kr
- Wagering: 10x on (deposit + bonus) = need to wager 10,000kr
- But you're playing through: (500 + 500) with 10x = total 10,000kr played
- Money at risk: Your deposit (500kr) + bonus (500kr) played through with 94% RTP
- Expected value after wagering: 1,000 × 0.94^10 ≈ 1,000 × 0.54 = 540kr
- Subtract your deposit: 540 - 500 = **+40kr EV**

**Simplified for high wagering**:
`EV ≈ (Deposit + Bonus) - (Deposit + Bonus) × (1 - RTP) × wagering_multiplier - Deposit`

### 2. Free Spins
**Formula**: `EV = (Number of Spins × Spin Value) × RTP - Cost`

**Example**: 50 free spins at 2kr per spin, no deposit required
- Total value: 50 × 2kr = 100kr
- Expected return: 100 × 0.94 = 94kr
- Cost: 0kr
- **EV = +94kr**

**With wagering**: If 94kr must be wagered 10x
- After wagering: 94 × 0.94^10 ≈ 94 × 0.54 = 51kr
- **EV = +51kr**

### 3. Freebet (Sports)
**Formula**: `EV = Freebet Amount × (Average Odds - 1) / Average Odds × RTP - 0`

**Simplified**: For a freebet, you get to keep only the profit (not stake returned)
- **Conservative estimate**: `EV ≈ Freebet × 0.70` (assumes ~2.0 odds)
- **Aggressive estimate**: `EV ≈ Freebet × 0.80` (assumes higher odds arbitrage)

**Example**: 200kr freebet
- **EV ≈ 140-160kr**

### 4. Cashback Offers
**Formula**: `EV = Expected Loss × Cashback %`

**Example**: 10% cashback on losses up to 500kr
- If you lose 500kr: Cashback = 50kr
- **EV = +50kr** (on a losing scenario)

## Volatility Assessment

### Standard Deviation for Slots
`SD = Bet × √(Variance Factor)`
- For high variance slots: Use factor of 2.0-3.0
- For low variance slots: Use factor of 0.8-1.2

### 5% Worst Case (5th Percentile)
**Formula**: `Worst Case = EV - (1.645 × SD)`

**Example**: 500kr bonus, EV = +40kr, SD = 300kr
- 5% worst case = 40 - (1.645 × 300) = 40 - 493 = **-453kr**
- This means 5% chance you lose more than 453kr

### Simplified Worst Case for Bonuses
For practical purposes with high wagering:
`5% Worst Case ≈ -(Deposit + Bonus) × 0.5`

**Example**: 500kr deposit + 500kr bonus
- **5% Worst Case ≈ -500kr** (you could lose most of your deposit)

## Risk Rating System

| EV/Risk Ratio | Rating | Action |
|---------------|--------|--------|
| > 0.5 | ⭐⭐⭐⭐⭐ Excellent | Take immediately |
| 0.2 - 0.5 | ⭐⭐⭐⭐ Good | Take if time permits |
| 0.1 - 0.2 | ⭐⭐⭐ Moderate | Consider carefully |
| 0.05 - 0.1 | ⭐⭐ Low | Skip unless low effort |
| < 0.05 | ⭐ Poor | Skip |

**EV/Risk Ratio** = `Absolute(EV) / Amount at Risk`

## Practical Examples

### Example 1: 100% Deposit Bonus
- **Offer**: Deposit 500kr, get 500kr bonus, wager 10x
- **Cost**: 500kr deposit
- **EV**: ~40kr (after 10x wagering at 94% RTP)
- **5% Worst Case**: -450kr
- **Ratio**: 40/500 = 0.08 (⭐⭐ Low priority)

### Example 2: No Deposit Free Spins
- **Offer**: 50 spins × 1kr = 50kr, wager 30x
- **Cost**: 0kr
- **Value after spins**: 50 × 0.94 = 47kr
- **Value after wagering**: 47 × 0.94^(~5 cycles) ≈ 35kr
- **EV**: +35kr
- **5% Worst Case**: 0kr (no deposit risk)
- **Ratio**: Infinite (⭐⭐⭐⭐⭐ Take always!)

### Example 3: 200kr Freebet
- **Offer**: 200kr freebet (stake not returned)
- **Cost**: 0kr
- **EV**: ~140-160kr (70-80% of freebet value)
- **5% Worst Case**: 0kr
- **Ratio**: Infinite (⭐⭐⭐⭐⭐ Take always!)

## Notes
- Always read terms & conditions for max bet limits, game restrictions
- Some bonuses exclude certain games (table games, high RTP slots)
- Time limits can reduce effective value
- Multiple bonuses running simultaneously can complicate bankroll management
