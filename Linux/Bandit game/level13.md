# Level 13 > 14

## Main task
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Steps taken
Found ssh key private file when using  ls commmand , exited the level since no need to continue on this used scp command to move the file to my local host directory after this loggged in using the previous level password. To be able to use the sshkey file we need to change file permission by using chmod 600 to give full permission to the owner only, ssh -I lets me use identify file without any password moving straight to level 14

```bash
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .
chmod 600 sshkey.private
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220

# Password: none
```

## commands used
- ls
- scp
- chmod
- ssh

                                 
