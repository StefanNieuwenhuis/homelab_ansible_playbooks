# Add Host Entries to jumpbox, server and worker nodes

This role generates a hosts file which will be appended to `/etc/hosts` on the jumpbox and to all cluster members This will allow each machine to be reachable using a hostname such as `server`, `node-0`, or `node-1`.

## Features
- Generate a Hosts Lookup Table
- Add `/etc/hosts` entries to `jumpbox`
- Add `/etc/hosts` entries to all cluster members

## Requirements
- Each host in the `[cluster]` group must define `hostname` and `fqdn` in `hosts.ini`.
