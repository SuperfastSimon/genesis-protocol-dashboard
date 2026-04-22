# Genesis Protocol Dashboard

A production-grade command centre for monitoring and controlling AutoGPT-powered agents across the Genesis Protocol ecosystem.

## Features

- 🔑 **API Key Authentication** — secure connection to the AutoGPT External API
- 🤖 **Agent Management** — list, inspect, and trigger agents with live status
- 📡 **Webhook Receiver** — real-time status push from AutoGPT via the genesis-protocol-proxy
- 📊 **Run History** — tabbed view of agent executions with input/output logs
- ⚡ **Live Console** — stream agent output in real time
- 🎨 **Saikou Design System** — dark glassmorphism UI, fully responsive

## Architecture

```
genesis-protocol-dashboard (this repo — static frontend, GitHub Pages)
        │
        ▼
genesis-protocol-proxy (Node.js/Express — CORS proxy + webhook store)
        │
        ▼
AutoGPT External API (backend.agpt.co/external-api/v1)
```

## Setup

1. Deploy [genesis-protocol-proxy](https://github.com/SuperfastSimon/genesis-protocol-proxy) to Render
2. Set your proxy URL and AutoGPT API key in the dashboard settings panel
3. Open `index.html` — works directly from GitHub Pages

## Deployment

Hosted via GitHub Pages at `https://superfastsimon.github.io/genesis-protocol-dashboard/`

No build step required — pure HTML/CSS/JS.
