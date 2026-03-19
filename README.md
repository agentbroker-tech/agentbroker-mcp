# AgentBroker MCP Server

**AgentBroker** is an AI-native cryptocurrency exchange built for autonomous agents. Register, deposit USDC, select a strategy, and trade — all programmatically via MCP tools. No KYC. No human sign-up required.

[![AgentBroker Server MCP server](https://glama.ai/mcp/servers/agentbroker-tech/agentbroker-mcp/badges/card.svg)](https://glama.ai/mcp/servers/agentbroker-tech/agentbroker-mcp)

## MCP Server

- **Endpoint:** `https://agentbroker.polsia.app/mcp`
- **Transport:** Streamable HTTP (MCP 2025-03-26)
- **Manifest:** `https://agentbroker.polsia.app/.well-known/mcp-server`
- **Agent Card:** `https://agentbroker.polsia.app/.well-known/agent.json`
- **OpenAPI:** `https://agentbroker.polsia.app/openapi.json`

## Tools (9 total)

| Tool | Description |
|------|-------------|
| `register_agent` | Create sandbox or live account — get API key instantly |
| `get_prices` | Real-time prices for 8 pairs (public) |
| `get_balance` | Account balance and holdings |
| `deposit` | Add USDC (virtual in sandbox, real in live) |
| `select_strategy` | momentum / grid / mean-reversion |
| `place_order` | Market or limit orders |
| `get_order_book` | Top 10 bids/asks per pair (public) |
| `get_trades` | Personal trade history |
| `withdraw` | Withdraw to external wallet (live only) |

## Supported Pairs

BTC/USDC · ETH/USDC · SOL/USDC · BNB/USDC · XRP/USDC · ADA/USDC · AVAX/USDC · MATIC/USDC

## Quickstart

```json
{
  "mcpServers": {
    "agentbroker": {
      "url": "https://agentbroker.polsia.app/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## Features

- No KYC — agents register with a name, get an API key instantly
- Sandbox with 10,000 virtual USDC for testing
- Real-time prices updated every 30s via CoinGecko
- 0.10% fees (0.05% for high-volume agents)
- REST API + WebSocket streaming + MCP transport

## Links

- Site: https://agentbroker.polsia.app
- MCP manifest: https://agentbroker.polsia.app/.well-known/mcp-server