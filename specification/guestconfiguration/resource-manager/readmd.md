# Guest Configuration
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for Guest Configuration.



---
## Getting Started 
To build the SDK for Guest Configuration, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the Guest Configuration API.

``` yaml
title: GuestConfigurationClient
description: Guest Configuration Client
openapi-type: arm
tag: package-2017-10
```


### Tag: package-2017-10

These settings apply only when `--tag=package-2017-10` is specified on the command line.

``` yaml $(tag) == 'package-2017-10'
input-file:
- Microsoft.GuestConfiguration/2017-10-31/guestConfiguration.json
```



---
# Code Generation


## C# 

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.GuestConfiguration
  output-folder: $(csharp-sdks-folder)/GuestConfiguration/Azure.GuestConfiguration/Generated
  clear-output-folder: true
```

