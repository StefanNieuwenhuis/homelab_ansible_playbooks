# Provision TLS Certificates

This role provisions a [PKI Infrastructure](https://en.wikipedia.org/wiki/Public_key_infrastructure) using `openssl` to bootstrap a Certificate Authority, and generate TLS certificates for the following components: `kube-apiserver`, `kube-controller-manager`, `kube-scheduler`, `kubelet`, and `kube-proxy`.

## Features
- Generate the CA configuration file, certificate, and private key
- Create Client and Server Certificates
- Distribute the Client and Server Certificates

## Requirements
- Each host in the `[cluster]` group must define `hostname` and `fqdn` in `hosts.ini`.
