## Convert file to base64

```powershell
$rawString = "test:123 test2:1234 test3:12345"  # or
$rawString = get-content -path .\custom-data.txt -encoding utf8 -raw
$encodedString = [System.Text.Encoding]::UTF8.GetBytes($rawString)
[System.Convert]::ToBase64String($encodedString) >> customdata64.txt
```


## Convert file from base64

```powershell
$EncodedString = get-content -path .\customdata64.txt -encoding utf8 -raw   # or
$EncodedString = "dGVzdDoxMjMgdGVzdDI6MTIzNCB0ZXN0MzoxMjM0NQ=="

$DecodedString = [System.Text.Encoding]::UTF8.GetString([System.Convert]::FromBase64String($EncodedString))
Write-Output $DecodedString
```
