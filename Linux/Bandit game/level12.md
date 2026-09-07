# Level 12 > 13

## Main task
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Steps taken
I began by determining the kind of file I was working with. I used xxd -r to reverse the hexdump file back into a regular binary file. After that, I continued to use the file to determine its format after each step, always using the appropriate decompression/decoding commands (such as gzip, bzip2, tar, or base64). I eventually eliminated every layer and obtained the final password by going through this method again. Ls has been used none stop as well 

```bash
ls
cat data.txt
mkdir /tmp/hetime 
cp data.txt /tmp/hetime 
cd /tmp/hetime  
man xxd
xxd -r data.txt
xxd -r data.txt > data data data.txt
file data
man gzip
mv data data.gz
gzip -d data.gz
file data
mv data data.bz2
bzip2 -d data.bz2
file data
mv data data.gz
gzip -d data.gz
file data 
mv data data.tar
man tar | grep ''xf''
tar xf data.tar
rm data tar data.txt
file data5.bin
mv data5.bin data.tar
tar xf data.tar
rm data.tar
file data6.bin
mv data6.bin databz2
bzip2 -d data.bz2
file data
mv data data.tar
tar xf data.tar
rm data.tar
file data8.bin
mv data8.bin data.gz
gzip -d data.gz
file data 
cat data 

# Password: qQYQiHOBPR8zR61qxYqX45quvihF2uzk
```

## commands used
- ls
- cat
- file
- xxd -r
- gunzip / gzip -d
- bunzip2 / bzip2 -d
- tar xf
- base64 -d
- cp
- mktemp -d

                                 
