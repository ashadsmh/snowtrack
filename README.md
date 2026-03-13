# SnowTrack ❄️
Live ski resort conditions for 12 major US resorts — 
because powder waits for no one.

🔗 [snowtrack-co.vercel.app](https://snowtrack-co.vercel.app)

---

## What It Does
SnowTrack pulls live weather data for 12 ski resorts across 
four US regions and turns it into an actionable conditions 
dashboard. Check snow, compare resorts, and plan your trip 
without bouncing between a dozen resort websites.

---

## Under The Hood
- **12 concurrent API calls** on page load via Promise.all() — 
  each resort fetches independently so one failure never 
  blocks the rest
- **Lift status engine** — derives open/closed/hold status 
  from live wind, temperature, and snowfall data rather than 
  relying on a third-party feed that doesn't exist for free
- **Temperature scoring algorithm** — weights ideal skiing 
  conditions (15-25°F) with directional bias toward warmer 
  end of range when comparing resorts
- **Comparison tool** — dynamically highlights best-value 
  metrics across up to 5 selected resorts in real time

---

## Tech
Vanilla HTML, CSS, JavaScript · Open-Meteo API · Vercel

---

## Why Vanilla JS
No frameworks, no build tools, no dependencies. 
Fast to load, easy to maintain, and it proves the fundamentals.

---

Built by [Ashad Shaik-Mohamed](https://github.com/ashadsmh)
