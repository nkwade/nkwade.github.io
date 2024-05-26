---
title: "Celerity"
date: 2024-05-24T20:28:35-04:00
draft: false
---
This project by far has been the most time consuming, most lines of code, and most educational project I have undertaken as a software engineer. I wouldn't consider myself a "Crypto Bro", but I do love the ethos underlying crypto: decentralized and fair finance for all. Because of this I had met some cool people working in crypto and one of them reached out to me because he knew I was a software engineer. He had an idea of building a better trading platform on top of decentralized exchanges (DEXs) than the rest of the competition. He is an experienced trader and knew what people liked, disliked, and wanted from their decentralized trading platform. With this in mind we have been building [Celerity: Solana Trading Platform](https://www.celerity.bot). <!--more--> We first started out with building a frontend for Discord, because nearly all platforms were Telegram or Web based, but Discord is the home for most of the crypto communities today. Once I completed that we have been working towards building a faster, more comprehensive web terminal using my underlying backend for the discord bot as the web terminals backend. 

## Quick Stats
- Active Traders: 100+
- Volume Traded: Over $107k/636SOL
- Lines Of Code: 
    - Total: 10,000 
    - 8,552 lines of code 
    - ~1,500 lines of comments/docstrings

## Tech Stack
- Backend
    - Python
    - [Solana-Py: Open source Python Solana SDK](https://github.com/michaelhly/solana-py)
    - MongoDB: JSON-based Database
    - Built my own API wrappers for Jupiter, Dexscreener, CoinGeckoTerminal, and Raydium in Python
- API
    - Python
    - Quart (async Flask fork)
- Frontend
    - [Py-Cord: Python Discord Bot Package](https://docs.pycord.dev/en/stable/)
    - Website is built by our web dev
- CI/CD
    - MyPy: Python static typer 
    - Black: Automatic Python Code Formatter
    - Sphinx: Automatic Document Generation From Python Docstrings & Types
    - Pydantic: Automatic OpenAPI documentation for API endpoints
    - Conda: Python virtual environment manager
    - Github Workflows/Actions
- Server
    - Current: Azure VM
    - For Web Terminal Launch: AWS (faster and cheaper, but more complex)

## Timeline
2024:
- Jan: Co-founder reached out to me and planning for Celerity began
- Feb: Connected Solana & Jupiter DEX Aggregator to Discord bot
- Mar: Connected On-Chain Coin Databases Dexscreener & CoinGeckoTerminal, and Raydium DEX to Discord bot
- Apr: V1 release, bug fixing, UI updates
- May: Work on web terminal began, building an API for our web dev to integrate