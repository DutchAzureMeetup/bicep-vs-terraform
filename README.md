# bicep-vs-terraform

# Quickstart 

## Bicep

### 1. Install bicep: 

#### With chocolatey 
```
choco install bicep
``` 
#### With Winget
```
winget install -e --id Microsoft.Bicep
```

### 2. Login to Azure

#### With Azure Powershell 
```
Connect-AzAccount
``` 
#### With Azure CLI
```
az login
```

### 3. Create your bicep files

### 4. Deploy

#### With Azure Powershell 

##### subscription-level deployment:
New-AzSubscriptionDeployment -Location <location> -TemplateFile <path-to-bicep>

##### resourcegroup-level deployment:
New-AzResourceGroupDeployment -ResourceGroupName <resource-group-name> -TemplateFile <path-to-bicep>

#### With Azure CLI 

##### subscription-level deployment:
az deployment group create --resource-group <resource-group-name> --template-file <path-to-bicep>

##### resourcegroup-level deployment:
az deployment sub create --location <location> --template-file <path-to-bicep>
