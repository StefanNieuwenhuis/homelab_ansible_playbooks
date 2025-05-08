# Bootstrap Kubernetes Worker Nodes

This role bootstraps the Kubernetes worker nodes. The following components will be installed: runc, container networking plugins, containerd, kubelet, and kube-proxy.

## Features
-

## Requirements
-

## Verification

```sh
ssh root@server \
  "kubectl get nodes \
  --kubeconfig admin.kubeconfig"
```

```sh
NAME     STATUS   ROLES    AGE    VERSION
node-0   Ready    <none>   1m     v1.32.3
node-1   Ready    <none>   10s    v1.32.3
```
