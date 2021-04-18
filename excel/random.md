## Create random numbers and characters in Excel

| Function | Result  |
|:-----------|:-----------|
| =RAND()| Generates number between 0 and 1  |
| =RANDBETWEEN(1,11) | Generates numbers between 1 and 11  |
| =CHAR(RANDBETWEEN(65,90)) | Generates an ASCII character between A and Z  |


### Add additional characters and symbols    
You can use the ASCII characters and symbols between 1 and 255, or just a subset.   

A - Z == 65 - 90    
a - z == 97 - 122   
0 - 9 == 48 - 57   
\# == 35    
$ == 36   

e.g. generate an uppercase letter, a random ASCII character, then a lowercase symbol    
=CHAR(RANDBETWEEN(65,90))&CHAR(RANDBETWEEN(1,255))&CHAR(RANDBETWEEN(65,90))    

Don't forget to add the '&' between the different RANDBETWEEN functions in the cell.     
