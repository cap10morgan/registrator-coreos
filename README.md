# Registrator on CoreOS

This is a fleet service file for running [Registrator](https://github.com/progrium/registrator) on CoreOS.

## Requirements

This runs Registrator in a Consul-backed configuration. The easiest way to get that running on your CoreOS cluster is to use [consul-coreos](https://github.com/cap10morgan/consul-coreos).

Registrator also supports etcd (included with CoreOS), but it doesn't support features like health checks.

## Usage

```
fleetctl submit registrator.service
fleetctl start registrator
```
