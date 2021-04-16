## Identify Virtual Machines available in a specific region    

```powershell
$variable = Get-AzComputeResourceSku

$variable | where {?_.locations.contains("eastus") -and ?_.resourcetype ` 
-eq "virtualmachines" -and $_.name -like "standard_A*"}

```
