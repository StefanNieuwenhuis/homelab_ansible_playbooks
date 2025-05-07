# Generating Data Encryption Config and Key

This role generates an encryption key and an encryption config suitable for encrypting Kubernetes Secrets.

## Features
- Generate the encryption config file.
- Distribute the encryption config file to each controller instance.

## Requirements
- Operational `ssh` connection to server nodes.
- For each controller instance: `encryption-config.yaml` is generated and available for copy.
