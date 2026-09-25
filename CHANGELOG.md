# Changelog

This file records material changes to the Bungee Funded Perp rulebook.

## v0.1 - 2026-09-02

Status: Working Draft

- Established the one-step evaluation and hard-breach model.
- Defined all supported trading products as isolated-margin perpetual contracts with no cross margin.
- Finalized Classic, Pro, and Turbo profit targets, daily loss limits, static drawdowns, and one-step structure.
- Updated standard pricing to match the live Bungee checkout and recalculated the referral and Founding Trader discount schedules.
- Finalized fixed leverage and maximum position notional for 21 supported markets.
- Set maker and taker trading fees to 1.5 basis points per execution.
- Set funding to a dynamic hourly rate with a 0% minimum.
- Set the daily loss reset time to 00:00 UTC.
- Set the minimum holding period to two minutes: profit from position quantities closed earlier is removed, while losses, fees, and funding remain.
- Defined FIFO treatment for position increases, partial reductions, and reversals under the two-minute rule.
- Added payout denial when Bungee detects a repeated or systematic scalping pattern.
- Set the payout split to 80% trader / 20% Bungee.
- Added gross per-request payout caps of $5,000, $10,000, $15,000, and $20,000 for the $10K, $25K, $50K, and $100K account sizes respectively.
- Added a 48-hour per-account cooldown beginning when an approved payout is deducted; rejected, cancelled, and reversed requests do not restart it.
- Added a post-payout drawdown rebase: after every approved payout, the realized post-payout balance becomes the new reference for the account's static maximum drawdown.
- Defined initial market, risk, execution, payout, and enforcement rules.
