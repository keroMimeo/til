## List the VMs running in a Resource Group

Azure CLI   

```powershell
running_vm_ids=$(az vm list --resource-group MyResourceGroup --show-details \
   --query "[?powerState=='VM running'].id" --output tsv)
```

