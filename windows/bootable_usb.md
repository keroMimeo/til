## Create a bootable USB to install Windows

Start a Command Prompt or PowerShell as Administrator 
```powershell
diskpart
list disk
select disk [x]   # Where x is the USB drive letter
clean   # removes all partitions from selected drive
create partition primary
select partition 1
active
format fs=ntfs quick
assign
exit
```

Insert a bootable Windows installation DVD or mount an ISO

```powershell
cd g:\boot  # boot directory of the Windows install disk or ISO
bootsect /nt60 d:  # where d: is the USB drive
```

Copy all installation files to the USB drive
```PowerShell
xcopy g:\*.*  /s /h /f d:\

/s - Copies directories and subdirectories except empty ones.
/h - Copies hidden and system files.
/f - Displays full source and destination filenames while copying.
```
