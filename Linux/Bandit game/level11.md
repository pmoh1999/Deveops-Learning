# Level 11 > 12

## Main task
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Steps taken
ROT13, which moves every letter in the alphabet 13 places, was used to encode the file. The password was found by decoding the text using cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m '. 

```bash

cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

# Password: GROozWPO8QyN0mGrjUkID0WCYkZiQxrN

```

## commands used
- cat
- tr 

                                 
