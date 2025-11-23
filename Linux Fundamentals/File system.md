## Soft Links, Hard Links, cp, and mv 
# Soft Links (Symbolic Links)
Always use absolute paths when creating soft links.

Syntax: ln -s <target-file> <link-name>

```
ln -s /opt/mysoftlink.txt /home/symbolic.txt
/opt/mysoftlink.txt → Original (parent) file
/home/symbolic.txt → Symbolic (child/orphan) link
```
Important:
If the parent file is deleted, the symbolic link becomes broken.
Recreating a file with the same name does not fix the link unless the path and inode match.

# Creating Soft Links Between Folders:
 ```
 ln -s /home/softlink /opt/mysoftlink
```
# Backups Using cp
```
cp <source> <destination>
Copy a directory (requires -r):
cp -r super1 /opt/
cp rana10.txt /opt/
```
