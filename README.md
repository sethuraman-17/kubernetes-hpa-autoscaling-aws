# Auto-Scaling Web Application using Kubernetes HPA on AWS EC2

## Overview

Production-oriented Kubernetes project demonstrating automatic horizontal scaling of an NGINX web application using Kubernetes Horizontal Pod Autoscaler (HPA).

## Architecture

AWS EC2
→ Kubernetes Cluster
→ NGINX Deployment
→ Kubernetes Service
→ Ingress
→ Metrics Server
→ HPA

## HPA Configuration

- Target CPU: 50%
- Minimum replicas: 2
- Maximum replicas: 10
- CPU request: 100m
- CPU limit: 250m
- Memory request: 128Mi
- Memory limit: 256Mi

## Scaling Demonstration

The application successfully demonstrated:

2 → 4 → 6 → 8 replicas during scale-up.

After workload reduction:

8 → 2 replicas during scale-down.

## Technologies

- AWS EC2
- Kubernetes
- Docker
- NGINX
- Metrics Server
- Kubernetes HPA
- Ingress
- Calico

## Project Structure

```text
kubernetes-hpa-autoscaling-aws/
├── README.md
├── manifests/
├── screenshots/
└── docs/
