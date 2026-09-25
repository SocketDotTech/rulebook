# Bungee Funded Perp Rulebook

> **Version:** v0.1 — Working Draft\
> **Status:** Product rulebook draft; subject to legal, compliance, risk, and operational review  
> **Last updated:** September 25, 2026

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

### Standard Pricing

| Account Size | Classic | Pro | Turbo |
| -----------: | ------: | --: | ----: |
| $10,000 | $110 | $85 | $50 |
| $25,000 | $275 | $200 | $120 |
| $50,000 | $520 | $380 | $220 |
| $100,000 | $1,000 | $750 | $400 |

> Pricing and plan availability may change. The live checkout page and Bungee dashboard are the source of truth.

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

## 8. Initial Supported Markets

The initial supported market list is:

| Market | Fixed Leverage | Maximum Position Notional |
| --- | ---: | ---: |
| BTC | 5x | $500,000 |
| ETH | 4x | $500,000 |
| SOL | 3x | $250,000 |
| XRP | 3x | $100,000 |
| HYPE | 3x | $100,000 |
| BNB | 3x | $50,000 |
| LINK | 2x | $20,000 |
| AAVE | 2x | $25,000 |
| LTC | 2x | $20,000 |
| ADA | 2x | $20,000 |
| GOLD | 3x | $150,000 |
| SILVER | 2x | $75,000 |
| CL | 2x | $75,000 |
| SP500 | 4x | $250,000 |
| XYZ100 | 3x | $150,000 |
| AAPL | 2x | $25,000 |
| MSFT | 2x | $25,000 |
| GOOGL | 2x | $25,000 |
| AMZN | 2x | $20,000 |
| NVDA | 2x | $50,000 |
| META | 2x | $20,000 |

> More assets may be added over time after liquidity and risk review.  
> The live Bungee dashboard is the source of truth for currently supported markets.

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

Each supported market has a maximum permitted total open position notional, as listed in Section 8.

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

## 15. Two-Minute Profit Eligibility and Scalping

Bungee permits short-term trading, but discourages rapid scalping patterns that rely on repeatedly entering and exiting positions over very short periods.

For profit from a position to be eligible, the relevant position quantity must remain open for at least:

> **2 minutes (120 seconds)**

If any position quantity is closed or reduced less than 120 seconds after it was opened:

- Any positive realized P&L attributable to that quantity will be removed from the account and excluded from profit-target, account-performance, and payout calculations.
- Any negative realized P&L will remain on the account and continue to count toward all applicable loss and drawdown limits.
- Trading fees, funding charges, and other applicable costs will remain payable and will not be reversed.
- Closing the position early is permitted and does not, by itself, constitute an account breach.

This rule applies regardless of how the position is closed or reduced, including:

- Manual closes
- Market, limit, and reduce-only orders
- Partial closes or scaling out
- Stop-loss and take-profit execution
- Automated strategies, bots, or APIs

Each increase in a position is treated as a separate opening quantity with its own two-minute timer. Position reductions are matched against opening quantities using first-in, first-out (FIFO) accounting. Reversing a position closes the existing quantity and opens any remaining quantity in the opposite direction with a new timer.

A quantity closed exactly 120 seconds or more after its opening execution is eligible for profit.

Closures initiated solely by Bungee for a technical incident, market delisting, or emergency administrative action are exempt. Liquidations and trader-configured stop-loss or take-profit executions are not exempt.

### Scalping-Pattern Review

Repeated or systematic opening and closing of positions within two minutes may constitute a prohibited scalping pattern. Bungee may consider the frequency of short-duration trades, their share of total trading activity or realized profit, trade-duration distribution, use of automation, and reliance on minor price movements or execution conditions.

If Bungee determines that a scalping pattern occurred, the applicable payout request will be denied. This review is separate from the automatic removal of profit from individual short-duration trades; removal of that profit does not prevent the broader pattern from being reviewed. Bungee may also take additional enforcement action under Section 30 where the activity involves another prohibited practice.

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

Every funded account, regardless of account size or evaluation track, has the same maximum gross payout cap per request:

> **$20,000 USD**

The cap applies to the gross payout request before the 80% trader / 20% Bungee profit split. It is a per-request cap for each account, not a lifetime limit on claimable profits.

