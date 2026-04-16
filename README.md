# Eno – Capital One Help Center Chatbot

A configurable AI chatbot demo powered by Claude (claude-sonnet-4-20250514), with BM25 retrieval over a curated Capital One knowledge base.

## Features

- **RAG pipeline** — BM25 keyword retrieval over 30 KB articles, top 5 chunks injected as context
- **Persona editor** — bot name, avatar, tone, system prompt, greeting
- **Theme editor** — primary color, font, presets
- **Multi-turn conversation** — last 6 turns sent as context to Claude
- **Source citations** — relevant KB articles linked below each response

## Topics covered

Credit Cards · Checking & Savings · Auto Loans · Fraud & Disputes · Account Access · Capital One Cafés · Venture / Venture X · Miles & Rewards

## Running locally

```bash
npm install
npm start
# open http://localhost:3000
```

## Deployment

Deployed on [Railway](https://railway.app) from this GitHub repo. Every push to `main` triggers an auto-deploy.

## Stack

- Node.js + Express (static file server)
- Vanilla HTML/CSS/JS frontend
- Anthropic Claude API (`claude-sonnet-4-20250514`)
