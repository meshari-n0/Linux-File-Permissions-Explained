# Linux File Permissions (Based on `ls -al` Output)
![Linux](https://github.com/user-attachments/assets/7c3843c0-984e-4e52-83b8-014c98f7077a)

Example:

```
drwxr-xr-x  2 baraa  4096  Feb 01 01:07  .config
```

## Structure Breakdown

```
drwxr-xr-x
│││ │ │ │
│││ │ │ └── Others permissions
│││ │ └──── Group permissions
│││ └────── Owner permissions
││└──────── Permission letters (r, w, x)
└────────── File type
```

## File Type

- `d` → Directory  
- `-` → Regular file  

---

## Permission Letters

- `r` → Read  
- `w` → Write  
- `x` → Execute  
- `-` → No permission  

Example:

```
rwxr-xr-x
```

- Owner → Read, Write, Execute  
- Group → Read, Execute  
- Others → Read, Execute  

---

## Other Columns in `ls -al`

Example:

```
drwxr-xr-x  2 baraa  4096  Feb 01 01:07  .config
```

- `2` → Number of links  
- `baraa` → Owner  
- `4096` → Size in bytes  
- `Feb 01 01:07` → Date and time  
- `.config` → File/Directory name  

---

## Hidden Files

Files starting with `.` are hidden:

```
.bashrc
.env
.gitconfig
.ssh
```

---

## Example of a Regular File

```
-rw-r--r--  1 baraa  264  Dec 6 2025  .bashrc
```

- `-` → Regular file  
- `rw-` → Owner: Read & Write  
- `r--` → Group: Read only  
- `r--` → Others: Read only  
