---
title: "Kubectl"
date: 2023-05-21T12:35:04
draft: false
author: Thomas Panzeri
---

## Basic Commands

| Command                       | Description                                      |
| ----------------------------- | ------------------------------------------------ |
| `kubectl get pods`            | List all pods in the current namespace           |
| `kubectl get deployments`     | List all deployments in the current namespace    |
| `kubectl get services`        | List all services in the current namespace       |
| `kubectl get nodes`           | List all nodes in the cluster                    |
| `kubectl create <resource>`   | Create a resource (e.g., pod, deployment)         |
| `kubectl delete <resource>`   | Delete a resource (e.g., pod, deployment)         |
| `kubectl describe <resource>` | Get detailed information about a resource        |
| `kubectl logs <pod>`          | View the logs of a pod                           |
| `kubectl exec <pod> <command>`| Execute a command in a running pod               |
| `kubectl apply -f <file>`     | Apply a configuration file                       |
| `kubectl port-forward <pod> <port>` | Forward a local port to a pod               |
| `kubectl scale <resource> --replicas=<count>` | Scale a resource to a specified number of replicas |

## Advanced Commands

| Command                              | Description                                                  |
| ------------------------------------ | ------------------------------------------------------------ |
| `kubectl create secret`               | Create a secret from literal values or a file                |
| `kubectl get <resource> -o yaml`      | Get the YAML representation of a resource                    |
| `kubectl edit <resource>`             | Edit a resource in a text editor                             |
| `kubectl rollout <resource>`          | Manage rollouts and rollbacks for a resource                 |
| `kubectl explain <resource>`          | Get detailed information about a resource type               |
| `kubectl top <resource>`              | Display resource usage (CPU/memory)                           |
| `kubectl cluster-info`                | Display cluster information                                  |
| `kubectl config view`                 | View the current Kubernetes configuration                    |
| `kubectl apply --dry-run -f <file>`   | Dry run to see what resources would be created or modified    |
| `kubectl proxy`                       | Start a proxy to the Kubernetes API server                    |
| `kubectl create ns <namespace>`       | Create a new namespace                                       |
| `kubectl config use-context <context>`| Set the current context in the kubeconfig file                |
| `kubectl exec -it <pod> -- /bin/bash` | Open an interactive shell inside a pod                       |

## Additional Resources

- Official kubectl Documentation: [kubectl Cheat Sheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
- Kubernetes Reference Documentation: [Kubernetes Documentation](https://kubernetes.io/docs/home/)
