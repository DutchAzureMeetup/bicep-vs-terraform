# 1. Install Bicep: 

## With chocolatey:
```
choco install bicep
``` 
## With Winget:
```
winget install -e --id Microsoft.Bicep
```

## With a custom Powershell script:

Use the [install-bicep.ps1](scripts/install-bicep.ps1) in this repo (in the scripts folder)

# 2. Login to Azure

## With Azure Powershell:
```
Connect-AzAccount
``` 
## With Azure CLI:
```
az login
```

# 3. Create your bicep files

That's up to you ;)

# 4. Deploy

## With Azure Powershell:

### subscription-level deployment:
New-AzSubscriptionDeployment -Location <location> -TemplateFile <path-to-bicep>

### resourcegroup-level deployment:
New-AzResourceGroupDeployment -ResourceGroupName <resource-group-name> -TemplateFile <path-to-bicep>

## With Azure CLI:

### subscription-level deployment:
az deployment group create --resource-group <resource-group-name> --template-file <path-to-bicep>

### resourcegroup-level deployment:
az deployment sub create --location <location> --template-file <path-to-bicep>
