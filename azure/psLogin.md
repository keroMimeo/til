### PowerShell Login
```powershell
connect-azAccount

#  Set Environment
Connect-AzAccount -EnvironmentName AzureCloud
Connect-AzAccount -EnvironmentName AzureUSGovernment

# Shows available subscriptions from your tenant
Get-AzSubscription
	
Get-AzContext -ListAvailable

$context = Get-AzSubscription -SubscriptionId xxx-xx-xxx
Set-AzContext $context
Get-AzContext
```