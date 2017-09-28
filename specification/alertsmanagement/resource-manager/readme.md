# AlertsManagement
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for AlerManagement.


---
## Getting Started 
To build the SDK for AlertManagement, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information 
These are the global settings for the AlertManagement API.

``` yaml
openapi-type: arm
tag: package-2017-10
```


### Tag: package-2017-10

These settings apply only when `--tag=package-2017-10` is specified on the command line.

``` yaml $(tag) == 'package-2017-10'
input-file:
- Microsoft.AlertsManagement/2017-10-10-privatepreview/AlertsManagement.json
```

---
## C# 

These settings apply only when `--csharp` is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.Management.AlertsManagement
  output-folder: $(csharp-sdks-folder)/AlertsManagement/Management.AlertsManagement/Generated
  clear-output-folder: true
```