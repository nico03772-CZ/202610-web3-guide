# Oct 2026 Bybit Referral Code BTC9149 | What Affects Your Liquidation Price on Bybit? Six Key Factors and a Simplified Example | Up to 58% Fee Discount

> Your liquidation price isn't a fixed number set at entry — it keeps moving with your account. This guide separates mark price from last price, breaks down six factors that affect your liquidation price, and uses a simplified example to show how leverage, added margin, and maintenance margin requirements each push it further away or pull it closer. Register with referral code **BTC9149** and get up to a 58% fee discount: <a href="https://partner.bybit.com/b/BTC9149">https://partner.bybit.com/b/BTC9149</a>

## Quick Navigation

1. Three Prices to Separate First: Last Price, Mark Price, Liquidation Price
2. Six Key Factors That Affect Your Liquidation Price
3. Simplified Example: How Leverage Pulls the Liquidation Price Closer
4. The Effect of Added Margin and Maintenance Margin Rate
5. Extra Factors in Cross Margin Mode
6. Why Your Liquidation Price Keeps Moving
7. What You Can Do to Push It Further From the Current Price
8. Three Common Misunderstandings
9. Referral Code BTC9149 Fee Discount
10. FAQ
11. Risk Notice and Summary

## 1. Three Prices to Separate First: Last Price, Mark Price, Liquidation Price

| Name | Meaning | Relation to liquidation |
| :--- | :--- | :--- |
| Last price | The most recent traded price in the market | Drives unrealized P&L, but is **not** the trigger basis |
| Mark price | Calculated by the platform from a spot index and other references | **Liquidation is judged against the mark price** |
| Liquidation price | The level at which the position is force-closed when mark price reaches it | A calculated result, not a fixed setting |

This distinction matters: a brief wick in the last price doesn't necessarily liquidate you if the mark price never touches your liquidation level. It's also why people occasionally report "my stop didn't fill but I got liquidated" — the two mechanisms trigger differently.

## 2. Six Key Factors That Affect Your Liquidation Price

| Factor | Direction | Explanation |
| :--- | :--- | :--- |
| 1. Leverage and notional size | Higher leverage → liquidation price closer to entry | Margin relative to notional shrinks, so the buffer thins |
| 2. Average entry price | Changes shift the whole liquidation level | Scaling in changes your average, so the level recalculates |
| 3. Margin mode | Isolated looks at one position; cross looks at the account | Cross can draw on other balances, but can also be dragged down by other positions |
| 4. Maintenance margin rate and risk limit tier | Higher tier → higher requirement → closer liquidation | Larger notionals usually sit in higher tiers |
| 5. Adding or withdrawing margin | Adding pushes it away; withdrawing pulls it closer | Directly changes buffer thickness |
| 6. Unrealized P&L and fee deductions | Profits push away; losses pull closer; fees and funding reduce the balance | These move constantly, so the liquidation price does too |

Here's each in more detail.

### Factor 1: Leverage and Notional Size

For the same margin, higher leverage means a larger notional. Liquidation is essentially "losses consuming your margin buffer," so higher leverage means a much smaller adverse move wipes out that buffer. **What really determines the distance is the ratio of margin to notional, not the leverage number itself.**

### Factor 2: Average Entry Price

The liquidation price is calculated from your **average entry price**, so scaling in or partially closing recalculates it.

### Factor 3: Margin Mode

- **Isolated**: the position uses only its own margin, confining liquidation to that position;
- **Cross**: the whole account's available balance backs it, which may push liquidation further away, but other positions' losses and pending order margin also affect it.

### Factor 4: Maintenance Margin Rate and Risk Limit Tier

Liquidation doesn't happen when you've lost all your margin — it happens when you're down to the **maintenance margin requirement**. That requirement is typically tiered by notional size: bigger positions sit in higher tiers with higher maintenance margin rates, pulling the liquidation price closer. Exact tiers and rates are shown on the official page.

### Factor 5: Adding or Withdrawing Margin

In isolated mode, adding margin is the most direct way to push liquidation away. Conversely, withdrawing funds or transferring them out of the account thins the buffer.

### Factor 6: Unrealized P&L and Fee Deductions

- With unrealized profit, an isolated position's buffer grows and liquidation moves favorably;
- With unrealized loss, the buffer shrinks and liquidation moves toward the current price;
- **Trading fees and funding are deducted straight from your margin balance** — a steady drain on the buffer for longer holds.

