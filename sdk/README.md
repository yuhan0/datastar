# Datastar SDK Directory

This directory contains the SDK test suite and related tools for Datastar SDK development.

## Structure

- `tests/` - Comprehensive test suite for validating SDK implementations
- `datastar-sdk-config.json` - SDK configuration with constants and defaults
- `datastar-sdk-config.schema.json-v1.json` - JSON schema for configuration validation
- `ADR.md` - Architecture Decision Record for SDK specifications

## SDK Development

### Configuration

The SDK configuration system provides:

- **Constants**: Event types, element patch modes, and other enums
- **Defaults**: Default values for booleans and durations
- **Literals**: List of known dataline literals
- **JSON Schema**: Validation for the configuration format

### Creating a New SDK

1. Read the [Architecture Decision Record](./ADR.md) for SDK specifications
2. Use [`datastar-sdk-config.json`](./datastar-sdk-config.json) as your source of constants
3. Implement the required `ServerSentEventGenerator` interface
4. Validate your implementation using the [test suite](./tests/README.md)

## Official SDKs

Official SDKs can be found at the [Datastar website](https://data-star.dev/reference/sdks).

## Available SDKs

The following SDKs are available for Datastar. Most have been moved to dedicated repositories for better maintainability and independent versioning.

| Language | Status | Repository |
|----------|--------|------------|
| Go | Official | [datastar-go](https://github.com/starfederation/datastar-go) |
| Python | Official | [datastar-python](https://github.com/starfederation/datastar-python) |
| TypeScript | Official | [datastar-typescript](https://github.com/starfederation/datastar-typescript) |
| Rust | Official | [datastar-rust](https://github.com/starfederation/datastar-rust) |
| PHP | Official | [datastar-php](https://github.com/starfederation/datastar-php) |
| C# (.NET) | Official | [datastar-dotnet](https://github.com/starfederation/datastar-dotnet) |
| Java | Official | [datastar-java](https://github.com/starfederation/datastar-java) |
| Ruby | Official | [datastar-ruby](https://github.com/starfederation/datastar-ruby) |
| Clojure | Official | [datastar-clojure](https://github.com/starfederation/datastar-clojure) |
| Haskell | Deprecated | - |
| Zig | Deprecated | - |

## Support

For SDK-specific issues, please open an issue in the respective SDK repository. For general Datastar questions or cross-SDK concerns, use the main [Datastar repository](https://github.com/starfederation/datastar).