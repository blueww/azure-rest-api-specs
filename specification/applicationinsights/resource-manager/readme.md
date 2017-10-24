# ApplicationInsights
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for ApplicationInsights.



---
## Getting Started 
To build the SDK for ApplicationInsights, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the ApplicationInsights API.

``` yaml
title: ApplicationInsightsManagementClient
description: Composite Swagger for Application Insights Management Client
openapi-type: arm
tag: package-2015-05
azure-validator: true
```

### Tag: package-2015-05

These settings apply only when `--tag=package-2015-05` is specified on the command line.

``` yaml $(tag) == 'package-2015-05'
input-file:
- microsoft.insights/2015-05-01/aiOperations_API.json
- microsoft.insights/2015-05-01/components_API.json
- microsoft.insights/2015-05-01/webTests_API.json
- microsoft.insights/2015-05-01/componentContinuousExport_API.json
- microsoft.insights/2015-05-01/componentFeaturesAndPricing_API.json
- microsoft.insights/2015-05-01/componentApiKeys_API.json
```
---
# Code Generation


## C# 

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  payload-flattening-threshold: 1
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.Management.ApplicationInsights.Management
  output-folder: $(csharp-sdks-folder)/ApplicationInsights/Management.ApplicationInsights/Generated
  clear-output-folder: true
```
