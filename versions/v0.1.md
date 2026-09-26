# Bungee Funded Perp Rulebook

---

## 1. Purpose

Bungee Funded Perp is designed to offer a simple, transparent evaluation and funded-trader program with clear risk limits, predictable payout rules, and market-specific controls.

Bungee offers isolated-margin perpetual contracts. Cross-margin trading is not supported.

The Bungee dashboard and internal account ledger are the authoritative source of truth for account status, balances, equity, breaches, payouts, supported markets, leverage, fees, and position limits.

---

# Part I — Evaluation Program

## 2. Evaluation Structure

Bungee Funded Perp uses a one-step evaluation.

- No time limit
- No minimum trading days
- No consistency rule
- Hard-breach model
- Profit target varies by evaluation type
- Maximum daily loss is 3% for every evaluation type
- Maximum total drawdown varies by evaluation type

Exact evaluation parameters will be displayed on the relevant evaluation plan before purchase and inside the Bungee dashboard.

## 3. Evaluation Plans

Bungee offers three one-step evaluation tracks.

### Evaluation Rules

| Rule | 1-Step Classic | 1-Step Pro | 1-Step Turbo |
| --- | ---: | ---: | ---: |
| Profit target | 10% | 12% | 9% |
| Maximum daily loss | 3% | 3% | 3% |
| Maximum drawdown | 6% static | 5% static | 3% static |
| Phases | 1 | 1 | 1 |
| Time limit | None | None | None |
| Standard reward split | 80% | 80% | 80% |

### Evaluation Pricing

