# Changelog

This file records material changes to the Bungee Funded Perp rulebook.

## v0.1 - 2026-09-02

Status: Working Draft

- Established the one-step evaluation and hard-breach model.
- Defined all supported trading products as isolated-margin perpetual contracts with no cross margin.
- Finalized Classic, Pro, and Turbo profit targets, daily loss limits, static drawdowns, and one-step structure.
- Updated standard pricing and added referral and Founding Trader discount schedules.
- Finalized fixed leverage and maximum position notional for 21 supported markets.
- Set maker and taker trading fees to 1.5 basis points per execution.
- Set funding to a dynamic hourly rate with a 0% minimum.
- Set the daily loss reset time to 12:00 UTC.
- Added a five-minute profit-eligibility rule: profit from position quantities closed early is removed, while losses, fees, and funding remain.
- Defined FIFO treatment for position increases, partial reductions, and reversals under the five-minute rule.
- Added payout denial when Bungee detects a repeated or systematic scalping pattern.
- Set the payout split to 80% trader / 20% Bungee.
- Defined initial market, risk, execution, payout, and enforcement rules.
