## Convert file to base64

```powershell
$rawString = get-content -path .\init-ubuntu.sh -encoding utf8 -raw
$encodedString = [System.Text.Encoding]::UTF8.GetBytes($rawString)
[System.Convert]::ToBase64String($encodedString) >> init.txt
```
