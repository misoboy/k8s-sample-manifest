# sample-manifest

> Kubernetes deployment manifest samples used as a reference for demo application deployments in CI/CD pipelines.

[![Kubernetes](https://img.shields.io/badge/Kubernetes-manifests-326CE5?logo=kubernetes&logoColor=white)](https://kubernetes.io)
[![YAML](https://img.shields.io/badge/YAML-config-CB171E)](https://yaml.org)

## Overview

A collection of Kubernetes manifest files for deploying a sample Spring Boot application. Used as the **manifest repository** in a GitOps-style pipeline where CI (Jenkins/GitHub Actions) updates image tags and CD (Kubernetes) applies the changes.

## Usage

Apply all manifests:

```bash
kubectl apply -f .
```

Or apply individually:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml
```

## Related

- [sample-github-action](https://github.com/misoboy/sample-github-action) — The application that deploys using these manifests

## License

MIT