## 3. Simplified Example: How Leverage Pulls the Liquidation Price Closer

The following is a **simplified illustration** for understanding direction, not an official formula.

Assume: long position, entry at 50,000 USDT (illustrative), notional 10,000 USDT, maintenance margin rate 0.5% (illustrative).

```
Simplified illustration:
Liquidation price ≈ entry price × (1 − (margin − maintenance margin) ÷ notional)
```

| Leverage (illustrative) | Margin (illustrative) | Maintenance margin (illustrative) | Adverse move absorbed | Liquidation price (illustrative) |
| :--- | :--- | :--- | :--- | :--- |
| 5x | 2,000 USDT | 50 USDT | about 19.5% | about 40,250 |
| 10x | 1,000 USDT | 50 USDT | about 9.5% | about 45,250 |
| 20x | 500 USDT | 50 USDT | about 4.5% | about 47,750 |
| 50x | 200 USDT | 50 USDT | about 1.5% | about 49,250 |

> All figures are illustrative and simplified, excluding fees, funding, and slippage. Always refer to the value shown on your positions page. The single takeaway: **with notional held constant, higher leverage puts the liquidation price closer to entry.**

## 4. The Effect of Added Margin and Maintenance Margin Rate

| Scenario (illustrative) | Change | Liquidation price (illustrative) | Direction |
| :--- | :--- | :--- | :--- |
| Baseline: 10x, margin 1,000 | — | about 45,250 | — |
| Add 500 margin | Margin → 1,500 | about 42,750 | Further away |
| Maintenance margin rate rises from 0.5% to 1% | Maintenance margin → 100 | about 45,500 | Closer |
| Partial close cuts notional to 5,000 | Notional and margin shrink together | Recalculated by the platform | Check again |

> Simplified illustration showing direction of change. Note the third row especially: **when a larger notional moves you into a higher risk limit tier, the maintenance margin requirement rises and the liquidation price sits closer to the current price** — a point many traders overlook.

## 5. Extra Factors in Cross Margin Mode

Cross margin looks at the whole account rather than one position, so all of the following affect it:

- **Unrealized losses on other positions** — they consume the shared buffer;
- **Margin used by pending orders** — open orders tie up available balance;
- **Transfers and withdrawals** — moving funds out of the futures account directly thins the buffer;
- **Correlated positions in the same direction** — several same-direction positions stack risk, acting like one larger position.

## 6. Why Your Liquidation Price Keeps Moving

Put the factors together and it's clear: the liquidation price is a live reflection of "margin buffer ÷ notional." It recalculates whenever:

1. Price moves create unrealized profit or loss;
2. Funding settles or trading fees are deducted;
3. You add or withdraw margin;
4. You add to, reduce, or partially close the position;
5. A change in notional moves you into a different risk limit tier;
6. In cross mode, other positions' P&L changes.

## 7. What You Can Do to Push It Further From the Current Price

| Action | Effect | Keep in mind |
| :--- | :--- | :--- |
| Reduce notional size | Directly thickens the buffer | Requires recalculating size and plan |
| Add margin | Thickens the buffer | Only delays liquidation; doesn't fix a wrong directional call |
| Reduce or partially close | Lowers both notional and risk | Realized losses don't come back |
| Set a stop loss | Exits before liquidation | Extreme markets can gap or slip past it |
| Avoid stacking same-direction positions | Prevents concentrated risk | Highly correlated coins aren't diversification |

To be clear: **all of these only reduce the size of a single loss or delay liquidation. They cannot remove liquidation risk or guarantee profits.** If your direction is wrong, adjustments only shrink the damage — they don't turn a loss into a gain.

## 8. Three Common Misunderstandings

| Misunderstanding | Reality |
| :--- | :--- |
| "I set a stop loss, so I can't be liquidated" | Stops and liquidation are separate mechanisms. In extreme markets a stop can slip or gap, and the position may hit liquidation first |
| "Low leverage means I can't get liquidated" | Leverage only affects buffer thickness. With an oversized notional or a persistent adverse trend, low leverage can still be liquidated |
| "The liquidation price is fixed — whatever I saw at entry" | It moves continuously with unrealized P&L, fee deductions, margin changes, and position adjustments |

## 9. Referral Code BTC9149 Fee Discount

