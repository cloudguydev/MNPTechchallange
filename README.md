# MNPTechchallange
Iac Build for MNP DevOps Challenge.

To deploy the ARM Template Iac MNP VMwebserver Build,Please click on the <b>Deploy to Azure Button </b> or use the <b>azure-pipelines.yml</b>

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fcloudguydev%2FMNPTechchallange%2Fmain%2FMNP_VMWebserver_template.json" rel="nofollow">
  <img src="https://aka.ms/deploytoazurebutton"/>
</a>

This template  deploys  Windows 2019 Datacenter server, using the latest patched version. This will deploy a A1 v2 size VM in the Az resource group in canada central and return the fully qualified domain name of the VM. The template code has a ConfigureIIS resource custom script type for automated install of IIS  on the VM.

Data residency region is in canada central.

Deployed Server is enabled for Monitoring  and Update managements through the "bootDiagnostics""enabled": true property on the template. 

Please see the <b> MNP DevOps Challenge Solution Consideration</b> file for my detailed explantion on how i considered the project requirnment and my chosen cause of action to meet the project requirnment. Also see the <b> MNP DevOps Challenge Solution Screen shot</b> file

Future work would be seperating  the Iac into a linked template scheme.

Main working files for this challange are;
- MNP_Webserver_template.json
- MNP DevOps Challenge Solution Consideration
- MNP DevOps Challenge Solution Screen Shot
- azure-pipelines.yml : working yml for CD of the build

Experimentation files. Intended to build out  the Iac as linked template (Future work). Probally the better way to excute the build when considering using deployment best practices.
- MNP_Webserver_parameters.json
- MNP_main_template.json
- MNP_main_parameter.json
- .github/workflows

Other resources included in the ARM deployment include:

- Configure IIS with CSE
- Virtual Network
- Network Security Group
- Network Interface
- Storage Account
- Network Interface
