# Cashflow 101 Multiplayer Foundation

A mobile-friendly, browser-based multiplayer room foundation for the Cashflow 101 game.

## Current scope
- Create a 6-character room code.
- Join an existing room with the code or ?room=ABC123.
- Multiple players can join the same room.
- Supabase Realtime Presence keeps the live player list synchronized.
- The host is elected automatically from the oldest connected player.
- Ready/unready status updates instantly for everyone.
- A lightweight Broadcast state channel is included for future game state.
- No game rules are implemented yet.

## Stack
- Plain HTML/CSS/JavaScript
- Supabase Realtime
- No framework or build step required
- Deployable as a static site on Vercel

## Setup
1. Create or use a Supabase project.
2. Copy the project URL and publishable/anon key.
3. Open the game and enter those values in the setup panel.
4. Save configuration in the browser.
5. Create a room on one device and join it from other devices using the room code.

Never place a service-role key in the browser.

## Future game layer
The realtime foundation is intentionally separate from game rules. Future modules can add turn management, player money/assets/liabilities, cards, random events, transactions, win/lose conditions, authoritative server validation, reconnect/state recovery, and persistent match history.
