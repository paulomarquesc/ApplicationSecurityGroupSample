# ApplicationSecurityGroupSample

<a href="https://portal.azure.com/#create/Microsoft.Template/urihttps%3A%2F%2raw.githubusercontent.com%2paulomarquesc%2ApplicationSecurityGroupSample%2master%2ApplicationSecurityGroups.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>

<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2F100-blank-template%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a>

This template shows how to work with Application Security Groups using templates. It assigns a VM to the Application Security Group and assigns this Application Security group to two security rules on Network Security Group, one that allows SSH and another one that allows HTTP using the Destination Application Security Group Id property of the security rule. 

It deploys the following items:
1. Application Security Group
1. Network Security with two Security Rules, both using destinationApplicationSecurityGroups attribute
1. Virtual Network with one Subnet assigned to this NSG.
1. Network Interface assigned to Application Security Group, through its ID (notice that more than one can be assigned)
1. Centos 6.9 Linux Web server with NGINX installed through Custom Script Extension for Linux

For more information about Application Security Groups, please refer to:

[Network Security Groups under Network Security document](https://docs.microsoft.com/en-us/azure/virtual-network/security-overview#application-security-groupshttps://docs.microsoft.com/azure/virtual-network/security-overview)

[Filter network traffic with a network security group using PowerShell](https://docs.microsoft.com/en-us/azure/virtual-network/tutorial-filter-network-traffic)

[Filter network traffic with a network security group using the Azure CLI](https://docs.microsoft.com/en-us/azure/virtual-network/tutorial-filter-network-traffic-cli)


