# Packet Delivery Game

A single-file browser game for introducing basic networking ideas.

Players send packets from a laptop to a school server, compare three routes, and see how latency, congestion, packet loss, reliability, and total time affect delivery.

## Scan to Play

Open the game at:

[https://arif-zaman.github.io/packet-delivery/](https://arif-zaman.github.io/packet-delivery/)

![QR code for Packet Delivery Game](packet-delivery-qr.png)

## Run It

1. Download or clone this repository.
2. Open `index.html` in a web browser.
3. No server, install step, internet connection, or package manager is required.

You can also serve it locally:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## GitHub Pages

This project can be hosted on GitHub Pages because it is a static HTML file.

Use GitHub repository settings:

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/root`

The site will be available at:

```text
https://YOUR_USERNAME.github.io/YOUR_REPOSITORY/
```

## What You Learn

- Network: connected devices sharing information.
- Packet: one small chunk of a larger message.
- Router: a device that forwards packets toward a destination.
- IP address: a label that identifies a device on a network.
- Latency: how long a packet takes to arrive.
- Congestion: too much traffic on a route, like a crowded hallway or traffic jam.
- Packet loss: when a packet fails to arrive.
- Reliability: the percentage of sent packets that arrive successfully.
- Total time: total route time spent on packet attempts.
- Tradeoffs: the fastest route is not always the best route.

## Gameplay Features

- Three selectable paths: Fast, Backup, and Direct.
- Send one packet or a burst of five packets.
- Adjustable packet-loss sliders for all three paths.
- Live counters for delivered packets, lost packets, average latency, total time, and reliability.
- Event log showing route choices, delivered packets, and lost packets.
- Intro sections that connect networking to everyday internet use and explain packets/congestion before play.
- Mobile-friendly layout with compact controls and a horizontally scrollable network map.

## Suggested Demo Flow

1. Start with the everyday motivation: browsing, streaming, games, messages, and schoolwork all use networks.
2. Explain that data travels in small chunks called packets.
3. Ask which route looks best first and why.
4. Select the Fast route and send a burst.
5. Discuss why some packets may be lost when a route is crowded.
6. Try Backup and Direct, then compare reliability and total time.
7. Change the packet-loss sliders and predict what will happen.
8. Try to deliver 5 packets with the best mix of reliability and total time.

## Default Route Settings

- Fast: `120 ms`, `36%` packet loss.
- Backup: `210 ms`, `14%` packet loss.
- Direct: `150 ms`, `8%` packet loss.

These can be adjusted in the page with the Packet Loss sliders.
