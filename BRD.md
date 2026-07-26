# AlphaOS — Business Requirements Document

**Version:** 0.1 MVP  
**Owner:** Darrian Belcher  
**Product:** Browser-based options research and paper-trading decision-support tool

## Vision

Help self-directed investors turn market research into disciplined, explainable options decisions. AlphaOS is a probability and risk-management tool, not a promise of profit, brokerage, investment adviser, or autonomous trading bot.

## MVP goals

1. Manage a ticker watchlist.
2. Record a thesis and invalidation condition.
3. Score bullish or bearish setups using transparent inputs.
4. Recommend a defined-risk strategy or “no trade.”
5. Size contracts from maximum acceptable portfolio loss.
6. Save and review paper trades.
7. Teach calls, puts, Greeks, IV, liquidity, and time decay.

## Scoring model v0.1

- Trend alignment: 20%
- Fundamental quality: 15%
- Catalyst quality: 15%
- Sentiment alignment: 10%
- Volatility fit: 15%
- Liquidity: 15%
- Time-to-expiration fit: 10%
- Risk penalties: up to −30 points

Grades:

- **75–100:** qualified paper-trade candidate
- **60–74:** watch / needs confirmation
- **Below 60:** no trade

A high directional score can still fail because of expensive implied volatility, wide spreads, weak open interest, short expiration, event risk, or excessive position size.

## Included in MVP

- Manual research inputs
- Explainable rules engine
- Calls, puts, and debit-spread suggestions
- Position sizing
- Local browser storage
- Paper-trade journal
- JSON export
- Options learning center

## Excluded from MVP

- Live brokerage execution
- Fidelity credential storage
- Naked option selling
- Guaranteed predictions
- High-frequency trading
- Personalized fiduciary advice

## Roadmap

### V1

- Licensed quotes and option-chain data
- Greeks, IV, volume, and open interest
- SEC filing and news ingestion
- Authentication and encrypted database

### V2

- Walk-forward backtesting
- Calibrated probability models
- Portfolio Greeks and correlation
- Read-only broker import
- Alerts and daily research briefs

## Acceptance criteria

The MVP is accepted when a user can open `index.html`, score a setup, calculate risk-based contracts, save and close paper trades, retain data after refresh, export the journal, and use the options academy without external services.