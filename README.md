# CookieRisk Quickscan for Cursor

Scan a public homepage for cookies and tracking observed before a visitor interacts with the consent banner.

## Use in Cursor

1. Install CookieRisk Quickscan from Cursor Marketplace. Cursor connects to the hosted service at https://cookierisk.eu/mcp. No CookieRisk account or API key is required.
2. Ask Cursor to run a CookieRisk Quickscan for a public homepage you want to check.
3. Approve the tool call when prompted. Cursor can retrieve the result using the scan ID returned by the server.

The server exposes two tools.

- `start_quickscan` starts a scan or reuses recent evidence for the domain. When available, the response says when the evidence was recorded and when the cooldown ends.
- `get_quickscan_result` retrieves scan progress and findings. Wait for the polling interval the server returns before checking again.

Quickscan covers the homepage before consent interaction. Accept and reject behavior are outside its scope.

See the [MCP setup guide](https://cookierisk.eu/developers/mcp), [privacy policy](https://cookierisk.eu/privacy), and [terms of service](https://cookierisk.eu/terms). For support, contact [CookieRisk](mailto:info@cookierisk.eu).
