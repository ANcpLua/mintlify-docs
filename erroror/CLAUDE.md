# ErrorOrX Documentation

@import ../CLAUDE.md

## Section Context

This section documents **ErrorOrX** - a discriminated union library for .NET with ASP.NET Core integration.

### Key Principles

- ErrorOrX is a PRODUCT package (not part of ANcpLua framework infrastructure)
- Two packages: `ErrorOrX` (runtime) and `ErrorOrX.Generators` (source generator)
- Targets .NET 10, AOT-compatible
- Integrates with ASP.NET Core Minimal API

### Package Structure

| Package             | Target         | Purpose                           |
| ------------------- | -------------- | --------------------------------- |
| ErrorOrX            | net10.0        | Runtime `ErrorOr<T>` type         |
| ErrorOrX.Generators | netstandard2.0 | Source generator for Minimal APIs |

### Key Concepts

| Concept         | Description                                 |
| --------------- | ------------------------------------------- |
| `ErrorOr<T>`    | Discriminated union: value or errors        |
| `ErrorType`     | Enum: Validation, NotFound, Conflict, etc.  |
| `Error`         | Error instance with Code, Description, Type |
| HTTP Mapping    | ErrorType → HTTP status code → TypedResults |
| Results<> Union | Generated OpenAPI-compatible response types |
| Fluent API      | Then, Else, Match, Switch, FailIf           |

### Diagnostics

All diagnostics use the `EOE` prefix (ErrorOr Endpoints):

- EOE001-EOE021: Handler structure errors
- EOE023-EOE025: Parameter binding
- EOE030-EOE040: AOT/serialization
- EOE050-EOE054: API versioning

### External Reference

GitHub: https://github.com/ANcpLua/ErrorOrX
