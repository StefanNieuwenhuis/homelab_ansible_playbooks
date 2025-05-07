# Generate Kubernetes Configuration files for authentication

This role generates [Kubernetes client configuration files](https://kubernetes.io/docs/concepts/configuration/organize-cluster-access-kubeconfig/) (`kubeconfigs`), which configure Kubernetes clients to connect and authenticate to Kubernetes API Servers.

## Features

- Generate kubeconfig files for the `kubelet` and the `admin` user.
- Generate a kubeconfig file for the `kube-proxy` service.
- Generate a kubeconfig file for the `kube-controller-manager` service.
- Generate a kubeconfig file for the `kube-scheduler` service.
- Distribute the `kubelet` and `kube-proxy` kubeconfig files to the `worker` nodes.
- Distribute the `kube-controller-manager` and `kube-scheduler` kubeconfig files to the `server` machine.

## Requirements

- Operational `ssh` connection to server and worker nodes.
