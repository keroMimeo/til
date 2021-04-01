```powershell
$myHashtable = @{      
    fname     = 'kero'   
    lname = 'mimeo'    
    id = 42    
}   
```

Create the PS Custom Object
```powershell
$myObject = [pscustomobject]$myHashtable     
```
Add a new field and value to the object
```powershell
$myObject | Add-Member -MemberType NoteProperty -Name 'Username' -Value 'keromimeo'     
````

Original values in the hashtable    
```powershell
$myHashtable     
```


New field and value are seen in the custom object   
```powershell
$myObject     
```
