[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/armin-runggaldier/ddev-scalar/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/armin-runggaldier/ddev-scalar/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/armin-runggaldier/ddev-scalar)](https://github.com/armin-runggaldier/ddev-scalar/commits)
[![release](https://img.shields.io/github/v/release/armin-runggaldier/ddev-scalar)](https://github.com/armin-runggaldier/ddev-scalar/releases/latest)

# DDEV Scalar

## Overview

This add-on integrates Scalar into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get armin-runggaldier/ddev-scalar
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Scalar |
| `ddev logs -s scalar` | Check Scalar logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.scalar --scalar-docker-image="busybox:stable"
ddev add-on get armin-runggaldier/ddev-scalar
ddev restart
```

Make sure to commit the `.ddev/.env.scalar` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `SCALAR_DOCKER_IMAGE` | `--scalar-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@armin-runggaldier](https://github.com/armin-runggaldier)**
