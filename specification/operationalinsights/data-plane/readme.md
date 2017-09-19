# OperationalInsightsData

> see https://aka.ms/autorest

This is the AutoRest configuration file for OperationalInsightsData.

---

## Getting Started

To build the SDK for OperationalInsightsData, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration

### Basic Information

These are the global settings for the OperationalInsightsData API.

``` yaml
title: OperationalInsightsDataClient
description: Operational Insights Data Client
add-credentials: true
tag: v1
```

### Tag: v1

These settings apply only when `--tag=v1` is specified on the command line.

``` yaml $(tag) == 'v1'
input-file:
- Microsoft.OperationalInsights/v1/OperationalInsights.json
```

---

# Code Generation

## C#

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

```yaml $(csharp)
csharp:
  namespace: Microsoft.Azure.Management.OperationalInsights.Data
  output-folder: $(csharp-sdks-folder)/OperationalInsights/Data/OperationalInsights.Data/Generated
  clear-output-folder: true
directive:
  reason: Don't expose the prefer param as a string query param. We'll make a better interface for this.
  from: swagger-document
  where: $.paths[*][*].parameters
  transform: >
    var idxToRemove = -1;
    for (var i=0; i<$.length; i++) {
      if ($[i]["$ref"] === "#/parameters/prefer-param") {
        idxToRemove = i;
        break;
      }
    }
    if (idxToRemove !== -1) {
      $.splice(idxToRemove, 1);
    }
```