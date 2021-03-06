| :mega: Do not use for Production |
|----------------------------------|
| This Docker image was quickly created based on the official documentation in order to run on Azure Container Instances. Do not run this in production environments.        |

# Azure DevOps Agent running in Docker
Docker image running the Azure DevOps Agent based on [official docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops).

[![Deploy to Azure](https://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/?repository=https://github.com/tomkerkhove/azure-devops-agent-in-docker)

## Running agent in Docker

```shell
⚡ tkerkhove@tomkerkhove C:\azure-devops-agent-in-docker
❯  docker run -e AZP_URL="https://dev.azure.com/{org}" -e AZP_TOKEN="{PAT token}" -e AZP_POOL="{pool name}" -e AZP_AGENT_NAME="{agent name}" tomkerkhove/azure-devops-agent:ubuntu-1604
```
