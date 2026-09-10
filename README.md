# Agentics Hello World Assembly Line

A minimal public three-station assembly line for testing the complete Agentics flow:

1. Import this repository into an Agentics project.
2. Create the prefilled task.
3. The task moves automatically through `Plan`, `Build`, and `Verify`.
4. A managed runner starts an Azure Container Apps Sandbox for each station job.
5. Each station runs inside its devcontainer and commits one artifact.
6. Each Sandbox is removed after its station job completes.

The expected result is:

```text
agentics-hello-world: passed
stations: plan -> build -> verify
execution: azure-sandbox
```
