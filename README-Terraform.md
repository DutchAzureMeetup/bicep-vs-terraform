# 1. Install Terraform: 

## With chocolatey:
```
choco install terraform
``` 
## Manual:
```
Download here https://www.terraform.io/downloads
```

## OSX:

brew tap hashicorp/tap
brew install hashicorp/tap/terraform
brew update
brew upgrade hashicorp/tap/terraform

## Linux:

Pick your distribution and follow the guide here:
https://learn.hashicorp.com/tutorials/terraform/install-cli


# 2. Login to Azure

``` 
## With Azure CLI:
```
az login

# 3. Create your Terraform templates

Create a directory and add *.tf templates.

The templates are up to you :wink:

# 4. Deploy

In the directory you created:

terraform init (only once or after changes to modules, providers or backend. You will be notified when you forget.)

terraform apply
```
