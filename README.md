# Vagrant Kubernetes Cluster
Vagrant Kubernetes cluster for local development and testing. Repo created for reference purpose only.

Installation and configuration is inspired by: https://kubernetes.io/blog/2019/03/15/kubernetes-setup-using-ansible-and-vagrant/. Majority of its settings have been reproduced, reused and stored for reference.

## Prerequisites
- Vagrant
- Oracle Virtual Box
- Ansible
- Ansible Galaxy

## Installation
Open current directory in terminal and execute: ```vagrant up```. Observe the output and VM creation results (master and 2 worker nodes).

### Ansible installation playbooks
Core installation playbooks (```/kubernetes-setup```):
- Install and perform initial configuration of master node
- Install and perform initial configuration of 2 worker nodes
- Join worker nodes with master

### Commands
Commands directory (```/commands```) is supplied for reference purposes only and includes basic command to work on a Kubernetes cluster such as:
- Setup cluster from scratch
- Working with nodes, pods etc.
- Check status of cluster, describe, explain etc.
