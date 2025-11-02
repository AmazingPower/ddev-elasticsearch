[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/AmazingPower/ddev-elasticsearch/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/AmazingPower/ddev-elasticsearch/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/AmazingPower/ddev-elasticsearch)](https://github.com/AmazingPower/ddev-elasticsearch/commits)
[![release](https://img.shields.io/github/v/release/AmazingPower/ddev-elasticsearch)](https://github.com/AmazingPower/ddev-elasticsearch/releases/latest)

# DDEV Elasticsearch

## Overview

This add-on integrates Elasticsearch into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get AmazingPower/ddev-elasticsearch
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Elasticsearch |
| `ddev logs -s elasticsearch` | Check Elasticsearch logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.elasticsearch --elasticsearch-docker-image="ddev/ddev-utilities:latest"
ddev add-on get AmazingPower/ddev-elasticsearch
ddev restart
```

Make sure to commit the `.ddev/.env.elasticsearch` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `ELASTICSEARCH_DOCKER_IMAGE` | `--elasticsearch-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@AmazingPower](https://github.com/AmazingPower)**
