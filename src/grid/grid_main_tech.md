
![](./img/tf_solution.png)

# ThreeFold Grid Main Technology Components

TODO: Sacha - make it clear that this is for tech people
### Zero-OS 

Zero-OS is a minimal operating system serving one single purpose: to make the hardware available to the autonomous layer. Zero-OS is a stateless operating system and is not installed on a storage device in the server. At boot time, the needed binaries and config files are made available over a secure network connection. The zero-footprint locally on the server simplifies administration work needed for these servers, enabling these servers to live anywhere.

In Zero-OS, the number of active components and therefore the complexity of the operating system has been brought down to the absolute minimum, making maximum execution capacity available to real-world use cases and applications.

- Core-0: We call Core-0 the combination of all the low level components of Zero-OS. Each component is responsible for a part of the logic handled by Zero-OS when exposing the hardware capacity (storage, compute, and network) to the higher layers.

- Core-X: Is the process manager for an individual container. Because of the secure nature of the 3Nodes, a direct connection from a user to a node is not possible, but Core-X allow users to connect to their own containers and manage the processes inside. It has a web interface as well as a REST interface. So, the containers can be managed both manually and programatically.

Read more about the Zero-OS in our [capacity white paper](https://wiki.threefold.io/#/capacity_layer_image).

### 3Bot

3Bot is the intelligent virtual alter ego which manages everything in our digital life, or the digital life of our company. The 3Bot makes it possible to run workloads in a fully autonomous manner. Your Digital Avatar (the 3Bot) has been designed to be as efficient as possible. The current memory footprint is less than 200MB yet still it is a wiki system, database, blockchain, web server, indexing & search machine, e-commerce system, wallet, decentralized exchange, and more. It can manage millions of objects and is the center of your company or your digital life.

To create this 3Bot we had no choice other than to start from scratch and re-invent a lot because existing IT components are too centralized and often too inefficient (e.g. memory hungry). The result is a system that has the right balance between resilience and efficiency. A lot of services are already available today.

Some of the first features include:
- Identity Information
- Autonomous DAPPS SDK
- Serverless Core 
    - Email, chat, contacts, calendar
    - speaks all legacy interfaces
- Up-to PB of storage per 3Bot 
    - Videos, pictures
    - Documents
    - Structured Database 
- Browser in Browser
- FinTech Platform
    - Ultra Secure Wallet
    - Decentralized Exchange
- Decentralized Applications for end-users
    - Social Media 
    - Video Conferencing 
    - File Storage 

Read more about the 3Bot in our [autonomous white paper](https://wiki.threefold.io/#/autonomous_layer_whitepapers).

### Jumpscale X

The automation platform which makes the 3Bot possible. Jumpscale is an automation framework written in Python. It has been developed for more than a decade and originates from an automation product which was acquired by SUN Microsystems from Q-Layer, which was one of our previous companies. Our newest release is version 10, called JSX.

Jumpscale is the foundation for the autonomous layer. To get to autonomous operations, IT experts have to model IT architectures. These models have to describe all the components involved in creating the architecture (e.g. a container running a webserver, a container running a database server, and then all the required network paths between these two containers and the rest of the world). Once this description is complete and tested, it can be given to the autonomous layer which launches, monitors, and operates the architecture. Hence, autonomous IT.

Read more about the Jumpscale in our [autonomous white paper](https://wiki.threefold.io/#/autonomous_layer_whitepapers).

### Beyond Blockchain Database (BCDB) 

This is a highly-capable database (scalable, secure, etc) incorporating all the features of modern blockchain technology.

The blockchain database (BCDB) is a super-efficient database that uses blockchain technology to securely store and retrieve data. Blockchain principles like “always append” and “store data in an immutable manner” are key aspects of this database technology.

The blockchain database is used in the autonomous layer for storing information of users, farmers, the digital representatives (3Bots), IT Architecture descriptions, and the state information of these running applications. This database technology provides distributed storage of key information of the autonomous layer.

For a 100 node deployment, our BCDB will be *50x more efficient *compared to other blockchain technologies for storing data from a storage and network perspective.

The BCDB is used in the 3Bot which means every user has his or her own Blockchain DataBase. A BCDB can also be used as a shared ledger between multiple people.

Read more about the BCDB in our [autonomous white paper](https://wiki.threefold.io/#/autonomous_layer_whitepapers).

### Zero-Store Technology

The Zero-Store technology contains all the logic to store data in a reliable and effective manner over multiple devices in multiple geo-locations. Embedded in the software are basic storage primitives to process data before sending it to distributed devices, which are aimed at increasing the performance of searching, finding data, and securing data.

Chunking: makes large datasets indexed and cut into smaller organized data chunks, improving access and search speed.
Compression: makes data storage use less physical storage by passing it through an algorithm that compresses the data volume.
Encryption: creates unreadable data for the people or processes that do not have the (proper) key to decipher the information.
Disperse: storage in such a way that data becomes 100% secure and cannot be retrieved from one site alone. It also allows you to retrieve your data when some of the storage nodes are offline.
All of these primitives are configurable and you can decide how data will be processed (optimized) before being sent to the distributed storage devices → the zero-databases. This makes dispersed storage a very reliable and performant storage solution without compromising effective use of physical storage capacity.

Read more about our storage system in our autonomous white paper.

### Zero-Database Technology

Zero-DB technology is characterized by the following aspects:

- Backend Storage Engine
- Can do +50.000 transactions per/sec
- Can work on SSD & HD
- Optimized for easy (soft/green) operation on HD
- Works with reservations
- Always append store
- Can keep unlimited history
- Master/Slave replication

### Open Source

All our code is dual licensed and free - which means all code is open source but there is no support provided. All our code is available on GitHub. We recognize that the documentation available on Github is probably not enough for anyone to pick it up, we aim to address this int he future. 

If you have any questions, we invite you to ask them on the [ThreeFold Forums](https://forum.threefold.io).