For current evaluation prices and available plans, visit the [Bungee evaluation page](https://app.bungee.exchange/funded-perps#pricing).

Pricing and plan availability may change. The live checkout page and Bungee dashboard are the source of truth.

## 4. Hard Breach Policy

Bungee uses a hard-breach model.

An account may be breached if the trader:

- Reaches or exceeds the maximum daily loss limit.
- Reaches or exceeds the maximum total drawdown limit.
- Uses a prohibited trading practice.
- Violates these rules or the applicable Bungee Funded Perp Terms.

After a hard breach:

- Open positions may be force-closed.
- The account may be permanently disabled.
- The trader must purchase or begin a new evaluation to continue.
- There is no automatic forgiveness, reset, grace period, or soft breach.

Warnings may be shown as a convenience but do not change the underlying limits.

## 5. Daily Loss

Daily loss is measured using account equity and may include:

- Realized P&L
- Unrealized P&L
- Trading fees
- Funding charges
- Other applicable account charges

The maximum daily loss is 3% for Classic, Pro, and Turbo evaluations.

The daily loss measurement resets each day at:

> **00:00 UTC**

The dashboard will display the active daily loss limit and the time remaining until the next reset.

## 6. Maximum Drawdown

Bungee uses a static maximum drawdown:

- Classic: 6%
- Pro: 5%
- Turbo: 3%

The drawdown limit is measured against the account’s defined starting balance and does not trail upward with profits.

After each approved funded-account payout, including the first, the account resets to its default state under Section 25. Its original starting balance and default risk limits are restored; unpaid eligible profits remain separately claimable and do not increase the trading balance or drawdown allowance.

---

# Part II — Supported Markets and Risk Limits

## 7. Asset Listing Policy

Bungee does not automatically support every market listed on Hyperliquid or any other venue.

A market must be explicitly approved and enabled by Bungee before it can be traded.

Bungee may evaluate markets based on:

- Market liquidity
- Order-book depth
- Volatility
- Manipulation risk
- Venue constraints
- Ability to hedge or externally execute exposure
- Counterparty and operational risk
- Maximum executable size

Venue listing alone does not make an asset eligible for Bungee Funded Perp.

Bungee may add more markets over time as they pass internal risk review.

## 8. Supported Markets

For currently supported markets, fixed leverage, and maximum position limits, visit the [Bungee assets page](https://app.bungee.exchange/funded-perps/assets).

## 9. Isolated Perpetuals and Fixed Leverage

All supported markets are perpetual contracts that use isolated margin.

Margin is assigned to each position independently and is not shared automatically with other open positions. A position's margin and liquidation risk are therefore isolated from the margin assigned to other positions.

Isolated margin does not remove account-level risk controls. Realized and unrealized P&L, trading fees, and funding from every position continue to affect account equity, daily loss, maximum drawdown, and breach status. An account-level breach may result in all open positions being closed.

Each supported asset has a fixed leverage amount set by Bungee.

Leverage is not user-adjustable.

Example:

- BTC trades on Bungee use 5x leverage.
- A trader cannot manually select another leverage amount for BTC.

Bungee may change an asset’s fixed leverage prospectively based on market conditions, liquidity, volatility, venue limits, or risk considerations.

The current fixed leverage for each asset will be displayed in the Bungee dashboard.

## 10. Maximum Position Notional

Each supported market has a maximum permitted total open position notional, as shown on the Bungee assets page linked in Section 8.

Notional limits may vary by market based on:

- Liquidity
- Volatility
- Order-book depth
- Market impact
- Venue constraints
- Bungee’s internal risk limits

More liquid markets may have larger notional limits. Thin or volatile markets may have smaller limits.

Bungee may reduce notional limits, place a market into reduce-only mode, or disable a market entirely where necessary.

## 11. Aggregate Account Allocation

A trader may hold multiple active Bungee Funded Perp accounts, subject to a current maximum combined allocation of:

> **$100,000 total active account size**

This refers to the combined nominal size of the trader’s active Bungee Funded Perp accounts.

It is not:

- Margin used
- Position notional
- Per-trade exposure

Example:

- One $100,000 account = $100,000 combined allocation
- Two $50,000 accounts = $100,000 combined allocation
- Four $25,000 accounts = $100,000 combined allocation

Each account remains subject to its own risk limits and position restrictions.

---

# Part III — Trading and Execution

## 12. Execution Model

A Bungee Funded Perp account represents a trade-idea / trading-mandate relationship.

The trader submits trades through the Bungee interface.

Bungee may, at its discretion:

- Simulate trades internally
- Hedge some or all exposure
- Net exposure across accounts
- Externally execute trades
- Route orders to one or more venues or liquidity providers

The trader does not directly own or control Bungee’s underlying capital or external hedge positions.

The trader’s contractual account economics are determined by the Bungee account ledger and applicable program rules.

## 13. Trading Fees

Transaction fees for opening and closing positions are set at:

> **1.5 basis points (0.015%) of executed notional**

Maker and taker fees are matched at the same rate. The higher rate applies to both, so each maker or taker execution is charged 1.5 basis points.

The fee applies when opening and closing a position.

Trading fees are included in:

- Account equity
- Daily loss calculations
- Drawdown calculations
- Payout calculations

The live Bungee dashboard is the source of truth for the fee applied to a trade.

## 14. Funding

Funding is dynamic and is charged every hour on the applicable open position notional.

The minimum funding rate is:

> **0%**

The funding rate may change between hourly intervals based on market conditions and Bungee's funding methodology. A 0% rate means no funding charge is applied for that interval. Funding will not be negative and will not create a funding credit for the trader.

Funding is included in account equity and therefore affects:

- P&L
- Daily loss
- Maximum drawdown
- Payout eligibility

The live Bungee dashboard is the source of truth for funding timestamps and charges applied to an account.

## 15. Bot Activity, High-Frequency Trading, and Scalping

Bot activity, high-frequency trading (HFT), and scalping are prohibited on evaluation and funded accounts. Bungee monitors trading activity for these practices and will deny the applicable payout request when a prohibited pattern is confirmed.

Prohibited activity includes:

- **Bot activity:** Using software, scripts, automated trading systems, or APIs to make trading decisions or automatically submit, modify, or cancel orders. Ordinary trader-configured stop-loss and take-profit orders are not, by themselves, bot activity.
- **High-frequency trading (HFT):** Systematic high-speed order submission, modification, cancellation, or execution, including bursts of orders designed to exploit latency, stale prices, or differences in execution speed.
- **Scalping:** Repeated or systematic rapid entries and exits intended to capture small price movements, spreads, or short-lived execution advantages. This applies whether trades are placed manually or through automation.

### Monitoring and Review

Bungee may review order and execution logs, trading frequency, order-to-trade and cancellation ratios, holding-time distributions, repeated trade sizes and timing, evidence of automation, and the share of activity or profits attributable to these patterns. Activity may be assessed across related accounts where relevant.

There is no fixed minimum holding period or automatic profit removal based solely on how long a position is held. A single short-duration trade does not, by itself, establish scalping or HFT. Holding a position longer does not exempt a prohibited trading pattern from review.

Payouts may be held while suspicious activity is investigated. If Bungee confirms prohibited bot activity, HFT, or scalping, the applicable payout request will be denied. Bungee may also restrict trading, suspend or breach the account, or take other enforcement action under Section 30.

## 16. Slippage and Market Execution

Bungee may model realistic market execution, including:

- Spread
- Slippage
- Available order-book depth
- Market impact
- Partial fills
- Trading fees
- Funding
- Venue availability

A displayed price does not guarantee that the full order will be filled at that price.

Bungee may reject, resize, or limit orders that exceed:

- Available liquidity
- Asset position limits
- Account risk limits
- Venue constraints
- Internal risk controls

## 17. Extreme Volatility and Market Controls

Bungee may take protective action during abnormal market conditions.

Bungee may:

- Reduce maximum position size
- Change fixed leverage prospectively
- Place a market into reduce-only mode
- Reject new orders
- Force-close positions where required by risk rules
- Temporarily suspend a market
- Delist a market

These controls may be used when liquidity deteriorates, volatility becomes extreme, manipulation risk increases, or a venue becomes unreliable.

---

# Part IV — Permitted and Prohibited Trading

## 18. Public Trading Content

Traders may:

- Learn from public market commentary
- Follow public trading ideas
- Use publicly available research
- Independently act on content they discover

Bungee does not prohibit ordinary inspiration from public trading content.

## 19. Copy Trading and Coordinated Execution

The following are prohibited unless expressly approved by Bungee:

- Automatically mirroring another trader’s account
- Centrally controlling trades across multiple supposedly independent accounts
- Coordinated synchronized trading intended to evade risk limits
- Using services specifically designed to game prop-firm evaluations
- Sharing account credentials
- Allowing another person to operate an account

## 20. Cross-Account Hedging

Cross-account hedging is prohibited.

Examples include:

- Long BTC in one Bungee account while short BTC in another
- Using correlated assets to manufacture substantially offsetting exposure
- Coordinating opposite positions with another trader
- Intentionally creating one losing account and one winning account to manufacture payout asymmetry

Bungee may assess the economic substance of the trading pattern rather than only the exact symbol traded.

## 21. Technical and Market Abuse

Prohibited activity includes:

- Latency exploitation
- Stale-price exploitation
- Exploiting feed errors
- Exploiting platform bugs
- Manipulating Bungee’s execution or risk systems
- Using strategies that depend on simulated-market defects
- Front-running using non-public information
- Trading on material non-public information
- Artificially splitting exposure across identities or accounts to evade limits

## 22. Account Sharing

Accounts are personal to the approved trader.

The following are prohibited:

- Sharing login credentials
- Transferring or selling an account
- Allowing another person to trade the account
- Operating accounts on behalf of another trader
- Using multiple identities to evade Bungee limits

---

# Part V — Payouts

## 23. Profit Split

Bungee’s payout structure is:

- Standard: 80% trader / 20% Bungee

## 24. Minimum Payout

The minimum payout is:

> **$50 after Bungee’s profit split**

## 25. Payout Cap and Post-Payout Account Reset

Every funded account, regardless of account size or evaluation track, has a maximum gross payout cap per request per 24 hours:

> **$20,000 USD**

The cap applies before the 80% trader / 20% Bungee profit split and limits total gross payouts from each account to $20,000 in any rolling 24-hour period, including payouts split across multiple requests.

Each processed payout counts toward the limit for 24 hours from its processing timestamp. During that time, you may request additional payouts up to your remaining allowance, subject to payout eligibility.

If you withdraw the full $20,000 in one payout, you must wait 24 hours before another payout. If you withdraw it through multiple payouts, allowance becomes available progressively as each payout passes its 24-hour mark. The window does not reset at midnight.

For example, if you withdraw $12,000 gross at 10:00 UTC and $8,000 gross at 16:00 UTC, $12,000 of allowance becomes available at 10:00 UTC the next day, and another $8,000 at 16:00 UTC, assuming no further payouts are processed.

The rolling limit applies independently to each funded account and is not a lifetime limit on claimable profits.

When an approved payout is processed:

1. The gross approved payout amount is deducted from the account’s eligible claimable profits.
2. Any remaining unpaid eligible profits are recorded separately in the Bungee account ledger and remain claimable in later eligible payout cycles, subject to the same rolling payout cap, profit split, and payout eligibility rules. The reset does not forfeit these profits.
3. The funded trading account resets to its default state: its original starting balance and default daily-loss and maximum-drawdown limits for the applicable account size and track are restored. Separately recorded claimable profits are excluded from the trading balance, trading equity, and risk-limit calculations.

The static maximum drawdown floor after the reset is:

> **Maximum drawdown floor = original starting balance × (1 − applicable maximum drawdown percentage)**

The applicable percentages remain:

- Classic: 6%
- Pro: 5%
- Turbo: 3%

The reset occurs after every approved payout, including the first. A pending, rejected, cancelled, or reversed payout request does not trigger a reset. The account remains funded; the payout reset does not require a new evaluation or clear an unresolved breach or investigation.

### Worked Example

A $10,000 Classic funded account grows to a realized balance of $40,000, including $30,000 of eligible profits. The trader requests the maximum gross payout of $20,000:

- Gross payout deducted from eligible claimable profits: $20,000
- Trader share at the standard 80% split: $16,000
- Remaining gross eligible profits recorded separately and still claimable: $10,000
- Trading account balance after reset: $10,000
- Restored Classic maximum drawdown floor: $10,000 × 94% = $9,400
- Default maximum-drawdown buffer after reset: $600

The remaining $10,000 of gross eligible profits may be requested once the $20,000 payout passes its 24-hour mark and payout allowance becomes available again, subject to payout eligibility. They do not increase the reset account’s trading balance or drawdown allowance.

## 26. Payout Timing

Bungee targets processing valid payout requests within:

> **1 business day**

This is a target rather than an unconditional guarantee.

Payout availability is governed by the rolling 24-hour allowance in Section 25. There is no mandatory wait after each payout while sufficient allowance remains. A payout’s processing timestamp is the time when its approved gross amount is deducted from eligible claimable profits and the account reset is recorded.

A pending payout request must be resolved before another request can be submitted. Pending, rejected, or cancelled requests do not consume the rolling allowance. If a processed payout is reversed, its gross amount is removed from the rolling total.

A payout may take longer where:

- KYC is incomplete
- Compliance review is required
- Trading activity is under risk or abuse review
- The payout involves unusual or thin-market profits
- A technical or operational issue occurs

## 27. Payout Eligibility

A trader must:

- Be on an eligible funded account
- Have withdrawable profit
- Complete required KYC and compliance checks
- Have no unresolved hard breach
- Have no unresolved abuse or risk investigation
- Have no confirmed prohibited bot activity, HFT, or scalping for the applicable payout period
- Have sufficient remaining allowance under the rolling 24-hour payout cap for the requested gross amount
- Meet any operational requirements shown in the Bungee dashboard

KYC is intended to occur after passing the evaluation and before funded payouts.

---

# Part VI — Risk Review and Enforcement

## 28. Manual Payout and Risk Review

Bungee may manually review payouts and trading activity, particularly where profits are generated from:

- Thin or illiquid markets
- Unusually large positions
- Sudden liquidity events
- Potentially manipulated markets
- Suspicious trading patterns
- Bot activity, high-frequency trading (HFT), or repeated or systematic scalping
- Coordinated accounts
- Activities that appear designed to exploit the program

A market being tradeable does not guarantee that every trading pattern or payout will be accepted without review.

## 29. Discretionary Abuse Review

Bungee reserves the right to investigate behavior that appears designed to exploit the evaluation, risk, execution, or payout system, even where the exact conduct is not expressly listed in this rulebook.

Examples include:

- Mirrored trades across multiple accounts
- Coordinated opposite-side accounts
- Manufacturing payout asymmetry
- Exploiting thin-market pricing
- Latency or stale-price strategies
- Coordinated device, account, network, or automation behavior
- Deliberately exploiting a loophole in the rules
- Splitting exposure across identities to evade limits

Bungee may evaluate the overall economic substance and trading pattern, not only an isolated trade.

## 30. Enforcement Actions

Depending on the nature and severity of a violation, Bungee may:

- Reject an order
- Resize an order
- Restrict trading
- Force-close positions
- Place an account under review
- Suspend an account
- Deny an ineligible payout
- Reverse an improperly credited payout
- Permanently breach an account
- Close related accounts
- Disqualify a trader from Bungee Funded Perp

Ordinary risk-limit breaches are enforced according to the hard-breach policy.

Suspected abuse may be manually reviewed before a final decision.

---

# Part VII — Technical and Operational Rules

## 31. Platform and Dashboard as Source of Truth

Bungee’s internal records and dashboard govern:

- Balance
- Equity
- P&L
- Fees
- Funding
- Drawdown
- Daily loss
- Breach status
- Position size
- Supported markets
- Fixed leverage
- Payout eligibility
- Account status

External screenshots, spreadsheets, third-party charting systems, or trader-side calculations do not override Bungee’s records.

## 32. Technical Outages

Bungee is not responsible for losses or missed trading opportunities caused solely by:

- Internet connectivity issues on the trader’s side
- Device failures
- Third-party software
- Exchange or venue outages
- Network congestion
- Market-data interruptions
- Force majeure events

Where an outage originates from Bungee infrastructure, Bungee may review affected accounts and determine an appropriate remedy at its discretion.

## 33. Disputes and Logs

Bungee’s internal execution, account, pricing, and risk logs will be used when reviewing account disputes.

A trader may raise a dispute through Bungee’s designated support process.

Bungee may correct clear technical or accounting errors where supported by its internal records.

## 34. Rule Changes

Bungee may update:

- Supported markets
- Fixed leverage
- Position limits
- Fees
- Funding treatment
- Evaluation availability
- Operational requirements
- Risk controls

Material changes should be communicated through the Bungee platform or applicable terms.

Changes to market-risk settings may take effect immediately where required to protect traders, Bungee, venues, or liquidity providers.
