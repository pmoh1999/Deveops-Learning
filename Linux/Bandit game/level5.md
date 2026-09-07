# Level 5 > 6

## Main task
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

## Steps taken
Always use the ls to check for any  directory or files, used cd command to see whats inside the inhere directory within that try to locate the exact using the prorerties from above so used find . ! -executable -readable -size 1033c  after that using cat command we got the password for the next level

```bash
ls
cd inhere
find . ! -executable -readable -size 1033c
cat inhere/maybehere07/.file2

# Password: pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
```

## commands used
- ls
- cd
- find
- cat


