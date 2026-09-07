# Level 9 > 10

## Main task
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Steps taken
since the file is in binary use the string command to find for any human readable file in the data.txtg Grep was used to find the pattern = in the file. After using cat to inspect the contents of the file, I used strings data.txt | grep "=" to locate the line that contained the password.

```bash
strings data.txt | grep "=="

# Password: B0s2khmbT9u0geKuOoVGW3JZKhndE3BG

## commands used
- strings
- grip


