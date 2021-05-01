## List extensions in a region

Azure CLI   

```powershell
az vm extension image list --location <REGION_NAME> --output table

az extension=$(az vm extension image list -l eastus2 -o tsv)
```