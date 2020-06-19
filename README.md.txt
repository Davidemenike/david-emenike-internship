# OverTheWire Bandit Wargame

## Level 0

### Description
Enter the username and password at port 2220 given to progress

### Solution
Username bandit0
password bandit0

---

## Level 1

### Description
looking for the password in our readme file


### Solution
using the ls and cat function, we see the password is contained in the readme file: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
We can copy and paste this in the appropriate postion using SHIFT + ctrl C / V

---

## Level 2

### Description
password is located in '-' named file in the home directory of bandit1


### Solution
solution was to have the ./ key placed before the dash to actually open the file and get the password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

---

## Level 3

### Description
password was located in a file that was named a group of words

### Solution
simply putting  (" ") quotation marks while trying to cat the file will display the password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

---

## Level 4

### Description
password is located in a hidden file 

### Solution
using the ls function and "-a", we uncover all hidden files in the directory and open to see our password: pIwrPrtPN36QITSp3EQaw936yaFoFgAB

---

## Level 5

### Description
password is located in one of 10 possible files

### Solution
by using the "file ./-file*", we reveal the content of all the 10 files and find out that only 1 has the ASCII password: koReBOKuIDDepwhWk7jZC0RTdopnAYKh

---

## Level 6

### Description
looking for a partcualir file with specific attributes out of several other files

### Solution
using the find command we can look specifically for the file with 1033 bytes and find our password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7

---

## Level 7

### Description
similar to last problem. Looking for specific file with special atrribues

### Solution
by using the find command and inputing the attrivutes we're looking for we find a location of where our password is : HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

---

## Level 8

### Description
giving a text document, we have to scan for a particular word "millionth" which has our password beside it

### Solution
using the grep command we can call a specific word out of the whole text and see our password beside it

---

## Level 9

### Description
similar to the previous one, we are given a data text filled with repeated text and only one line has a non repeated text which is our password

### Solution
by using the sort command we organise everything and see the only single text or by using the uniq function, we pull out the line of code that is not repeated
password : UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

---

## Level 10

### Description
the password is located in a text document mostly filled with unreadable text

### Solution
by using the strings command as well as the grep for the equal sign, we locate our password as on of the only readable texts there : truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk 

---

## Level 11

### Description
the password to this level is encrypted as a bas64 text 

### Solution
by using the base64 -d command, we decrypt our password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

---

## Level 12

### Description
password is located in a text document that has being encrypted in a ROT13 format 

### Solution
we simply copy the content of our data text and decrypt it in the ROT13.com decryptor 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

---

## Level 13

### Description
password is stored in a compressed file 

### Solution
by moving the file to our own directory, there using gzip and zcat, we can unzip and decompress the file multiple times till we get our password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL

---

## Level 14

### Description
for this level, instead of looking for a password, we are to find a private key that will link us to the next level

### Solution
using the ssh command and -i, we take the private key given to us and link our way to the next level

---

## Level 15

### Description
the password is located in the file given to us in the previous level. 

### Solution
simply open it and we get our password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e then later we use the netcat command with our destination and 
password to get us to this password :BfMYroe26WYalil77FoDi9qh59eK5xNr

---

## Level 16

### Description
password from last level on port 30001

### Solution
insert the password when found cluFn7wTiGryunymYOu4RcffSxQluehd

---

## Level 17

### Description

### Solution


---

## Level 18

### Description
given two we just have to use the diff command to see lines that have been changed 
### Solution
using the diff on the two passwords, we see the different ones and find our password: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd

---

## Level 19

### Description
level will automatically shut you out the moment you login but the password is in the home directory

### Solution
since the password is right in the home, we can use the cat command on the readme file simultaneously while logging in and we get our password: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x

---

## Level 20

### Description
bandit-20 file that contains password


### Solution
from inside the bandit-20 file, we can cat the file and try to open up the specific password we're looking for:GbKksEFF4yrVs6il55v6gwY5aVje5f0j

---

## Level 21

### Description



### Solution
placing a port in our suconnect and using the -l to listen, we find our password: gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr
---

## Level 22

### Description
We're looking in a particular directory that contains running files in which our password is in

### Solution
as we open our etc/cron.d directory, we focus our motives on the bandit 22 root that we're looking for and find the password in the usr bin : Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI 

---

## Level 23

### Description
similar to previous level, looking for the particular directory that contains password

### Solution
a little different this time. Our bandit 23 root opens up and echo that when we copy and repeat, gives us the file that then contains the password: jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n

---

## Level 24

### Description
Our password to this level is located in an etc directory from cron 

### Solution
we make a new directory after openning the bandit24 file, create our shell script and copy it back to the new directory we make and wait for the password to copy over: UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ

---

## Level 25

### Description
We're looking for a random four digit pin to add to our password from the previous level to get to the next level

### Solution
in our shell file that we will make, we create a for loop which will insert every possible four digit combination possible and eventually end up with the password: uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG

---

## Level 26

### Description
while looking for our password, our shell file cannot contain /bin/bash like the last one

### Solution
we shrink down our screen when trying to use the bandit26 sshkey so when the screen can't show the rest, we :e the shell file and input our password location and it gets displayed: 5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z

---

## Level 27

### Description
similar to the last one, we keep getting shut our of our 26 bandit so we apply the same method

### Solution
reduce the screen size so the program can't run fully, then in the vim file, we represent the shell file with bandit 26 and this puts us in. Then all we have to do is cat the bandit 27 password file i.e /etc/bandit_pass/bandit27: 3ba3118a22e93127a4ed485be72ef5ea 

---

## Level 28

### Description
we have to clone a repository in our bandit 27 and find the password

### Solution
first, we make a new directory in the tmp directory and we clone the repo in there and input our password for bandit 27. We get a repo directory that contains a readme file with our password: 0ef186ac70e04ea33b4c1853d2526fa2

---

## Level 29

### Description
quite similar to the laast one except the READme file doesn't contain a password

### Solution
after literally following the exact steps from the last one, we git our bandit 28 mode to see all the past commits that have been done, then we git show the very first one that gives us a username and a password: bbc96594b4e001778eee9975372716b2

---

## Level 30

### Description
password is not displayed in the READme file of the git cloned repo

### Solution
if we log on to the git of our repo, we see a bunch of commits that have been created while ago. At the very end, we see the original README.md file that was created. By opening this file we get our password: 5b90576bedb2cc04c86a9e924ce42faf

---

## Level 31

### Description
Our README.md file is nothing but an empty file. THe password is hidden

### Solution
Since none of our git shown commit files works, we look for the tag which says secret. Fairly easy we just open the tag and we get our password: 47e603bb428404d265f59c42920d81e5

---

## Level 32

### Description
we have to push a txt file that should contain some words into a remote directory

### Solution
in our repo directory, we create a txt file that contains the specified words. Then we comit it and push it up and input our old password to confirm and get the new one: 56a9bf19c63d650ce78e6ec0354ee45e

---

## Level 33

### Description
we are in an UPPERCASE shell and need to get back to the bash shell

### Solution
by inputing the dollar sign and zero we start of the process of recovering back. THen by using the right positional parameters and exporting SHELL as our /bin/bash. Simply echo this and open the etc/banditpass to get our password: c9c3199ddf4121b10cf581a98d51caee

---

## Level 34

### Description


### Solution