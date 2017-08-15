# Data Factory

> see https://aka.ms/autorest

This is the AutoRest configuration file for Data Factory.



---
## Getting Started
To build the SDK for Sql, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`
---

## Configuration



### Basic Information
These are the global settings for the Data Factory API.

``` yaml
title: DataFactoryManagementClient
description: The Azure Data Factory management API provides a RESTful set of web services that interact with Azure Data Factory services.
openapi-type: arm
tag: package-2017-03-preview
```


### Tag: package-2017-03-preview

These settings apply only when `--tag=package-2017-03-preview` is specified on the command line.

``` yaml $(tag) == 'package-2017-03-preview'
input-file:
- Microsoft.DataFactory/2017-03-01-preview/datafactory.json
```
