# Hello World Chromia Template

This repository is a Chromia Rell template project with a pre-configured environment for **GitHub Codespaces** and **Local Development** using Docker. It includes all necessary tools to start building on Chromia immediately.

## Quick Start

Use this repository as a template.

### Create your repository
Click **Use this template** and choose **Create a new repository** or **Open in a codespace**.

### Choose your development environment

#### GitHub Codespaces
Choose **Open in a codespace** to start a Codespace directly from this template.

#### Local Development
Prerequisites:
- [Docker](https://docs.docker.com/get-started/get-docker) must be installed and running.
- [VS Code](https://code.visualstudio.com/) with the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) installed.

Setup:
1. Clone your new repository locally.
2. Open the project folder in VS Code.
3. When prompted with **Reopen in Container**, click it. This builds and starts the development environment.

## Usage

Once your environment is ready, use the integrated terminal to run Chromia CLI (`chr`) commands.

### Run tests
```bash
chr test
```

### Build the project
```bash
chr build
```

## What's Included

The environment comes pre-installed with:

- Chromia CLI (`chr`) for project management, testing, and building.
- PMC (`pmc`) - the Chromia Project Management Console.
- Pre-configured PostgreSQL database backend.
- Rell extension for syntax highlighting and language support in VS Code.
- A standard project structure including:
  - `chromia.yml` (Project configuration)
  - `src/main.rell` (Hello World Rell module)
  - `src/test/` (Example tests)

## Resources
- [Chromia Documentation](https://docs.chromia.com/)
- [Rell Language Reference](https://docs.chromia.com/rell/)
- [Chromia CLI Reference](https://docs.chromia.com/dev-tools/cli/)
