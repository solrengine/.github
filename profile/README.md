# SolRengine

**The Rails framework for building Solana dapps.**

Rails is the most productive web framework. Solana is the fastest blockchain. SolRengine connects them.

## Why Rails + Solana?

Most Solana dapps are CRUD apps with wallet auth — exactly what Rails was built for. You don't need React, Next.js, or a JavaScript backend to build on Solana. You need a framework that gets out of your way.

SolRengine gives Rails developers:

- **Wallet Authentication** — Sign in with any Solana wallet via SIWS. Ed25519 verification in Ruby.
- **RPC Client** — Talk to Solana from Ruby. Balances, tokens, transactions, blockhash.
- **Token Portfolio** — SPL token metadata from Jupiter. USD prices. Persisted in your database.
- **SOL Transfers** — Build transactions with @solana/kit, sign with the wallet, track confirmation.
- **Real-time Updates** — Solana WebSocket subscriptions push to your UI via Turbo Streams.

All using the Rails 8 default stack: Hotwire, Turbo, Stimulus, Solid Queue, Solid Cache, Solid Cable, SQLite.

## Quick Start

```ruby
gem "solrengine"
```

```bash
rails generate solrengine:install
rails db:migrate
bin/dev
```

## The Gems

| Gem | What |
|-----|------|
| [solrengine](https://github.com/solrengine/solrengine) | Meta-gem — bundles everything |
| [solrengine-auth](https://github.com/solrengine/auth) | SIWS wallet authentication |
| [solrengine-rpc](https://github.com/solrengine/rpc) | Solana JSON-RPC client |
| [solrengine-tokens](https://github.com/solrengine/tokens) | Token metadata + portfolio via Jupiter |
| [solrengine-transactions](https://github.com/solrengine/transactions) | SOL transfers + confirmation tracking |
| [solrengine-realtime](https://github.com/solrengine/realtime) | WebSocket monitoring + Turbo Streams |

Each gem works independently or together via `solrengine`.

## Showcase

[**WalletTrain**](https://github.com/solrengine/wallet-train) — a full-featured Solana wallet built with SolRengine. Wallet auth, token portfolio, send SOL, real-time updates, landing page with on-chain donations.

---

A [Moviendome](https://moviendo.me) project.
