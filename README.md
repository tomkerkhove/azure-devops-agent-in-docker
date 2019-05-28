# Azure DevOps Agent running in Docker
Docker image running the Azure DevOps Agent based on [official docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops).

## Running agent in Docker

```shell
⚡ tkerkhove@tomkerkhove C:\azure-devops-agent-in-docker
❯  docker run -e AZP_URL="https://dev.azure.com/{org}" -e AZP_TOKEN="{PAT token}" -e AZP_POOL="{pool name}" -e AZP_AGENT_NAME="{agent name}" tomkerkhove/azure-devops-agent:ubuntu-1604
```