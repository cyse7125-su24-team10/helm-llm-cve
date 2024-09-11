# helm-llm-cve

This Helm chart deploys the `llm-cve` application, which integrates a large language model (LLM) for processing CVE data.

## Prerequisites

- Kubernetes 1.16+
- Helm 3.0+
- Docker registry credentials (e.g., Docker Hub PAT)
- Configured API keys for Groq and Pinecone services

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/cyse7125-su24-team10/helm-llm-cve.git
cd helm-llm-cve
```


### 2. Installing the Chart

Make sure to update secretes in values.yaml file, to install the chart with the release name `llm-cve`:

```bash
helm install llm-cve ./ -n llm-cve
```