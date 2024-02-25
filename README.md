

```


 __     __  ______   ______  _______   ______  __    __ ________                                                          
/  |   /  |/      \ /      \/       \ /      \/  \  /  /        |                                                         
$$ |   $$ /$$$$$$  /$$$$$$  $$$$$$$  /$$$$$$  $$  \ $$ $$$$$$$$/                                                          
$$ |   $$ $$ |__$$ $$ | _$$/$$ |__$$ $$ |__$$ $$$  \$$ |  $$ |                                                            
$$  \ /$$/$$    $$ $$ |/    $$    $$<$$    $$ $$$$  $$ |  $$ |                                                            
 $$  /$$/ $$$$$$$$ $$ |$$$$ $$$$$$$  $$$$$$$$ $$ $$ $$ |  $$ |                                                            
  $$ $$/  $$ |  $$ $$ \__$$ $$ |  $$ $$ |  $$ $$ |$$$$ |  $$ |                                                            
   $$$/   $$ |  $$ $$    $$/$$ |  $$ $$ |  $$ $$ | $$$ |  $$ |                                                            
    $/    $$/   $$/ $$$$$$/ $$/   $$/$$/   $$/$$/   $$/   $$/                                                             
                                                                                                                                                                                                                     

```

```
 __     __ ______ _______  ________ __    __  ______  __       ______ ________  ______  ________ ______  ______  __    __ 
/  |   /  /      /       \/        /  |  /  |/      \/  |     /      /        |/      \/        /      |/      \/  \  /  |
$$ |   $$ $$$$$$/$$$$$$$  $$$$$$$$/$$ |  $$ /$$$$$$  $$ |     $$$$$$/$$$$$$$$//$$$$$$  $$$$$$$$/$$$$$$//$$$$$$  $$  \ $$ |
$$ |   $$ | $$ | $$ |__$$ |  $$ |  $$ |  $$ $$ |__$$ $$ |       $$ |     /$$/ $$ |__$$ |  $$ |    $$ | $$ |  $$ $$$  \$$ |
$$  \ /$$/  $$ | $$    $$<font   $$ |  $$ |  $$ $$    $$ $$ |       $$ |    /$$/  $$    $$ |  $$ |    $$ | $$ |  $$ $$$$  $$ |
 $$  /$$/   $$ | $$$$$$$  |  $$ |  $$ |  $$ $$$$$$$$ $$ |       $$ |   /$$/   $$$$$$$$ |  $$ |    $$ | $$ |  $$ $$ $$ $$ |
  $$ $$/   _$$ |_$$ |  $$ |  $$ |  $$ \__$$ $$ |  $$ $$ |_____ _$$ |_ /$$/____$$ |  $$ |  $$ |   _$$ |_$$ \__$$ $$ |$$$$ |
   $$$/   / $$   $$ |  $$ |  $$ |  $$    $$/$$ |  $$ $$       / $$   /$$      $$ |  $$ |  $$ |  / $$   $$    $$/$$ | $$$ |
    $/    $$$$$$/$$/   $$/   $$/    $$$$$$/ $$/   $$/$$$$$$$$/$$$$$$/$$$$$$$$/$$/   $$/   $$/   $$$$$$/ $$$$$$/ $$/   $$/ 
                                                                                                                          
 
```
                                                                                                                          
        ______  __    __ ________ ______  __       __  ______  ________ ______  ______  __    __                          
  /      \/  |  /  /        /      \/  \     /  |/      \/        /      |/      \/  \  /  |                         
 /$$$$$$  $$ |  $$ $$$$$$$$/$$$$$$  $$  \   /$$ /$$$$$$  $$$$$$$$/$$$$$$//$$$$$$  $$  \ $$ |                         
 $$ |__$$ $$ |  $$ |  $$ | $$ |  $$ $$$  \ /$$$ $$ |__$$ |  $$ |    $$ | $$ |  $$ $$$  \$$ |                         
 $$    $$ $$ |  $$ |  $$ | $$ |  $$ $$$$  /$$$$ $$    $$ |  $$ |    $$ | $$ |  $$ $$$$  $$ |                         
 $$$$$$$$ $$ |  $$ |  $$ | $$ |  $$ $$ $$ $$/$$ $$$$$$$$ |  $$ |    $$ | $$ |  $$ $$ $$ $$ |                         
 $$ |  $$ $$ \__$$ |  $$ | $$ \__$$ $$ |$$$/ $$ $$ |  $$ |  $$ |   _$$ |_$$ \__$$ $$ |$$$$ |                         
 $$ |  $$ $$    $$/   $$ | $$    $$/$$ | $/  $$ $$ |  $$ |  $$ |  / $$   $$    $$/$$ | $$$ |                         
 $$/   $$/ $$$$$$/    $$/   $$$$$$/ $$/      $$/$$/   $$/   $$/   $$$$$$/ $$$$$$/ $$/   $$/                          
                                                                                                                          
                                                                                                                     
                                                                                                                           
 
```


# Vagrant Virtualization Automation

## Overview

This branch contains configurations for automating virtualization with Vagrant. It includes features like directory syncing, provisioning, pruning, and multi-VM setups. This guide provides detailed instructions on setting up and using the Vagrant environment.

## My Information

- Name: Dhanraj Choudhary
- Role: Developer
-  [Go to my portfolio](https://portfoli2.vercel.app/)

## Prerequisites

Before using this Vagrant setup, ensure you have the following installed on your system:

- [Vagrant](https://www.vagrantup.com/downloads.html)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) (or another provider supported by Vagrant)

## Setup

1. Clone this repository and checkout the "vagrant" branch:

   ```sh
   git clone -b vagrant https://github.com/DHANRAJCHOUDHARY244/DEVOPS.git
   ```

2. Navigate to the project directory:

   ```sh
   cd DEVOPS
   ```

## Usage

### Starting a Vagrant Environment

To start a single VM:

```sh
vagrant up
```

To start multiple VMs:

```sh
vagrant up vm1 vm2
```

To start all VMs defined in the Vagrantfile:

```sh
vagrant up --no-parallel
```

### Stopping a Vagrant Environment

To stop a single VM:

```sh
vagrant halt vm-name
```

To stop all running VMs:

```sh
vagrant halt
```

### Provisioning

To provision a VM:

```sh
vagrant provision vm-name
```

To provision all VMs:

```sh
vagrant provision
```

### Synced Folders

By default, the `./data` directory on your host machine is synced to `/vagrant_data` inside the VM. Edit the Vagrantfile to customize this behavior.

### Pruning

To remove all resources associated with a VM:

1. Stop and delete the VM:

   ```sh
   vagrant destroy vm-name
   ```

2. Delete the base box:

   ```sh
   vagrant box remove box-name
   ```

### Multi-VM Setup

Edit the Vagrantfile to define multiple VMs. Use `vagrant up` with the VM names to start them.

## Customization

- Edit the Vagrantfile to adjust VM configurations, synced folders, and provisioning scripts.
- Place provisioning scripts in the `provision` directory.

## Notes

- For troubleshooting and detailed usage, refer to the [Vagrant documentation](https://www.vagrantup.com/docs).
- Ensure your host machine meets the [hardware requirements](https://www.virtualbox.org/manual/ch01.html#intro-installing) for virtualization.

```
