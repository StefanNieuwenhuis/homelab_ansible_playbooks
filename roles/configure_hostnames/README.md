# Configure Hostnames

This role configures hostnames and updates `/etc/hosts` for all nodes in the `[cluster]` group.

## Features
- Sets system hostname from inventory variables.
- Updates 127.0.1.1 line in /etc/hosts with proper hostname.
- Adds an Ansible-managed block for all cluster nodes to /etc/hosts.

## Requirements
- Each host in the `[cluster]` group must define `hostname` and `fqdn` in `hosts.ini`.
