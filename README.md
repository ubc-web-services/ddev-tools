[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/ubc-web-services/ddev-tools/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/ubc-web-services/ddev-tools/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/ubc-web-services/ddev-tools)](https://github.com/ubc-web-services/ddev-tools/commits)
[![release](https://img.shields.io/github/v/release/ubc-web-services/ddev-tools)](https://github.com/ubc-web-services/ddev-tools/releases/latest)

# DDEV Tools

## Overview

This add-on integrates Tools into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get ubc-web-services/ddev-tools
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Tools |
| `ddev logs -s tools` | Check Tools logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.tools --tools-docker-image="ddev/ddev-utilities:latest"
ddev add-on get ubc-web-services/ddev-tools
ddev restart
```

Make sure to commit the `.ddev/.env.tools` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `TOOLS_DOCKER_IMAGE` | `--tools-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@ubc-web-services](https://github.com/ubc-web-services)**
