# Distribute SSH Keys to server and worker nodes

This role generates and distributes an SSH keypair to the server and worker machines, which will be used to run commands on those machines.

## Features
- Generate a new SSH Key
- Copy the SSH public key to each machine
- Verify SSH public key access is working

## Requirements
- Each host in the `[cluster]` group must define `hostname` and `fqdn` in `hosts.ini`.
