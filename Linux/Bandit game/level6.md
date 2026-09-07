# Level 6 > 7

## Main task
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

## Steps taken
Finding the file using its properties—user bandit7, group bandit6, and size 33 bytes—was done using find. After the right file location was given by running find / -user bandit7 -group bandit6 -size 33c 2>/dev/null, the password was read using cat.

```bash
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password

# Password: Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3

```

## commands used
- find
- cat 
- 2>/dev/null


