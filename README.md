Build a complete, single-file HTML page called "AI Stock Analyst" — a cinematic,
dark-themed financial intelligence dashboard that simulates how an AI analyzes
stocks in real time.
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
VISUAL AESTHETIC
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Dark terminal aesthetic: deep black background (#0A0A0F) with electric green
(#00FF88) and cyan (#00D4FF) accents
- Font pairing: "Share Tech Mono" (monospace, techy) for data + "Orbitron"
(display) for headings — both from Google Fonts
- Animated scanline overlay effect across the whole page (CSS keyframe, subtle)
- Glowing neon borders on cards using box-shadow
- Numbers and data should flicker/pulse as if updating live
- Noise/grain texture overlay at low opacity for depth
- Cursor: custom crosshair cursor
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
PAGE LAYOUT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Header:
- Logo: "NEURAL STOCK AI" with a blinking cursor after it
- Subtitle: "Real-time AI Analysis Engine v2.4"
- Status badge: "● LIVE" blinking in green
Search section:
- Large input field: "Enter stock ticker (e.g. AAPL, TSLA, NVDA)"
- A glowing "ANALYZE" button
- Below it: 6 quick-pick chip buttons for popular tickers: AAPL · TSLA · NVDA ·
MSFT · AMZN · META
Main analysis panel (appears after searching):
Split into a responsive grid with these modules:
1. PRICE TICKER MODULE
- Shows: current price (large), % change, volume, market cap
- All values randomly generated but realistic per ticker
- Animate numbers counting up on load
2. AI THINKING MODULE (the star of the page)
- Title: " AI REASONING PROCESS"
- Shows a live typewriter animation of the AI "thinking out loud":
> "Fetching real-time data for [TICKER]..."
> "Analyzing 14 technical indicators..."
> "Checking RSI: 67.4 — approaching overbought territory"
> "MACD crossover detected — bullish signal"
> "Scanning news sentiment: 78% positive"
> "Comparing to sector peers..."
> "Running Monte Carlo simulation (10,000 runs)..."
> "Calculating risk/reward ratio..."
> "ANALYSIS COMPLETE"
- Each line appears one by one with a blinking cursor, like a terminal
3. TECHNICAL INDICATORS MODULE
- RSI, MACD, Moving Averages (50d / 200d), Bollinger Bands, Volume
- Each shown as a horizontal bar with color coding (green/red/yellow)
- Animated fill on load
4. SENTIMENT ANALYSIS MODULE
- "News Sentiment", "Social Media Buzz", "Analyst Consensus"
- Shown as circular progress rings that animate in
- Color: green = bullish, red = bearish
5. PRICE CHART MODULE
- A fake but realistic-looking SVG line chart showing 30-day price history
- Randomly generated but with smooth curves
- Hover tooltip showing price on each point
- Gradient fill under the line
6. AI VERDICT MODULE
- Large card at the bottom
- Shows: BUY / HOLD / SELL (randomly pick one, style it bold with matching
color)
- Confidence score: "Confidence: 84%"
- 3-line AI summary paragraph explaining the verdict
- "⚠ This is not financial advice. For entertainment purposes only."
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
TECHNICAL REQUIREMENTS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Single HTML file, NO external dependencies except Google Fonts (CDN)
- Pure HTML + CSS + Vanilla JavaScript only — no frameworks, no npm
- All data is simulated/randomly generated on the client side — no real API calls
needed
- Each ticker must produce consistent results (seed the random generator with the
ticker string so same ticker = same data every time)
- Fully responsive: works on mobile and desktop
- Smooth CSS animations throughout (no janky jumps)
- The "analyzing" sequence must feel dramatic and satisfying — add a 50-100ms
delay between each typewriter line
- After analysis completes, all modules animate in with staggered delays
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
EXTRA DETAILS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- Add a floating "particles" or matrix-rain effect in the background (subtle, CSS
or JS)
- Footer: "Powered by Neural Stock AI · Not financial advice"
- Add a "RESET" button to clear and search a new ticker
- All cards should have a subtle hover glow effect
- The page title (browser tab) should say: "Neural Stock AI — Real-Time Analysis"
Deliver everything as ONE complete index.html file ready to deploy on Netlify by
dropping into a folder. No build step required.
