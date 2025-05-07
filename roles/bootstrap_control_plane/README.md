# Bootstrap Kubernetes Control Plane

This role bootstraps the Kubernetes control plane. The following components will be installed on the server machine: Kubernetes API Server, Scheduler, and Controller Manager.

## Features
- Generate the encryption config file.
- Distribute the encryption config file to each controller instance.

## Requirements
- Operational `ssh` connection to server nodes.
- For each controller instance: `encryption-config.yaml` is generated and available for copy.
