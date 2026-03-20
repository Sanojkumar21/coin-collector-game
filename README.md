# Coin Collector

Multiplayer coin collecting game built with a Python WebSocket server and plain HTML/JS client.

## Architecture

Authoritative server model server owns all game state (positions, coins, scores). Clients send inputs and render server state only.

- 200ms artificial latency on both directions
- Client side interpolation for smooth movement under latency

## Setup
```bash
pip install websockets
python server.py
```

Open `client.html` in two browser tabs.

## Demo

[Video](https://drive.google.com/file/d/1Rr736Lk9NQjuzL3JP1naCmpk6BSbQ9pf/view?usp=sharing)

![screenshot](./Screenshot.png)
