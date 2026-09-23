# Bungee Funded Perp Rulebook

> **Version:** v0.1 — Working Draft  
> **Status:** Product rulebook draft; subject to legal, compliance, risk, and operational review  
> **Last updated:** September 23, 2026

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
- Daily loss limit varies by evaluation type
- Maximum total drawdown varies by evaluation type

Exact evaluation parameters will be displayed on the relevant evaluation plan before purchase and inside the Bungee dashboard.

## 3. Evaluation Plans

Bungee intends to offer the following evaluation sizes and tracks.

| Account Size | Classic | Pro | Turbo |
| -----------: | ------: | --: | ----: |
| $10,000 | $90 | $70 | $45 |
| $25,000 | $230 | $165 | $105 |
| $50,000 | $430 | $300 | $195 |
| $100,000 | $865 | $590 | $360 |

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

The exact daily loss percentage will be defined per evaluation product and displayed in the dashboard.

The daily loss measurement resets each day at:

> **12:00 UTC**

The dashboard will display the active daily loss limit and the time remaining until the next reset.

## 6. Maximum Drawdown

Bungee uses a static maximum drawdown unless otherwise stated for a specific plan.

The drawdown limit is measured against the account’s defined starting balance and does not trail upward with profits.

Exact drawdown values will be defined per evaluation plan.

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

The initial intended market list is:

| Asset | Fixed Leverage | Max Position Size |
| ----- | -------------: | ----------------: |
| BTC | TBD | TBD |
| ETH | TBD | TBD |
| SOL | TBD | TBD |
| HYPE | TBD | TBD |
| XRP | TBD | TBD |
| BNB | TBD | TBD |
| DOGE | TBD | TBD |
| LINK | TBD | TBD |
| SUI | TBD | TBD |
| AVAX | TBD | TBD |

> More assets may be added over time after liquidity and risk review.  
> The live Bungee dashboard is the source of truth for currently supported markets.

## 9. Isolated Perpetuals and Fixed Leverage

All supported markets are perpetual contracts that use isolated margin.

Margin is assigned to each position independently and is not shared automatically with other open positions. A position's margin and liquidation risk are therefore isolated from the margin assigned to other positions.

Isolated margin does not remove account-level risk controls. Realized and unrealized P&L, trading fees, and funding from every position continue to affect account equity, daily loss, maximum drawdown, and breach status. An account-level breach may result in all open positions being closed.

Each supported asset has a fixed leverage amount set by Bungee.

Leverage is not user-adjustable.

Example:

- If BTC is set to 10x leverage, BTC trades on Bungee use 10x.
- A trader cannot manually select 5x, 2x, or another leverage amount for BTC.

Bungee may change an asset’s fixed leverage prospectively based on market conditions, liquidity, volatility, venue limits, or risk considerations.

The current fixed leverage for each asset will be displayed in the Bungee dashboard.

## 10. Maximum Position Size

Each supported asset has a maximum permitted open position size.

Position limits may vary by asset based on:

- Liquidity
- Volatility
- Order-book depth
- Market impact
- Venue constraints
- Bungee’s internal risk limits

More liquid markets may have larger position limits. Thin or volatile markets may have smaller limits.

Bungee may reduce position limits, place a market into reduce-only mode, or disable a market entirely where necessary.

## 11. Aggregate Account Allocation

A trader may hold multiple active Bungee Funded Perp accounts, subject to a current maximum combined allocation of:

> **$200,000 total active account size**

This refers to the combined nominal size of the trader’s active Bungee Funded Perp accounts.

It is not:

- Margin used
- Position notional
- Per-trade exposure

Example:

- Two $100,000 accounts = $200,000 combined allocation
- Four $50,000 accounts = $200,000 combined allocation

> **Placeholder:** The $200,000 cap may change once Bungee finalizes its maximum account sizes and product lineup.

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

## 15. Minimum Holding Period

Every position must remain open for at least:

> **5 minutes (300 seconds)**

A position cannot be closed or reduced during the minimum holding period. This restriction applies to manual closes and to stop-loss or take-profit instructions that would close or reduce the position.

Bungee may close a position before the minimum holding period ends when required for a hard breach, liquidation, market delisting, technical incident, or emergency risk control.

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

## 25. Payout Method

Initial payout method:

- USDC
- Ethereum / ERC-20

Bungee may add additional payout networks or methods over time.

## 26. Payout Timing

Bungee targets processing valid payout requests within:

> **1 business day**

This is a target rather than an unconditional guarantee.

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

1. Profit targets for Classic, Pro, and Turbo
2. Daily loss limits for each plan
3. Maximum static drawdown for each plan
4. Final fixed leverage per supported asset
5. Final max position size per supported asset
6. Whether the $200,000 combined allocation cap remains appropriate
7. Exact treatment of open positions during payout requests
8. Final restricted-jurisdiction policy
9. Final legal and compliance language
10. Any scaling or account-growth program

---

# Current Product Decisions at a Glance

| Rule | Bungee v0.1 |
| ---- | ----------- |
| Evaluation | One-step |
| Time limit | None |
| Minimum trading days | None |
| Consistency rule | None |
| Breach model | Hard breach |
| Drawdown | Static |
| Daily loss | Equity-based, including unrealized P&L |
| Daily reset | 12:00 UTC |
| Supported markets | Bungee allowlist only |
| Trading product | Isolated-margin perpetuals; no cross margin |
| Initial market count | 10 |
| More markets later | Yes, after risk review |
| Leverage | Fixed per asset; not user-adjustable |
| Position limits | Per asset |
| Minimum position holding period | 5 minutes |
| Combined active allocation | $200K placeholder |
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
| Payout asset | USDC ERC-20 initially |
| Payout target | 1 business day |
| KYC | After pass / before funded payout |
| Manual payout review | Yes |
| Emergency reduce-only / delisting | Yes |
| Dashboard / internal ledger | Source of truth |

---

> **Important:** This document is a product rulebook draft, not final legal terms. Before launch, it should be reconciled with Bungee’s actual execution infrastructure, risk engine, KYC/AML process, supported jurisdictions, venue relationships, and legal documentation.
