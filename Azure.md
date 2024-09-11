Ex:Create ubuntu linux virutual machine?

name: <#of characters>

name = 1 to 12

+++++++++++++++++++++++++++++++++++++++++

  1.Resource Provider :Azure serives (VMs,DB,Network,Storage ..etc)
  
  
  2.Setup Your Environment
    -Azure portal
	-Azure CLI
	-Azure Powershell
	-Visual studio
	
	
3.Create a Resource Group
  -Azure Portal: 
  -Azure  CLI:
  az group create --name MyResourceGroup --Location eastus
  
  -Azure Powershell
  New-AzResourceGroup -Name New-AzResourceGroup -Location eastus
  
4.Create  a ARM Template
  -Create JSON ARM template in VScode editor
  
5.Deploy the template
   
    -Azure CLI:
	az deployment group create --resource-group MyResourceGroup 
	--storage-account.json
	
	-Azure Powershell
	New-AzResourceGroupDeployment -ResourceGroupName MyResourceGroup
	-TemplateFile storage-account.json
   