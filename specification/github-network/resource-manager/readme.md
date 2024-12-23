# GitHub.Network Resource Provider

> see https://aka.ms/autorest

This is the AutoRest configuration file for GitHub.Network Resource Provider.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the Resource Provider.

---

```yaml
openapi-type: arm
openapi-subtype: rpaas
tag: package-2024-04-02
```

### Tag: package-2024-04-02

These settings apply only when `--tag=package-2024-04-02` is specified on the command line.

```yaml $(tag) == 'package-2024-04-02'
input-file:
  - GitHub.Network/stable/2024-04-02/GitHub.Network.json
```

### Tag: package-2024-04-01

These settings apply only when `--tag=package-2024-04-01` is specified on the command line.

```yaml $(tag) == 'package-2024-04-01'
input-file:
  - GitHub.Network/stable/2024-04-01/GitHub.Network.json
```

### Tag: package-2024-04-01-preview

These settings apply only when `--tag=package-2024-04-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2024-04-01-preview'
input-file:
  - GitHub.Network/preview/2024-04-01-preview/GitHub.Network.json
```

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

```yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-java
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-ruby
    after_scripts:
      - bundle install && rake arm:regen_all_profiles['azure_mgmt_github_network']
```

## Python

See configuration in [readme.python.md](./readme.python.md)

## Ruby

See configuration in [readme.ruby.md](./readme.ruby.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)
