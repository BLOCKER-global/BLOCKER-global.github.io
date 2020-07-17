---
layout: default
title: Ecosystem
nav_order: 2
description: "The BLOCKER Ecosystem"
permalink: /ecosystem
last_modified_date: 2020-04-27T17:54:08+0000
---

# Ecosystem

## The BLOCKER `engine`
###### API domain:   `engine.blocker.global`
The `engine` is the core daemon `server` which services instantiation of your `Blockerfile`

Retrieve your provisioned containers from the cloud daemon (comparable to `dockerd` running on your computer,
`blockerd` runs distributed in Cloud Native)

`$ blocker container ls`

## BlockerHub
###### API domain:   `hub.blocker.global`

BlockerHub is the primary consumer facing `client` and social hub.

+ Dashboard
    + Telemetry
    + Anonymized proximal data  (feedback for module contributors)
+ Builder
    + Pick and choose contributed `Mods` to drop into your projects.
        + Continuously generates `Blockerfiles` for your build.
        + Racks up a `Cost` to deploy a given `solution` which is based on the logistics cost provided by the core BLOCKER `engine`
+ Browser (the social platform - similar to "Thingiverse", "Pinterest", "instagram")
    + Browse through other users projects.
        + Instantiate public projects yourself.

# `Blockernetes`

`Blockernetes` is our fork of Kubernetes

`Blockernetes` and `blocker` CLI clients are for power users.

Need to host emergency response medical service with high redundancy?  Provision autohealing clusters to disaster response.
If services die containers and mods can be auto deployed by the blocker `engine` through the use of `Blockernetes`

+ blockctl  ( our fork of Kubernetes for orchestrating Blockerfiles )
+ Blocker build

###### Reference: Kubernetes to Blockernetes

| Kubernetes | Blockernetes | Description |
|------------|--------------| ----------- |
| Pod        | Mod          | Atomic logical collection of functionality which has been "blockerized" by contributors |
| Node       | Abode        | A physical container in which modules are installed |
| Svc        | Svc          | A service rendered by one or more Pods/Mods |
| Deploy     | Deploy       | A deploment is a description |

Get BLOCKs 
```bash
$ blockctl get blocks
```

Get services 
```bash
$ blockctl get svc
```





{: .fs-6 .fw-300 }

[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 }
