# MNPTechchallange
Iac Build for MNP DevOps challenge

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fcloudguydev%2FMNPTechchallange%2Fmain%2FMNP_VMWebserver_template.json" rel="nofollow">
  <img src="https://aka.ms/deploytoazurebutton"/>
</a>

This template  deploys  Windows 2019 Datacenter server, using the latest patched version. This will deploy a A1 v2 size VM in the Az resource group in canada central and return the fully qualified domain name of the VM. The template code has a ConfigureIIS resource custom script type for automated install of IIS  on the VM.

Data residency region is in canada central.

Deployed Server is enabled for Monitoring  and Update managements throughthe "bootDiagnostics""enabled": true property on the template. 

Please see the <b> MNP DevOps Challange Solution Consideration</b> doc for my detailed explantion on how i considered the project requirnment and my chosen cause of action to meet the project requirnment. 

Seperated the Virtual Machine resource into a linked template.

Other resources included in the deployment include:

- Custom script extension
- Virtual Network
- Network Security Group
- Network Interface
- Storage Account
- Network Interface
