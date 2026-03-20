# Coin Collector

Multiplayer coin collecting game — two players compete in real time to grab coins faster than each other.

Built with a Python WebSocket server that acts as the authority for all game state, and a plain HTML/JS client. No frameworks.

## How it works

Server tracks everything — positions, coins, scores. Clients just send inputs and render what the server says. This prevents cheating and keeps both clients in sync.

Added 200ms artificial latency on both sides to simulate real network conditions, with client side interpolation so movement stays smooth despite the delay.

## Run it
```bash
pip install websockets
python server.py
```

Open `client.html` in two browser tabs.

## Demo

[Video](https://drive.google.com/file/d/1Rr736Lk9NQjuzL3JP1naCmpk6BSbQ9pf/view?usp=sharing)

![screenshot](./Screenshot.png)
