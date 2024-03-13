

# Project Branch: Full-Stack Automation Java Application with Vagrant Provisioning

This branch contains configurations and scripts for setting up a development environment using Vagrant. The project includes a full-stack automation Java application with the following components running in separate Vagrant VMs:

- **Java Application:** A Java application for automation tasks.
- **RabbitMQ:** A message broker for communication between components.
- **Tomcat:** A web server for hosting the Java application.
- **SQL:** A database for storing application data.
- **Memcached:** A distributed memory caching system for improving performance.
- **Nginx:** A web server for serving static content and acting as a reverse proxy.

## Getting Started

To get started with the development environment, follow these steps:

1. Clone the repository and switch to the `vagrant` branch:

   ```bash
   git clone https://github.com/DHANRAJCHOUDHARY244/DEVOPS.git
   cd DEVOPS
   git checkout project
   ```

2. Provision the Vagrant environment:

   ```bash
   vagrant up
   ```

