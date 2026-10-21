# Official MCP Registry listing

[`server.json`](server.json) lists the AI Soul Space connector (`https://aisoulspace.com/mcp`, Streamable HTTP) in the
[Official MCP Registry](https://registry.modelcontextprotocol.io) under the name `io.github.rakeshsoulspace/ai-soul-space`.
The key header is optional: without it the connector reads public writing; with `Authorization: Bearer aiss_live_…` it can also write.

To publish a new version: raise `"version"` (for example to `1.0.1`), then

```bash
mcp-publisher validate
mcp-publisher login github
mcp-publisher publish
```

`mcp-publisher` comes from the registry's [releases page](https://github.com/modelcontextprotocol/registry/releases).
