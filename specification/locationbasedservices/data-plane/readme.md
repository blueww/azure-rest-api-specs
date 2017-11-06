# LocationBasedServices
    
> see https://aka.ms/autorest

Configuration for generating Entity Search SDK.

The current release is `release_1_0`.

``` yaml
tag: release_1_0
openapi-type: data-plane
```
### Tag: Release 1.0
These settings apply only when `--tag=release_1_0` is specified on the command line.

``` yaml $(tag) == 'release_1_0'
input-file: Microsoft.LocationBasedServices/1.0/lbs.json
```

## CSharp Settings
These settings apply only when `--csharp` is specified on the command line.
``` yaml $(csharp) 
csharp: 
  license-header: MICROSOFT_MIT_NO_VERSION
  azure-arm: false
  namespace: Microsoft.LocationBasedServices
  output-folder: $(csharp-sdks-folder)/LocationBasedServices/Generated
  clear-output-folder: true
```


