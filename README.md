# CST8912 Lab 1

**Student Name**: Collin MacLeod
**Student ID**: macl0379
**Course**: CST8912 Cloud Solutions Architecture
**Semester**: Fall 2026

## How the VM, OS disk, network interface, virtual network, subnet, public IP, network security group, Log Analytics workspace, Azure Monitor Agent, and data collection rule relate to each other.

These components relations can be traced from the compute resource. The VM runs the system d applications that are held on the OS disk. Inside of a Virtual network (VNet), the VM is able to communicate with other resources through a network interface (NIC). The VNet can be divided into subnets to logical sections which limit congestion between unrelated resources and maintains better security. Security rules for the NIC or a subnet will be set on a Network Security Group (NSG). To communicate with addresses outside of the VNet, a resource will have a public IP address.

To monitor the system an Azure Monitor Agent can be run inside a VM to gather performance metrics and logs. This information is collected and sent based on the configuration of the Data Collection Rule (DCR). The destination is usually a Log Analytics workspace where Azure Monitor stores and provides an interface to analyze, visualize and create alerts.

## Reflections

During this Lab my biggest take away was the seemingly infinite amount of configurations you have available to setup VMs and VNets as well as all the supporting systems around it. It was also apparent how expensive these systems can get and how over supplying resources . At a low level system running for a short period of time but when you look at a service that might need 1000+ machines running these costs can add up quickly.

## Screenshots

### 1. Resource Group

![Resource Group Screenshot](/Screenshots/Resource-Group.png)

### 2. VM Deployment & Overview

![VM Deployment Screenshot](/Screenshots/VM-Deployment.png)

![VM Overview Screenshot](/Screenshots/VM-Overview.png)

### 3. Stopping & Starting of VM

![VM Stop and Start Screenshot](/Screenshots/Stop&Start-Success.png)

### 4. Log Analytics Workspace

![Log Analytics Workspace Screenshot](/Screenshots/LAW.png)

### 5. Azure Monitor Agent

![Azure Monitor Agent Screenshot](/Screenshots/AzureMonitorLinuxAgent.png)

### 6. SSH Command Output & File Transfer Verification

![Terminal Output Screenshot](/Screenshots/Command-Line-Output.png)

### 7. Cleanup Confirmation

![Cleanup Confirmation Screenshot](/Screenshots/Resource-Cleanup.png)