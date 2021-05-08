# Auditbeat

[Auditbeat](https://www.elastic.co/guide/en/beats/auditbeat/current/index.html) is a lightweight shipper to audit the activities of users and processes on your systems, so that you can identify potential security policy violations. You can use Auditbeat to collect audit events from the Linux Audit Framework. You can also use Auditbeat for file integrity check, that is to detect changes to critical files, like binaries and configuration files.

## Introduction

This chart deploys auditbeat agents to all the nodes in your cluster via a DaemonSet.

By default this chart only ships a single output to a file on the local system.  Users should set config.output.file.enabled=false and configure their own outputs as [documented](https://www.elastic.co/guide/en/beats/auditbeat/current/configuring-output.html)

## Prerequisites

-   Kubernetes 1.9+
