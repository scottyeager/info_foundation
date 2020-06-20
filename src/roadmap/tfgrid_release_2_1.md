# TFGrid release 2.1

![](./img/roadmap.png)

- [details on github of the project](https://github.com/orgs/threefoldtech/projects/93)

## high lights

- resource pool reservation
    - reservation is now for capacity only
    - this is a super important feature to allow to reserve a pool of capacity, pricing is adjusted in relation to duration of the reservation.
    - deployment of a workload happens as part of a reservation
    - as long as there is available capacity in the reservation a workload can be stopped, started, ...
    - this allows flexibility around doing live cycle management of apps
- support for farming on IPv4 networks (using an IPv6 overlay networking technology, probably [yggdrasil](https://yggdrasil-network.github.io/))
- building of applications directly on the TFGrid
    - mechanism with example to show how continuous integration can be done on the TFGrid without having to use docker on your own computer
    - the result is a flist, which is the low level description of the IT workload which can be started as a container inside a resource pool reservation (see above)
- 0-stor web frontend for machines (REST)
    - HTTP REST & SSH based front end on top of the 0-Stor
    - allows anyone to easily store large amounts of data on top of 0-Stor using our distributed storage algorithm.
- [S3 storage improvements](https://github.com/threefoldtech/home/issues/720)
    - monitoring integration
    - users can make the S3 solution self healing if required (experts only)
- lots of small fixes
    - bug fixes, maintenance, ...


## components used

Below are linked to some main component projects

- ZeroOS 0.4 (is a 2.x release, but golang forces the 0.4 nr) = our operating system
- [Jumpscale 10.7](https://github.com/orgs/threefoldtech/projects/91) = our automation framework


## maybe (not guaranteed)

- build in support for hypercore/ipfs, basically allow IPFS or HyperDrive to connect to our storage backend, this way our more robust reliable storage system can be a backend for these known P2P storage mechanisms without loosing data ownership properties.

## timing & release plan

release to public

- mid June 2020 we will release a ```release candidate of TFGrid 2.1.0 beta``` on branch development for 3sdk
    - jumpscale stays on development !!! for 1-2 weeks till full stability, but everyone in field can play with it
    - zos needs to be upgraded in the field to 0.4 before its usable
- we will keep this RC active on that branch until we get confirmation from field that this release is at least as stable as current 2.x one.
- mid June everyone will be able to use 2.0.x and 2.1.x in parallel by just changing branch in the 3sdk tool


### development on 

- all is on ```development``` branch for jumpscale
- all developers can use it now using 3sdk tool

