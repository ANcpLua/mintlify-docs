# Analyzers Documentation

@import ../CLAUDE.md

## Section Context

This section documents **ANcpLua.Analyzers** - Roslyn analyzers for code quality.

### Key Principles

- Analyzers are auto-included with SDK - no separate installation needed
- Each rule page follows consistent structure: description, bad/good examples, configuration
- Configuration is always via `.editorconfig`

### Rule Categories

| Category          | Focus                                  |
| ----------------- | -------------------------------------- |
| Design            | Primary constructors, type structure   |
| Usage             | Span, IXmlSerializable, static lambdas |
| Style             | Pattern matching, null guards          |
| ASP.NET Core      | Form binding, parameter validation     |
| OpenTelemetry     | Semantic conventions                   |
| Threading         | Lock statement patterns                |
| Reliability       | Division by zero                       |
| VersionManagement | Hardcoded versions                     |

### Rule Page Structure

````mdx
---
title: 'AL0001'
description: 'One-line description'
---

## Problem

What triggers this diagnostic.

## Bad Code

```csharp
// Code that triggers AL0001
```
````

## Good Code

```csharp
// Corrected code
```

## Configuration

```ini
dotnet_diagnostic.AL0001.severity = warning
```

```

### External Reference

Full documentation: https://ancplua.io/analyzers/overview
```
