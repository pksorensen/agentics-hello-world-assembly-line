# Agentics Hello World Assembly Line

A minimal public assembly line for testing the complete Agentics flow:

1. Import this repository into an Agentics project.
2. Create the prefilled task.
3. A managed runner starts one Azure Container Apps Sandbox.
4. The station runs inside its devcontainer and commits `HELLO.md`.
5. The Sandbox is removed after the job completes.

The expected result is:

```text
hello from agentics
execution: azure-sandbox
```
