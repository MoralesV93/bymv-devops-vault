# Vault Helm Chart Documentation

## Overview

This Helm chart deploys HashiCorp Vault on Kubernetes.

## Prerequisites

- Kubernetes 1.16+
- Helm 3.0+

## Installation

```bash
helm install vault ./helm/vault -n vault --create-namespace
```

## Configuration

Key configuration options in `values.yaml`:

- **replicaCount**: Number of Vault server replicas
- **image.tag**: Vault container image version
- **server.dataStorage**: Persistent volume size for data
- **storage.type**: Backend storage type (file, consul, etc.)
- **ingress.enabled**: Enable/disable ingress

## Usage

Port-forward to access Vault:

```bash
kubectl port-forward -n vault svc/vault 8200:8200
```

Then access at http://localhost:8200

## Uninstall

```bash
helm uninstall vault -n vault
```
