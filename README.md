# Build Pipelines
## Description 
This repository contains Build templates, often referred as 'Continuous Integration' (CI) pipelines, and these templates are defined in YAML format. Description about each job template is listed below with its input parameters and tasks.

## Templates
### .NET Core Package
#### Tasks included
- Perform Restore
- Perform Build
- Perform Test
- Publish Package
- Publish Pipeline Artifact

#### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job |
| display_name | Display name of the job |
| pool | Name of the Agent (more info [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/pools-queues?view=azure-devops&tabs=yaml)) |
| project_title | Title of the project |
| artifcat_name | Name of the artifact to publish as output of the build job |

## Zip Package
### Tasks included
- Archive files
- Publish Pipeline Artifact

### Parameters
| Parameter | Description |
|--|--|
| name | Internal name of the job. |
| display_name | Display name of the job |
| pool | Name of the Agent (more info [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/pools-queues?view=azure-devops&tabs=yaml)) |
| project_title | Title of the project |
| artifcat_name | Name of the artifact to publish as output of the build job |