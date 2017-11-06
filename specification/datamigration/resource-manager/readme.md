# Data Migration Service
    
> see https://aka.ms/autorest

This is the AutoRest configuration file for Data Migration Service.

The Data Migration RP comprises of APIs that enable a customer to manage the service instances that help migrate databases from a source to target.

---

## Getting Started 
To build the SDK for Compute, simply [Install AutoRest](https://aka.ms/autorest/install) and in this folder, run:

> `autorest`

To see additional help and options, run:

> `autorest --help`

---

## Configuration

### Basic Information 
These are the global settings for the Data Migration Service API.

``` yaml
title: DataMigrationManagementClient
description: Data Migration Client
openapi-type: arm
tag: package-2017-04-privatepreview
```

### Tag: package-2017-04-privatepreview

These settings apply only when `--tag=package-2017-04-privatepreview` is specified on the command line.

``` yaml $(tag) == 'package-2017-04-privatepreview'
input-file:
- Microsoft.DataMigration/2017-04-15-privatepreview/datamigration.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/Common.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToSourceMySqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToSourceOracleTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToSourceSqlServerTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToTargetAnySqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToTargetCloudDbTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToTargetSqlDbTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ConnectToTargetSqlServerTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/GetProjectDetailsMySqlSqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/GetProjectDetailsOracleSqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/GetUserTablesSqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrateMySqlSqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrateOracleSqlTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrateSqlServerCloudDbTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrateSqlServerSqlDbTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrateSqlServerSqlServerTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/Projects.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/Services.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/Tasks.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/TasksCommon.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ValidateMigrationInputSqlServerCloudDbTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/ValidateMigrationInputSqlServerSqlServerTask.json
- Microsoft.DataMigration/2017-04-15-privatepreview/definitions/MigrationValidation.json
```

``` yaml $(tag) == 'package-2017-11-15-preview'
input-file:
- Microsoft.DataMigration/2017-11-15-preview/datamigration.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/Common.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/ConnectToSourceSqlServerTask.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/ConnectToTargetSqlDbTask.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/GetUserTablesSqlTask.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/MigrateSqlServerSqlDbTask.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/Projects.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/Services.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/Tasks.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/TasksCommon.json
- Microsoft.DataMigration/2017-11-15-preview/definitions/MigrationValidation.json
```
---

# Code Generation

## C#

These settings apply only when --csharp is specified on the command line.
Please also specify `--csharp-sdks-folder=<path to "SDKs" directory of your azure-sdk-for-net clone>`.

``` yaml $(csharp)
csharp:
  azure-arm: true
  license-header: MICROSOFT_MIT_NO_VERSION
  namespace: Microsoft.Azure.Management.DataMigration
  output-folder: $(csharp-sdks-folder)/DataMigration/Management.DataMigration/Generated
  clear-output-folder: true
```

## Python

These settings apply only when `--python` is specified on the command line.

``` yaml $(python)
python:
  azure-arm: true
  output-folder: $(output-folder)Generated/Python
  license-header: MICROSOFT_MIT_NO_VERSION
  payload-flattening-threshold: 2
  namespace: azure.mgmt.datamigration
```