# Cheatsheet

## `find`

To change all the directories to 755 (`drwxr-xr-x`):

```
find sampledir -type d -exec chmod 755 {} \;
```

To change all the files to 644 (`-rw-r--r--`):

```
find sampledir -type f -exec chmod 644 {} \;
```

