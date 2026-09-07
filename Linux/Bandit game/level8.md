# Level 8 > 9

## Main task
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Steps taken
After sorting the file to group duplicate lines together, use uniq -u to display only the line that appears once. The password was obtained by running sort data.txt | uniq -u.

```bash
sort data.txt | uniq -u

# Password: EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl

```

## commands used
- uniq
- sort


