# Distribute Kubernetes Configuration files for authentication

This role distributes Kubernetes Configuration files for authentication to `server` and `worker` nodes.

## Features
- Distribute generated Kubeconfigs to `server` node(s).
- Distribute generated Kubeconfigs to `worker` node(s).

## Requirements
- Operational `ssh` connection to server and worker nodes.
- For worker node(s): `{{host}}.kubeconfig` & `kube-proxy.kubeconfig` are generated and available for copy.
- For server node(s): `admin.kubeconfig`, `kube-proxy.kubeconfig`, `kube-controller-manager.kubeconfig` & `kube-scheduler.kubeconfig` are generated and available for copy.
