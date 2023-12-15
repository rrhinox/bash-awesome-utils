# ☁️  Az-cli awesome command line for day by day!

## Intro & Documentation

**What is Azure CLI?**

The Azure command-line interface (Azure CLI) is a set of commands used to create and manage Azure resources. The Azure CLI is available across Azure services and is designed to get you working quickly with Azure, with an emphasis on automation.

[Azure CLI Home](https://learn.microsoft.com/en-us/cli/azure/)

[What is?](https://learn.microsoft.com/en-us/cli/azure/what-is-azure-cli)

[Reference index](https://learn.microsoft.com/en-us/cli/azure/reference-index?view=azure-cli-latest)



## Main command 

+ `az login --use-device`

+ `az account set --subscription 1b1b1b1b-9aa1-4x75-9d7d-\*******`

## Example with some context

### Azure AKS connect and kubelogin convert credentials 

Connect to Azure Kubernetes service and convert credentials from cluster with kubelogin :

+ `az aks get-credentials --resource-group rg-dev --name aks-dev`

+ `kubelogin convert-kubeconfig -l azurecli`