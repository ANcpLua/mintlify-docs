# API Reference Documentation

@import ../CLAUDE.md

## Section Context

This section documents the **qyl API** - REST API for the observability platform.

### Key Principles

- OpenAPI spec is the source of truth: `/api-reference/openapi.yaml`
- Use Mintlify's OpenAPI integration for auto-generated endpoint pages
- Manual pages only for conceptual content (authentication, rate limits)

### OpenAPI Integration

In `docs.json`:

```json
{
  "tab": "API Reference",
  "groups": [
    {
      "group": "qyl API",
      "pages": ["api-reference/introduction"]
    }
  ],
  "openapi": "/api-reference/openapi.yaml"
}
```

### Endpoint Page Structure

Auto-generated from OpenAPI spec. Manual additions use:

```mdx
---
openapi: 'GET /endpoint'
---

Additional context here if needed.
```

### External Reference

Full documentation: https://ancplua.io/api-reference/introduction
