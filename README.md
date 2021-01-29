# Docker Azure DevOps Terraform Agent (Linux)

This is the Dockerfile and associated assets requried to run the Terraform CI/CD and subscription creation pipelines.

Container image containing:

* [Terraform](https://github.com/hashicorp/terraform)
* [tflint](https://github.com/terraform-linters/tflint)
* [tfline azurerm ruleset](https://github.com/terraform-linters/tflint-ruleset-azurerm)
* [az cli](https://github.com/Azure/azure-cli)

## Agent installation

This is handled at runtime, using the `start.sh` is taken from the [official docs](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops).

## Environment Variables

See [here](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops#environment-variables)

## To run standalone

```bash
docker run -e AZP_URL=<Azure DevOps instance> -e AZP_TOKEN=<PAT token> -e AZP_AGENT_NAME=mydockeragent myrepo/myimage:latest
```
