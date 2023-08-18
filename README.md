# Serverless - Azure Function with GO - Type: queueTrigger

This repo is just to learn the Serverless GO with Azure

## Guide - VSCode

1. Install Azure Function extension
2. Azure tab -> Workspace -> Create Project -> Create Function
3. Select a folder, usually your current folder.
4. In Select a language, select Custom Handler.
5. In Select a template for your first function, select QueuTrigger.
6. Give the app a name, such as queueTrigger.
7. Select an authorization level of anonymous. You can change that later if you want.

## Run the app

```shell
go build server.go
```

- Then update `defaultExecutablePath` in `host.json`
- Update `local.settings.json` with `"AzureWebJobsStorage": "UseDevelopmentStorage=true",`
- Start Azurite Queue Service in VSCode using command pallet
- Download and Start [Azure Storage Explorer](https://azure.microsoft.com/en-in/products/storage/storage-explorer/)
- Once done, start func for local testing

```shell
func start
```
