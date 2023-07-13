# RemoteDCdeploy
Ansible playbooks to perform a full Edge datacenter deployment based on Dell VxRail. The code in this repo was used in this [IaC Avengers video](https://www.youtube.com/watch?v=NFDMtoVon6E)

## Components
- "main.yml" this is the playbook that starts the process 
- "dc-templates" directory contains datacenters templates. These are JSON files that define the different applications/VMs that need to be deployed in the Edge datacenter. At the start the playbook prompts for the name of the datacenter template to use
- "VxRail_Configuration.json" is a file with the [pre-answered questions of the deployment wizard](https://infohub.delltechnologies.com/p/the-latest-vxrail-platform-innovation-is-now-included-in-your-cloud/)
- "create-vms.yml" playbook creates the VMs with the hardware configuration defined in the datacenter template
- "profile" directory contains playbooks to deploy specific applications
- "source_files" directory contains directory structures 
