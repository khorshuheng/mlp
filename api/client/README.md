# Go API client for client

API Guide for accessing MLP API

## Overview
This API client was generated by the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.  By using the [swagger-spec](https://github.com/swagger-api/swagger-spec) from a remote server, you can easily generate an API client.

- API version: 0.4.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.GoClientCodegen

## Installation
Put the package under your project folder and add the following in import:
```golang
import "./client"
```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8080/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ProjectApi* | [**ProjectsGet**](docs/ProjectApi.md#projectsget) | **Get** /projects | List existing projects
*ProjectApi* | [**ProjectsPost**](docs/ProjectApi.md#projectspost) | **Post** /projects | Create new project
*ProjectApi* | [**ProjectsProjectIdGet**](docs/ProjectApi.md#projectsprojectidget) | **Get** /projects/{project_id} | Get project
*ProjectApi* | [**ProjectsProjectIdPut**](docs/ProjectApi.md#projectsprojectidput) | **Put** /projects/{project_id} | Update project
*SecretApi* | [**ProjectsProjectIdSecretsGet**](docs/SecretApi.md#projectsprojectidsecretsget) | **Get** /projects/{project_id}/secrets | List secret
*SecretApi* | [**ProjectsProjectIdSecretsPost**](docs/SecretApi.md#projectsprojectidsecretspost) | **Post** /projects/{project_id}/secrets | Create secret
*SecretApi* | [**ProjectsProjectIdSecretsSecretIdDelete**](docs/SecretApi.md#projectsprojectidsecretssecretiddelete) | **Delete** /projects/{project_id}/secrets/{secret_id} | Delete secret
*SecretApi* | [**ProjectsProjectIdSecretsSecretIdPatch**](docs/SecretApi.md#projectsprojectidsecretssecretidpatch) | **Patch** /projects/{project_id}/secrets/{secret_id} | Update secret


## Documentation For Models

 - [Label](docs/Label.md)
 - [Project](docs/Project.md)
 - [Secret](docs/Secret.md)


## Documentation For Authorization

## Bearer
- **Type**: API key 

Example
```golang
auth := context.WithValue(context.Background(), sw.ContextAPIKey, sw.APIKey{
	Key: "APIKEY",
	Prefix: "Bearer", // Omit if not necessary.
})
r, err := client.Service.Operation(auth, args)
```

## Author



