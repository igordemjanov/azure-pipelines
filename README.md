# Build Pipelines
## Description 
This repository contains Build templates, often referred as 'Continuous Integration' (CI) pipelines, and these templates are defined in YAML format. Description about each job template is listed below with its input parameters and tasks.

## Templates
### .NET Core Application
#### Description
This job template runs build, test and publish of .NET Core application based on the provided parameters.

#### Tasks included
- [.NET Core CLI (restore, build, test, publish)](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/build/dotnet-core-cli?view=azure-devops)
- [Publish Pipeline Artifact](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/publish-pipeline-artifact?view=azure-devops)

#### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job. |
| display_name | Display name of the job. |
| project_title | Title of the project. |
| artifact_name | Name of the artifact to publish as output of the build job. |

## Archieve Files
#### Description
This job template archives files based on the provided parameters.

### Tasks included
- [Archive Files](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/archive-files?view=azure-devops)
- [Publish Pipeline Artifact](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/publish-pipeline-artifact?view=azure-devops)

### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job. |
| display_name | Display name of the job. |
| project_title | Title of the folder that contains files to be archived. |
| artifact_name | Name of the artifact to publish as output of the build job. |

## Angular Application
#### Description
This job template runs lint, build, test and publish of Angular application based on the provided parameters.

### Tasks included
- [Npm (ci, lint, build, test)](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/package/npm?view=azure-devops)
- [Archive Files](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/archive-files?view=azure-devops)
- [Publish Test Results](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/test/publish-test-results?view=azure-devops&tabs=yaml)
- [Publish Code Coverage Results](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/test/publish-code-coverage-results?view=azure-devops)
- [Publish Pipeline Artifact](https://docs.microsoft.com/en-us/azure/devops/pipelines/tasks/utility/publish-pipeline-artifact?view=azure-devops)

### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job. |
| display_name | Display name of the job. |
| project_title | Title of the project. |
| artifact_name | Name of the artifact to publish as output of the build job. |
