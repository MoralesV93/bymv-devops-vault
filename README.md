# BYMV DevOps Vault

Comprehensive Vault server configuration and deployment using Helm charts.

## Overview

This repository contains:
- Helm charts for Vault server deployment
- Configuration templates
- Deployment scripts and documentation

## Structure

```
.
├── helm/
│   └── vault/
│       ├── Chart.yaml
│       ├── values.yaml
│       ├── templates/
│       └── charts/
├── docs/
├── scripts/
└── README.md
```

## Quick Start

### Prerequisites
- Kubernetes cluster (1.16+)
- Helm 3.0+

### Deployment

```bash
helm install vault ./helm/vault
```

## Documentation

See [docs](./docs) directory for detailed documentation.

## License

Proprietary
