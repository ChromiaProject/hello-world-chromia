# Hello World Chromia Template

This repository is a Chromia Rell template project with a pre-configured Docker and devcontainer environment.

## Pre-configured environment with Docker

This setup provides a fully pre-configured development environment using Docker and dev containers, so you do not need
to manually install and configure the individual Chromia components.

### Prerequisites

Before starting, make sure you have the following installed on your machine:

- [Docker](https://docs.docker.com/get-started/get-docker): must be installed and running
- VS Code or a VS Code-based IDE such as Cursor or Windsurf
- Dev Containers extension:
  [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## Quick Start

### Open the project

Clone this repository, then open the project folder in VS Code.

When VS Code detects the devcontainer configuration, it will suggest reopening the folder in a container. Choose
**Reopen in Container** to:

- Build and start the development container
- Install the required dependencies
- Configure the development environment
- Provide access to the Chromia development tools

Once the devcontainer is running, you can use the integrated terminal in VS Code to run Chromia CLI commands such as
`chr test` and `chr build`.

## Create a GitHub Codespace

You can also create a Codespace directly from the repo.

### Recommended flow

1. Click **Code**.
2. Select the **Codespaces** tab.
3. Click **Create codespace on main**.

GitHub will build the dev container automatically and open the project in a cloud-based development environment with the
same tools and configuration included in this template.

## What's included

The dev container environment comes pre-configured with:

- Rell VS Code extension
- PostgreSQL
- Chromia CLI
- PMC
- Proper environment configuration

## Template contents

This template includes:

- `chromia.yml` for Chromia project configuration
- `src/main.rell` with a simple Hello World example
- `src/test/` with example Rell tests
- `.devcontainer/` with a ready-to-use development container setup
