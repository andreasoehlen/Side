# Bonus Hunting Workflow

## Twice-Weekly Update Schedule

**Recommended Days**: Monday & Thursday (or adjust to your preference)

---

## PHASE 1: You Request Update (Monday/Thursday)

Simply message: **"Update on offers"** or similar

I will then:
1. Search all sources for current Danish casino/sports bonuses
2. Filter for offers you can take (exclude signup bonuses)
3. Calculate EV for each offer
4. Assess volatility and 5% worst case
5. Return a **prioritized checklist** with recommendations

---

## PHASE 2: I Provide Offer Checklist

You'll receive a response like this:

```markdown
## Available Offers - [Date]

### 🔥 High Priority (Take These)
- [ ] **Bet365 - 100kr Freebet**
  - Requirements: Place 100kr bet on odds >2.0
  - EV: +70kr | 5% Worst: 0kr | Risk: None ⭐⭐⭐⭐⭐
  - Estimated time: 10 min

### ✅ Medium Priority (Good Value)
- [ ] **Betano - 50 Free Spins**
  - Requirements: Deposit 100kr
  - EV: +35kr | 5% Worst: -80kr | Risk: Low ⭐⭐⭐⭐
  - Estimated time: 30 min

### ⚠️ Low Priority (Skip Unless Bored)
- [ ] **LeoVegas - 100% Bonus**
  - Requirements: Deposit 500kr, wager 15x
  - EV: +25kr | 5% Worst: -450kr | Risk: High ⭐⭐
  - Estimated time: 2 hours

### ❌ Skip
- [ ] **Expekt - Reload Bonus**
  - Requirements: Deposit 1000kr, wager 20x
  - EV: -15kr | Negative EV ❌
```

---

## PHASE 3: You Take Actions

Over the next few days, you:
1. Work through the checklist
2. Take the offers you want
3. Note any results (optional: keep rough notes)

---

## PHASE 4: You Report Back

When ready (before next update), message me with:

**Format Option 1 - Detailed**:
```
Update from last session:
- Bet365 freebet: Won 140kr
- Betano free spins: Deposited 100kr, ended with 85kr balance
- Skipped LeoVegas
```

**Format Option 2 - Simple**:
```
Update:
- Bet365: +140kr
- Betano: Deposit 100kr, balance now 85kr
- LeoVegas: No change
```

**Format Option 3 - Just site balances** (I'll calculate the rest):
```
Current balances:
Bet365: 2236kr
Expekt: 300kr
Betano: 85kr
Danske Spil: 66kr
LeoVegas: 0kr

New deposits: Betano 100kr
New withdrawals: None
```

---

## PHASE 5: I Update & Summarize

I will:
1. Update `betting-tracker.json` with new data
2. Calculate profit/loss for the session
3. Provide a summary:

```markdown
## Session Summary

**Period**: Nov 22 - Nov 25

### Performance
| Site | Starting | Ending | Change | Session P/L |
|------|----------|--------|--------|-------------|
| Bet365 | 2096kr | 2236kr | +140kr | +140kr |
| Betano | 1012kr | 85kr | -927kr | -15kr* |
| **Total** | | | | **+125kr** |

*Betano: Withdrew 100kr deposit, net -15kr after accounting

### Overall Stats
- **Total Profit (All Time)**: 5,921kr
- **Sessions Completed**: 1
- **Average Session**: +125kr
- **Best Site**: Bet365 (+5,796kr all-time)
- **Worst Site**: LeoVegas (-1,000kr all-time)

### Notes
- Excellent session, positive EV plays paid off
- Consider reducing Betano exposure if variance continues
```

---

## Quick Reference Commands

When you message me, use these phrases:

| What You Say | What I Do |
|--------------|-----------|
| "Update on offers" | Search & provide new offer checklist |
| "Report: [changes]" | Update tracker & provide summary |
| "Check [Site Name]" | Search specific site for offers |
| "What's my total profit?" | Quick stats summary |
| "Add site [Name]" | Add new betting site to tracker |

---

## Tips for Maximum Profit

1. **Prioritize no-deposit offers**: Freebets and free spins with 0kr risk
2. **Take high priority offers immediately**: Time-sensitive deals expire
3. **Track your time**: Sometimes low EV isn't worth 2 hours of play
4. **Diversify sites**: Don't put all money on one site
5. **Set stop-loss**: If 5% worst case is too high for your bankroll, skip
6. **Check emails**: Sites send exclusive offers to existing customers

---

## Files in This System

- `betting-tracker.json` - Your current balances and history
- `bonus-sources.md` - Where to find offers
- `ev-calculation-guide.md` - How EV is calculated
- `WORKFLOW.md` - This file

---

## Getting Started

You're all set! Next time you want an update, just message:

**"Update on offers for this week"**

And I'll search all sources and provide your personalized checklist! 🎰
