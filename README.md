EmPOWER: Mobile Networks Operating System
=========================================

### What is EmPOWER?
EmPOWER is a new network operating system designed for heterogeneous mobile networks.

### Top-Level Features
* Supports both LTE and WiFi radio access networks
* Northbound abstractions for a global network view, network graph, and
  application intents.
* REST API and native (Python) API for accessing the Northbound abstractions
* Support for Click-based Lightweight Virtual Networks Functions
* Declarative VNF chaning on precise portion of the flowspace
* Flexible southbound interface supporting WiFi APs LTE eNBs

Checkout out our [website](http://empower.create-net.org/) and our [wiki](https://github.com/5g-empower/empower-runtime/wiki)

This repository includes the EmPOWER packages for OpenWRT 15.05.01.

Code is released under the Apache License, Version 2.0.

### How to install

```
  $: cd $TOPDIR
  $: echo 'src-git empower https://github.com/5g-empower/empower-openwrt-packages-15.05.git' >> feeds.conf.default
  $: ./scripts/feeds update empower
  $: ./scripts/feeds install -a -p empower
  $: make menuconfig
  $: select Network -> empower-agent
```
