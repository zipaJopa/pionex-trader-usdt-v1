# pionex-trader-usdt-v1
Autonomous Pionex USDT Trading Agent - Real Money, Real Profits

This agent trades autonomously on Pionex using a USDT budget. 
It runs every 15 minutes via GitHub Actions.

**Configuration (via GitHub Secrets):**
- `PIONEX_API_KEY`: Your Pionex API Key.
- `PIONEX_API_SECRET`: Your Pionex API Secret.
- `GH_PAT`: GitHub Personal Access Token for saving results.

**Trading Strategy:**
- Focuses on symbols: SHIB/USDT, DOGE/USDT, PEPE/USDT, BTC/USDT, ETH/USDT
- Uses a simple RSI-based strategy on 15-minute candles.
- Buys on RSI < 30, sells on RSI > 70 (or via TP/SL).
- Manages a budget of 40.0 USDT.
- Max 10.0 USDT per trade per coin.
- Take Profit: 5.0%, Stop Loss: 2.0%.

**Results:**
Trade results, P&L, and cycle summaries are logged to the `zipaJopa/agent-results` repository.
