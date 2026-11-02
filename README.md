# Crypto Intel — KuCoin USDT Spot starter

## Run
Open `index.html` in a modern browser. If direct file access blocks API requests, host this static folder on a free HTTPS static host (for example GitHub Pages or Cloudflare Pages).

## Data
Uses KuCoin public REST endpoints:
- `/api/v1/market/allTickers`
- `/api/v1/market/candles`

No API key, wallet connection, or trading permissions are used.

## Important limitations
- Public REST refreshes every 60 seconds; this starter is not a WebSocket stream.
- Top 20 are ranked by 24h quote volume among filtered USDT spot pairs.
- 7-day dip is calculated against the highest high among recent available candles.
- 1M is approximated using daily candles; it is not a native monthly candle interval.
- This is a screening tool, not a trading system. It does not place orders or guarantee BUY signals.
