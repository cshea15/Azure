# Backup for Personal HostPools

## Introduction

Peronsal Session Host VMs are treated like a physical device and the data is stored locally it might be a good idea to backup your VMs. By backing up your VMs you will be able to restore from a certain point incase you run into any data loss or VM corruption. 

## How to set it up
- Create a Recovery Services Vault in the same region as your VM (ie VM is located in US East, create RSV in East US). 
- Under Getting Started Select Backup
- Make sure your Azure is selected for "Where your workload is running?" and Virtual Machines is selected for "What you want to backup?"
- Select "Backup" and either use the "Default Policy" or create a new policy. 
- Add your Virtaul Machines you want to back up and then Enable Backup. 

**IMPORTANT:** You should set alerts incase of backup failure. You will be alerted and make sure you have the latest backup. 

## Resources
- [Overview of Azure VM Backup](https://docs.microsoft.com/en-us/azure/backup/backup-azure-vms-introduction)
