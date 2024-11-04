# Windows Bootable Pendrive Commands
## this command will not run in win xp so run this command in a newer version of windows like-win7,vista,win8 etc
```
diskpart
```
```
list disk
```
```
select disk no.
```
```
clean
```
```
create partition primary
```
```
select partition 1
```
```
active
```
```
format fs=ntfs quick
```
```
assign
```
(copy the content of windows into pendrive)
```
exit
```
