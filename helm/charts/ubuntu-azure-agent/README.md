# ubuntu-azure-agent

## Introduce

The chart deploy a pool of Azure agents.

## Treat with it

Now I just accomplished with ARM platform. The AMD will coming soon.

### Install chart

```bash
    export IMAGE_REPOSITORY=docker.io/bigcat3997/ubuntu-azure-agent
    export IMAGE_TAG=1.0.9-arm64
    export AZP_URL=<BASE64_AZP_URL>
    export AZP_POOL=<BASE64_AZP_POOL>
    export AZP_TOKEN=<BASE64_AZP_TOKEN>

    helm install ubuntu-azure-agent ubuntu-azure-agent \
        --set image.repository=$IMAGE_REPOSITORY \
        --set image.tag=$IMAGE_TAG \
        --set secret.data.AZP_URL=$AZP_URL \
        --set secret.data.AZP_POOL=$AZP_POOL \
        --set secret.data.AZP_TOKEN=$AZP_TOKEN
```
