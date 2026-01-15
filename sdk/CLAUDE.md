# SDK Documentation

@import ../CLAUDE.md

## Section Context

This section documents **ANcpLua.NET.Sdk** - an MSBuild SDK for .NET 10 projects.

### Key Principles

- SDK docs show WHAT we provide and HOW to use it
- Installation instructions belong in `/quickstart` only - reference with links
- Features are auto-injected; opt-out properties are documented, not "installation"
- Link to Microsoft docs for external concepts (e.g., MTP)

### SDK Variants

| Variant                | Use Case                    |
| ---------------------- | --------------------------- |
| `ANcpLua.NET.Sdk`      | Libraries, Console, Workers |
| `ANcpLua.NET.Sdk.Web`  | ASP.NET Core APIs           |
| `ANcpLua.NET.Sdk.Test` | xUnit v3 test projects      |

### Pages in This Section

| Page                | Purpose                       |
| ------------------- | ----------------------------- |
| overview            | Feature summary with links    |
| variants            | What each variant provides    |
| msbuild-properties  | Complete property reference   |
| service-defaults    | Web SDK configuration         |
| polyfills           | netstandard2.0 compatibility  |
| extensions          | Opt-in code injection         |
| shared-utilities    | Guard clauses, test helpers   |
| banned-apis         | Deprecated API enforcement    |
| configuration-files | EditorConfig files included   |
| testing             | Integration test base classes |

### External Reference

Full documentation: https://ancplua.io/sdk/overview
