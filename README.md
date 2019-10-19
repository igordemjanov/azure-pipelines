# Build Pipelines
## Description 
This repository contains Build templates, often referred as 'Continuous Integration' (CI) pipelines, and these templates are defined in YAML format. Description about each job template is listed below with its input parameters and tasks.

## Templates
### .NET Core Package
#### Description
This job template runs build, test and publish of .Net Core project based on the provided parameters.

#### Tasks included
- [.NET Core CLI (restore, build, test, publish)](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/build/dotnet-core-cli?view=azure-devops)

- [Publish Pipeline Artifact](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/publish-pipeline-artifact?view=azure-devops)

#### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job |
| display_name | Display name of the job |
| pool | Name of the Agent (more info [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/pools-queues?view=azure-devops&tabs=yaml)) |
| project_title | Title of the project |
| artifcat_name | Name of the artifact to publish as output of the build job |

## Zip Package
#### Description
This job template archives files based on the provided parameters.

### Tasks included
- [Archive files](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/archive-files?view=azure-devops)
- [Publish Pipeline Artifact](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/publish-pipeline-artifact?view=azure-devops)

### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job. |
| display_name | Display name of the job |
| pool | Name of the Agent (more info [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/pools-queues?view=azure-devops&tabs=yaml)) |
| project_title | Title of the project |
| artifcat_name | Name of the artifact to publish as output of the build job |