When an approved payout is processed:

1. The gross approved payout amount is deducted from the account’s eligible claimable profits.
2. Any remaining unpaid eligible profits are recorded separately in the Bungee account ledger and remain claimable in later eligible payout cycles, subject to the same cap, profit split, cooldown, and payout eligibility rules. The reset does not forfeit these profits.
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

The remaining $10,000 of gross eligible profits may be requested after the 24-hour cooldown, subject to payout eligibility. They do not increase the reset account’s trading balance or drawdown allowance.

## 26. Payout Timing

Bungee targets processing valid payout requests within:

> **1 business day**

This is a target rather than an unconditional guarantee.

After an approved payout is processed for a funded account, the trader must wait:

> **24 hours**

before submitting another payout request for that same account. The cooldown begins at the timestamp when the approved gross payout is deducted from eligible claimable profits and the account reset is recorded. It applies independently to each funded account.

The first payout request on an account is not subject to a cooldown. A pending payout request must be resolved before another request can be submitted. A rejected, cancelled, or reversed request does not start or restart the 24-hour cooldown.

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
- Have no detected prohibited scalping pattern for the applicable payout period
- Have completed the applicable 24-hour payout cooldown
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
- Repeated or systematic short-duration scalping
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

---

# Part VIII — Items Still to Finalize

The following remain open before final launch:

1. Exact daily-loss baseline and equity-floor calculation at 00:00 UTC
2. Whether maximum position notional is enforced per account or across all accounts belonging to a trader
3. Maximum funding rate and the dynamic funding calculation methodology
4. Exact treatment of open positions and equity limits while a payout request is pending
5. Final restricted-jurisdiction, VPN, and minimum-age policies
6. Final legal, compliance, refund, and KYC language
7. Any scaling or account-growth program

---

# Current Product Decisions at a Glance

| Rule | Bungee v0.1 |
| ---- | ----------- |
| Evaluation | One-step |
| Time limit | None |
| Minimum trading days | None |
| Consistency rule | None |
| Breach model | Hard breach |
| Profit target | Classic 10%; Pro 12%; Turbo 9% |
| Drawdown | Classic 6%; Pro 5%; Turbo 3%; static |
| Daily loss | 3%; equity-based, including unrealized P&L |
| Daily reset | 00:00 UTC |
| Supported markets | Bungee allowlist only |
| Trading product | Isolated-margin perpetuals; no cross margin |
| Initial market count | 21 |
| More markets later | Yes, after risk review |
| Leverage | Fixed per asset; not user-adjustable |
| Maximum position notional | Per market; values listed in Section 8 |
| Short-duration profit eligibility | Position quantity must remain open for at least 2 minutes; earlier profit is removed |
| Detected scalping pattern | Applicable payout request denied |
| Combined active allocation | $100K maximum nominal account size across all active accounts |
| Cross-account hedging | Prohibited |
| Public-content inspiration | Allowed |
| Automated/coordinated copy trading | Prohibited |
| Account sharing | Prohibited |
| Latency / stale-price exploitation | Prohibited |
| Execution model | Simulate, hedge, net, or externally execute at Bungee’s discretion |
| Trading fees | Maker and taker matched at 1.5 bps (0.015%) per execution |
| Funding | Dynamic, charged hourly, with a 0% minimum rate |
| Standard payout split | 80/20 |
| Minimum payout | $50 |
| Gross payout cap | $20,000 USD per request for every account size and track, before the profit split |
| Payout cooldown | 24 hours per account after an approved payout is processed and the reset is recorded |
| Post-payout account reset | Original starting balance and default risk limits restored after every approved payout |
| Unpaid eligible profits | Remain separately claimable after reset; excluded from trading balance, equity, and risk limits |
| Payout asset | USDC ERC-20 initially |
| Payout target | 1 business day |
| KYC | After pass / before funded payout |
| Manual payout review | Yes |
| Emergency reduce-only / delisting | Yes |
| Dashboard / internal ledger | Source of truth |

---

> **Important:** This document is a product rulebook draft, not final legal terms. Before launch, it should be reconciled with Bungee’s actual execution infrastructure, risk engine, KYC/AML process, supported jurisdictions, venue relationships, and legal documentation.
