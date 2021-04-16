## Identify API versions for Azure Resource Types

```powershell
((Get-AzResourceProvider -ProviderNamespace Microsoft.Web).ResourceTypes | Where-Object ResourceTypeName -eq sites).ApiVersions

```
