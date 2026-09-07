# Level 14 > 15

## Main task
The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

## Steps taken
First we check the if there is any files or hidden directory once I got it we used echo to print the exact string I gave it since its in port 30000 to receive the password , nc stands for netcat for a networking tool that uses TCP or UDP to read from and write to network connections followed by the localhsot which refers to my spefic machine finally the port itself to connect to which is 30000

```bash
cat /etc/bandit_pass/bandit14 

echo "aaWecNkG4FhxJQxz07uiwzVP6bJiYS65" | nc localhost 30000

# Password: pbLYuZtTg4MgaqfJx8jbA9gKKGqM68A7
```

## commands used
- ls
- cat
- echo
- nc
- 3000
- localhost

                                 