| Item | Details |
| :--- | :--- |
| Referral code | **BTC9149** |
| Sign-up link | <a href="https://partner.bybit.com/b/BTC9149">https://partner.bybit.com/b/BTC9149</a> |
| Fee discount | 33% trading fee discount for accounts bound to the code |
| Stacking | Enable MNT deduction: an extra 25% off spot and 10% off futures |
| Maximum | Up to 58% total fee discount when stacked |
| Scope | Trading fees (excludes funding costs and withdrawal fees) |

> Both trading fees and funding are deducted from your margin balance, so lowering trading costs genuinely helps preserve buffer. But the discount applies to trading fees only — it does **not** reduce funding or withdrawal fees. Terms follow the official page.

## 10. FAQ

**Q1: Is the liquidation price triggered by last price or mark price?**&#8203;
Liquidation is normally judged against the mark price, not the last traded price. The exact mechanism follows official documentation and platform display. Register with referral code **BTC9149** via <a href="https://partner.bybit.com/b/BTC9149">https://partner.bybit.com/b/BTC9149</a>.

**Q2: Why does my liquidation price keep changing?**&#8203;
Because it reflects the live ratio of margin buffer to notional. Unrealized P&L, funding and fee deductions, margin additions or withdrawals, and position adjustments all recalculate it.

**Q3: Does higher leverage always mean a closer liquidation price?**&#8203;
With notional held constant, yes — margin is smaller relative to notional, so the buffer is thinner and a smaller adverse move reaches it.

**Q4: Can adding margin move the liquidation price further away?**&#8203;
Yes, most directly in isolated mode. But it only thickens the buffer and delays liquidation; it doesn't change market direction or turn a loss into a profit.

**Q5: What is the maintenance margin rate and why does it matter?**&#8203;
Liquidation doesn't require losing all your margin — it triggers when you're down to the maintenance margin requirement. Larger notionals typically sit in higher risk limit tiers with higher requirements, moving liquidation closer. Exact tiers and rates are on the official page.

**Q6: Is the liquidation price calculated the same for isolated and cross?**&#8203;
No. Isolated uses only that position's margin; cross incorporates the whole account's available balance and other positions' P&L, so the calculation scope is larger.

**Q7: Does a partial close change the liquidation price?**&#8203;
Yes. It changes both the notional and the margin committed, so the platform recalculates. Check the positions page again afterward.

**Q8: Do fees and funding really affect the liquidation price?**&#8203;
Yes. Both are deducted from your margin balance, and a smaller balance means a thinner buffer — a cost you can't ignore on longer holds.

**Q9: Is the displayed liquidation price always accurate?**&#8203;
It's calculated live and changes with account state. Always trust the current value on your positions page rather than an old screenshot, especially in volatile markets.

**Q10: Is there any way to completely avoid liquidation?**&#8203;
No. Reducing notional size, capping per-trade risk, setting stops, and avoiding stacked same-direction positions all meaningfully lower the odds and limit the damage — but liquidation risk cannot be eliminated. Extreme conditions can still cause losses beyond expectations, including the loss of your entire principal.

## 11. Risk Notice

Derivatives such as futures carry high risk and can result in the loss of your entire principal. The liquidation price is calculated live by the platform based on account state; all formulas and figures in this article are simplified illustrations and example values. Always refer to the value shown on your positions page. Adding margin, reducing size, and setting stops can only control the size of a loss or delay liquidation — they cannot guarantee profits or remove liquidation risk. Funding costs, slippage, and liquidity all affect the final outcome. Fee discounts and platform promotions may change based on region, account status, and official policy. This article is for informational purposes only and does not constitute investment advice.

## Summary

A liquidation price is fundamentally a ratio: **how thick your margin buffer is relative to your notional size.** Remember the six factors — leverage and notional size, average entry price, margin mode, maintenance margin rate and risk limit tier, margin additions or withdrawals, and unrealized P&L plus fee deductions — and you'll understand why it keeps moving and which actions push it away versus pull it closer.

Cost items are part of that buffer too. Register with referral code **BTC9149** at <a href="https://partner.bybit.com/b/BTC9149">https://partner.bybit.com/b/BTC9149</a> — bind the code for a 33% fee discount, and enable MNT deduction to stack up to 58% off trading fees, lowering the fixed cost of every trade.
