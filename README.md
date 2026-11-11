# EAAF · Enterprise Agentic AI Framework

EAAF gives enterprise applications a shared way to call AI models under their own access and usage policies. The Governance Gateway authenticates each application, enforces model permissions, quotas and simulated budgets, and records audit metadata. LiteLLM routes authorized requests to the configured provider.

[Visit the EAAF project portal](https://tandrian06.github.io/eaaf-project/)

## What you can try

### AI for Work · Chat and document search

Open the local chat portal and try the Global, HR, IT, and Marketing spaces. Department chat can retrieve excerpts from fictional documents and show the sources alongside the answer. Docker Compose runs the demo with a simulated provider. OpenAI is optional.

[Run Chat and RAG locally](https://github.com/tandrian06/eaaf#readme)

### AI for DevOps · Architecture to Terraform

Start with a reviewed YAML description of one HTTP container. The DevOps CLI reads the inputs and outputs of a prepared Terraform module, then generates the module call and its input values. You can validate the result locally. The deployment example adds a generated pull request and an optional AWS Fargate deployment.

[Explore the DevOps generator](https://github.com/tandrian06/eaaf-devops#readme) · [View the deployment example](https://github.com/tandrian06/eaaf-deployment-demo#readme) (GitHub access required while this repository is private)

## How the repositories fit together

| Repository | Responsibility |
| --- | --- |
| [EAAF Core](https://github.com/tandrian06/eaaf) | Shared model access and governance. It currently also hosts the local Chat and RAG demo. |
| [EAAF DevOps](https://github.com/tandrian06/eaaf-devops) | Reusable architecture intake, validation, and Terraform generation. Drafting from text can use the EAAF Gateway. |
| [EAAF Deployment Demo](https://github.com/tandrian06/eaaf-deployment-demo) | Example architecture, prepared Terraform module, generation workflow, and optional AWS deployment. |

## Portal source

This repository hosts the project website. Open [docs/index.html](docs/index.html) locally to preview it. GitHub Pages publishes the site from the `docs/` directory on `main`.
