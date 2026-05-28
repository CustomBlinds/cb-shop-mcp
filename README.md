# Custom Blinds Shop MCP

South Africa's first AI-transactable window covering catalogue. Lets MCP-compatible AI agents (Claude, ChatGPT, Cowork, Cursor) search the Custom Blinds catalogue, get live ZAR pricing, configure products, submit enquiries, and create draft orders with Yoco payment links — direct from [shop.customblinds.co.za](https://shop.customblinds.co.za).

<!-- mcp-name: io.github.CustomBlinds/cb-shop -->

## What it does

| Tool | Access | Description |
|---|---|---|
| `search_products` | Open | Filter the Custom Blinds catalogue by product type and colour |
| `get_price` | Open | Live ZAR pricing by product, width, and height |
| `configure_product` | Open | Full product configuration with colour validation |
| `submit_enquiry` | Bearer token | Send an enquiry to rfq@customblinds.co.za |
| `create_order` | Bearer token | Draft an order and return a Yoco payment link |

Bearer tokens for transactional tools are issued on request — contact rfq@customblinds.co.za.

## Connection

This is a **remote** MCP server — no install required.

### Claude Desktop / Claude Code

```json
{
  "mcpServers": {
    "custom-blinds-shop": {
      "url": "https://shop.customblinds.co.za/mcp",
      "transport": "streamable-http"
    }
  }
}
```

### Other clients

Point your MCP client at:
https://shop.customblinds.co.za/mcp
Transport: streamable-HTTP.

## Verification

- Manifest: https://shop.customblinds.co.za/mcp-manifest.json
- Verify page: https://customblinds.co.za/verify/
- llms.txt: https://customblinds.co.za/llms.txt

## About Custom Blinds

Custom Blinds Shutters & Awnings (Pty) Ltd — established 2010 in Stellenbosch, South Africa. Duncan Walls, 20+ years industry experience.

- Brochure: https://customblinds.co.za
- Shop: https://shop.customblinds.co.za
- Issues: https://github.com/CustomBlinds/cb-shop-mcp/issues

## License

MIT
