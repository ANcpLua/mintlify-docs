# ANcpLua Framework Documentation

Documentation for the ANcpLua ecosystem: ANcpLua.NET.Sdk, ANcpLua.Analyzers, and ANcpLua.Roslyn.Utilities.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview documentation changes locally:

```bash
npm i -g mint
```

Run at the root of the documentation (where `docs.json` is located):

```bash
mint dev
```

View your local preview at `http://localhost:3000`.

## Publishing changes

Changes are deployed to production automatically after pushing to the default branch via the [Mintlify GitHub app](https://dashboard.mintlify.com/settings/organization/github-app).

## Troubleshooting

- Dev environment not running: Run `mint update` to get the latest CLI version
- Page loads as 404: Ensure you're in a folder with a valid `docs.json`

## Resources

- [Mintlify documentation](https://mintlify.com/docs)
- [ANcpLua on NuGet](https://www.nuget.org/profiles/ANcpLua)
- [ANcpLua on GitHub](https://github.com/ANcpLua)