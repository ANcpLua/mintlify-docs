# ANcpLua Framework Documentation

Documentation for the ANcpLua ecosystem: ANcpLua.NET.Sdk, ANcpLua.Analyzers, and ANcpLua.Roslyn.Utilities.

## Setup

```bash
npm install
```

## Development

```bash
npm run dev
```

View your local preview at `http://localhost:3000`.

## Automation

This repo has self-healing automation built in:

| Layer      | What                           | Auto-fix    |
| ---------- | ------------------------------ | ----------- |
| Pre-commit | Prettier formats MDX/JSON/YAML | Yes         |
| CI         | Broken link detection          | Report      |
| CI         | Accessibility checks           | Report      |
| CI         | OpenAPI validation             | Report      |
| CI         | Formatting fixes               | Auto-commit |

### Commands

```bash
npm run format       # Auto-fix formatting
npm run lint         # Run all checks
npm run lint:links   # Check broken links
npm run lint:a11y    # Check accessibility
npm run lint:openapi # Validate OpenAPI spec
```

## Publishing

Changes deploy automatically after pushing to `main` via
the [Mintlify GitHub app](https://dashboard.mintlify.com/settings/organization/github-app).

## Resources

- [Mintlify documentation](https://mintlify.com/docs)
- [ANcpLua on NuGet](https://www.nuget.org/profiles/ANcpLua)
- [ANcpLua on GitHub](https://github.com/ANcpLua)
