# Docker Azure DevOps Agent (Linux)

This is the Dockerfile and associated assets requried to run the Terraform CI/CD and subscription creation pipelines.

To run standalone:

```bash
docker run -e AZP_URL=<Azure DevOps instance> -e AZP_TOKEN=<PAT token> -e AZP_AGENT_NAME=mydockeragent myrepo/myimage:latest
```
