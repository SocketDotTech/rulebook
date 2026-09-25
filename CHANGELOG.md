# Changelog

This file records material changes to the Bungee Funded Perp rulebook.

## v0.1 - 2026-09-02

Status: Working Draft

- Established the one-step evaluation and hard-breach model.
- Defined all supported trading products as isolated-margin perpetual contracts with no cross margin.
- Finalized Classic, Pro, and Turbo profit targets, daily loss limits, static drawdowns, and one-step structure.
- Updated standard pricing to match the live Bungee checkout.
- Finalized fixed leverage and maximum position notional for 21 supported markets.
- Set maker and taker trading fees to 1.5 basis points per execution.
- Set funding to a dynamic hourly rate with a 0% minimum.
- Set the daily loss reset time to 00:00 UTC.
- Set the minimum holding period to two minutes: profit from position quantities closed earlier is removed, while losses, fees, and funding remain.
- Defined FIFO treatment for position increases, partial reductions, and reversals under the two-minute rule.
- Added payout denial when Bungee detects a repeated or systematic scalping pattern.
- Set the payout split to 80% trader / 20% Bungee.
- Set the maximum gross payout to $20,000 USD per request for every account size and track, before the 80/20 profit split.
- Set a 24-hour per-account cooldown beginning when an approved payout is processed and the account reset is recorded; rejected, cancelled, and reversed requests do not restart it.
- Set the maximum combined active allocation to $100,000 in nominal account size per trader.
- Reset the funded account to its original starting balance and default risk limits after every approved payout.
- Preserved unpaid eligible profits as separately claimable amounts after reset, excluded from trading balance, equity, and risk-limit calculations.
- Defined initial market, risk, execution, payout, and enforcement rules.
