# Level 2 > 3

## Main task
Find the password for the next level in a file called --spaces in this filename-- located in the home directory.

## Steps taken
Used ls command first to read any content inside the directory
Located a file called "spaces in the filename" used cat command didnt work
since file name has spaces and it has -- we add that when using the cat command including quotetation  marks 

```bash
ls          # To check for any directory or file
cat "--spaces in this filename--"
# OR
cat ./--spaces\ in\ this\ filename--

# Password: 7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
```

## commands used
- ls 
- cat 
