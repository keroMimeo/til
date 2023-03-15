# Report the current line number from a failure

```powershell
try { 
  $a = 1234 
  $sdf = 'fasdf' 
  
  throw 'Some error'
}
  
catch { 
    $ln = $_.InvocationInfo.ScriptLineNumber 
    Write-Host "Failed at line: $ln" 
    -ForegroundColor Red
}
```
