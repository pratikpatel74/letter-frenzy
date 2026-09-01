# 🔤 Letter Frenzy

A real-time multiplayer Scattergories-style word game built with vanilla JS and Supabase.

## How to Play

1. One player creates a game room and shares the 4-letter code
2. Other players join using the code
3. Each round, a letter is revealed — fill in every category with a word starting with that letter
4. Unique answers score 10pts, duplicates score 5pts, blank/wrong-letter answers score 0
5. Players can challenge each other's answers — the host rules on disputes
6. After all rounds, the highest score wins!

## Features

- 🎲 Random letter mode or 🗳️ Players Pick mode
- Fuzzy duplicate detection (Levenshtein ≤ 2)
- Animated SVG countdown timer (green → orange → red)
- Challenge system with host arbitration
- Post-game score sharing
- Mobile-first, works on any device
- Session reconnect — refresh the tab without losing your place

## Tech Stack

- **Frontend**: Vanilla JS, single HTML file, no build step
- **Backend**: [Supabase](https://supabase.com) — Postgres + Realtime WebSockets
- **Hosting**: Netlify

## Local Development

Just open `index.html` in a browser — no build step required.
