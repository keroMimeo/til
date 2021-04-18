## Identify API versions for Azure Resource Types

```powershell
((Get-AzResourceProvider -ProviderNamespace Microsoft.Web).ResourceTypes | Where-Object ResourceTypeName -eq sites).ApiVersions

```

[Microsoft Resource Providers and Types](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/resource-providers-and-types)


![image name](/../images/resourceexplorer.png)

