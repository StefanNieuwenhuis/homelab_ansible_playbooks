# Distribute TLS Certificates

This role distributes TLS certificates to `server` and `worker` nodes.

## Features
- Distribute generated TLS certificates to `server` node(s).
- Distribute generated TLS certificates to `worker` node(s).

## Requirements
- Operational `ssh` connection to server and worker nodes.
- For worker node(s): `ca.crt`, `{{host}}.crt` & `{{host}}.key` are generated and available for copy.
- For server node(s): `ca.key`, `ca.crt`, `kube-api-server.key`, `kube-api-server.crt`, `service-accounts.key` & `service-accounts.crt` are generated and available for copy.
