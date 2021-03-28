$myHashtable = @{
    Name     = 'Mike'
    Language = 'PowerShell'
    State    = 'Virginia'
}
$myObject = [pscustomobject]$myHashtable

$myObject | Add-Member -MemberType NoteProperty -Name 'Username' -Value 'mmoore'

