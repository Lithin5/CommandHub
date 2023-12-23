# Kubernetes Basic Commands

This file contains a list of basic Kubernetes commands to help you get started with container orchestration.

## Table of Contents
- [Check Kubernetes Version](#check-kubernetes-version)
- [Deploy an Application](#deploy-an-application)
- [List Pods](#list-pods)
- [Get Pod Information](#get-pod-information)
- [Delete a Pod](#delete-a-pod)
- [Expose an Application](#expose-an-application)
- [Scale an Application](#scale-an-application)
- [View Cluster Information](#view-cluster-information)

### Check Kubernetes Version

```bash
kubectl version
```

### Deploy an Application

```bash
kubectl create deployment <deployment_name> --image=<image_name>
```

### List Pods

```bash
kubectl describe pod <pod_name>
```

### Delete a Pod

```bash
kubectl delete pod <pod_name>
```

### Expose an Application

```bash
kubectl expose deployment <deployment_name> --type=NodePort --port=<port_number>
```

### Scale an Application

```bash
kubectl scale deployment <deployment_name> --replicas=<number_of_replicas>
```

