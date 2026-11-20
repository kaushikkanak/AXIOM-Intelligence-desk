# AXIOM — The Intelligence Desk

An original, terminal-inspired research prototype. It displays current market quotes through TradingView alongside a clearly separate hypothetical portfolio and company dependency model. The fund-desk tone is inspired by financial dramas; no show's names, logos, or assets are used. The visual design does not reproduce Bloomberg software.

## Run locally

Unzip and open `index.html` in a current browser. No install or API key is required. **Connect to the internet to see market quotes.** For the most reliable loading, run `python3 -m http.server 8000` inside this folder and open `http://localhost:8000`. If opening the file directly blocks third-party widgets in your browser, use the server command. The local shock model still works offline.

TradingView supplies the top ticker and the market panel. Its embedded stock quotes may be delayed due to exchange rules. TradingView says forex and crypto widget quotes are live. The external widgets do not supply data to the shock calculator. Neither a paid TradingView account nor an API key is required for these public widgets, but your browser must allow scripts from TradingView.

## Two-minute demo

1. **Command center:** Show the real market ticker and overview, then point out that the separate ₹1,00,000 model portfolio is hypothetical. Helix AI is absent from that portfolio.
2. **Company network:** Search `HELX` or click Helix AI. Follow the *invented* model arrows: Helix buys from Nimbus Cloud; Nimbus buys chips from Vector and power from Gridline. Select Nimbus to see its modeled suppliers and customers. The model nodes have no asserted market quotes or news.
3. **Shock laboratory:** Select the AI spending pullback, leave the shock at 18%, and click Run Simulation. The highlighted chain and per-position loss show the result. Adjust severity, or try the other scenarios.
4. **Portfolio & funds:** Expand AXIS Connected Fund to show its components. Three fund components overlap with directly held shares.

## Modeling notes

The scenario uses a transparent, deterministic linear rule. In the default example, Nimbus's decline is 40% of the Helix spending shock; Vector's is 28% of Nimbus's decline; Gridline's is 18% of Nimbus's decline. The ETF decline is the weighted sum of its component declines. Loss for each position is position value × modeled decline. Other scenarios have their own listed assumptions. Cash is unaffected. Values are rounded for display.

Market quotes come from TradingView. The model companies, symbols, business relationships, sample account balance, fund weights, shock coefficients, and results are invented assumptions and are never presented as real market data. This is not financial advice or a brokerage. The share counts are illustrative and do not determine the displayed rounded position values.
