# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
### Display the content of the files
cat < file1
## OUTPUT
<img width="423" height="443" alt="Screenshot 2026-07-31 212230" src="https://github.com/user-attachments/assets/ef190a4f-820b-45f8-b2f0-321ea0e37fc6" />





cat < file2
## OUTPUT
<img width="375" height="167" alt="Screenshot 2026-07-31 212141" src="https://github.com/user-attachments/assets/a4c83668-95f0-4710-9f64-dde1681d0d0b" />



# Comparing Files
cmp file1 file2
## OUTPUT
<img width="399" height="119" alt="Screenshot 2026-07-31 212344" src="https://github.com/user-attachments/assets/2de6d99b-1bd7-4c54-85e2-c5852dfecb45" />

 
comm file1 file2
 ## OUTPUT
<img width="386" height="249" alt="Screenshot 2026-07-31 212417" src="https://github.com/user-attachments/assets/b14d2e6d-dafa-450a-9310-f4c9d555a6ff" />

 
diff file1 file2
## OUTPUT
<img width="407" height="317" alt="Screenshot 2026-07-31 212435" src="https://github.com/user-attachments/assets/c09cdc15-6950-479e-8fb3-88fbef59c68c" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
<img width="388" height="276" alt="Screenshot 2026-07-31 212523" src="https://github.com/user-attachments/assets/cb5f185c-3797-41fc-b6ba-a2048ec9e2cd" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
<img width="385" height="359" alt="Screenshot 2026-07-31 212554" src="https://github.com/user-attachments/assets/762c66ec-5480-4c9f-a100-81c7c6f87a97" />



cut -c1-3 file11
## OUTPUT
<img width="366" height="212" alt="Screenshot 2026-07-31 212618" src="https://github.com/user-attachments/assets/626289ea-8211-4cc8-b2ee-d8ef0a7aedfd" />





cut -d "|" -f 1 file22
## OUTPUT
<img width="359" height="131" alt="Screenshot 2026-07-31 212749" src="https://github.com/user-attachments/assets/ec292256-c08d-4043-b23e-dc4c6d9907ff" />





cut -d "|" -f 2 file22
## OUTPUT
<img width="405" height="124" alt="Screenshot 2026-07-31 212637" src="https://github.com/user-attachments/assets/905f5940-56bd-4152-85e2-33d7e4db91d9" />


cat < newfile 
```
Hello world
hello world
^d
````

<img width="446" height="101" alt="Screenshot 2026-07-31 212822" src="https://github.com/user-attachments/assets/917f1617-20bd-4437-84d4-c5afb4315cec" />

cat > newfile 
Hello world
hello world



grep Hello newfile 
## OUTPUT
<img width="411" height="69" alt="Screenshot 2026-07-31 223219" src="https://github.com/user-attachments/assets/7f740600-e01f-4e19-80a2-023b817ec2cd" />






grep hello newfile 
## OUTPUT
<img width="343" height="81" alt="Screenshot 2026-07-31 223238" src="https://github.com/user-attachments/assets/50fdec5b-260a-4338-9879-4d1fc6ac49fd" />



grep -v hello newfile 
## OUTPUT
<img width="288" height="51" alt="Screenshot 2026-07-31 232824" src="https://github.com/user-attachments/assets/296b3d35-6911-4c36-a5b0-19eea25a13a1" />




cat newfile | grep -i "hello"
## OUTPUT
<img width="402" height="137" alt="Screenshot 2026-07-31 234008" src="https://github.com/user-attachments/assets/33a575c7-320f-4e3c-8860-aa2460c0abd4" />





cat newfile | grep -i -c "hello"
## OUTPUT
<img width="439" height="84" alt="image" src="https://github.com/user-attachments/assets/adab795f-bed3-4aaf-8944-92f20d0b9bd0" />





grep -R ubuntu /etc
## OUTPUT
<img width="1430" height="754" alt="image" src="https://github.com/user-attachments/assets/58886adb-1972-493b-8088-3a6f1bec7a4e" />
<img width="1347" height="825" alt="image" src="https://github.com/user-attachments/assets/9e406197-7939-40b3-bb32-8f8839c8dfcf" />
<img width="1475" height="802" alt="image" src="https://github.com/user-attachments/assets/8ec82c90-adcc-4653-b33a-283a19847b7d" />

<img width="1657" height="823" alt="image" src="https://github.com/user-attachments/assets/53b214b2-cc11-44c3-a4bc-59c22eaac4cb" />

<img width="948" height="755" alt="image" src="https://github.com/user-attachments/assets/fce96369-4d1d-47eb-b2d3-ddcf94a7d4f7" />



grep -w -n world newfile   
## OUTPUT
<img width="391" height="99" alt="image" src="https://github.com/user-attachments/assets/026b049e-b631-48aa-8791-b67ca2aebc3b" />





cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```


cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```

<img width="388" height="451" alt="image" src="https://github.com/user-attachments/assets/8e3e80b7-f097-4e6e-a491-2d37ed9f54b6" />


egrep -w 'Hello|hello' newfile 
## OUTPUT
<img width="397" height="102" alt="image" src="https://github.com/user-attachments/assets/5b56d7f8-c6d0-41cd-843b-adeb8b758398" />





egrep -w '(H|h)ello' newfile 
## OUTPUT
<img width="393" height="106" alt="image" src="https://github.com/user-attachments/assets/162d6fb0-9579-427a-85dd-616115bc5e40" />




egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT
<img width="420" height="104" alt="image" src="https://github.com/user-attachments/assets/697c051f-f807-41a3-bf76-6162bb94605b" />





egrep '(^hello)' newfile 
egrep '(world$)' newfile 
egrep '(World$)' newfile 
egrep '((W|w)orld$)' newfile 
## OUTPUT
<img width="397" height="380" alt="image" src="https://github.com/user-attachments/assets/5edd4bf3-fb84-4aeb-9e09-18fde43518fa" />




egrep '[1-9]' newfile 
egrep 'Linux.*world' newfile 
egrep 'Linux.*World' newfile 
egrep l{2} newfile
egrep 's{1,2}' newfile
## OUTPUT 
<img width="388" height="519" alt="image" src="https://github.com/user-attachments/assets/297cc375-d7f4-4a1d-af99-7c0f3da5f627" />



cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```
<img width="340" height="244" alt="image" src="https://github.com/user-attachments/assets/a3c4788f-8fbc-4859-a525-a2cc90f8fa33" />



sed -n -e '3p' file23
sed -n -e '$p' file23
sed  -e 's/Ram/Sita/' file23
sed  -e '2s/Ram/Sita/' file23
sed  '/tom/s/5000/6000/' file23
sed -n -e '1,5p' file23
sed -n -e '2,/Joe/p' file23
sed -n -e '/tom/,/Joe/p' file23
## OUTPUT
<img width="470" height="741" alt="image" src="https://github.com/user-attachments/assets/005b4bb4-2da6-4ccc-9f95-f92902cb2454" />
<img width="445" height="466" alt="image" src="https://github.com/user-attachments/assets/d5321c06-8574-4c0a-8cd3-f1d7fbbaa45c" />




seq 10 
seq 10 | sed -n '4,6p'
seq 10 | sed -n '2,~4p'
## OUTPUT
<img width="433" height="546" alt="image" src="https://github.com/user-attachments/assets/f2a893e1-1985-47f5-8bcf-505ae6ac991c" />



seq 3 | sed '2a hello'
seq 2 | sed '2i hello'
seq 10 | sed '2,9c hello'
## OUTPUT
<img width="401" height="396" alt="image" src="https://github.com/user-attachments/assets/739ce829-820e-4a14-9b12-12ac1db5086c" />



sed -n '2,4{s/^/$/;p}' file23
sed -n '2,4{s/$/*/;p}' file23




#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
 ## OUTPUT
<img width="465" height="705" alt="image" src="https://github.com/user-attachments/assets/54d56d23-3df9-4ff4-a1a6-9ad308b156d5" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22




#Using tr command

cat file23 | tr [:lower:] [:upper:]


cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT
 <img width="487" height="758" alt="image" src="https://github.com/user-attachments/assets/f0f56ecb-b3e3-4346-89d7-bc6a303e920f" />



 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT
<img width="546" height="504" alt="image" src="https://github.com/user-attachments/assets/0dd6f03b-3007-44fa-9df0-69b78633c1c5" />



#Backup commands
tar -cvf backup.tar *

mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
tar -xvf backup.tar
## OUTPUT
<img width="661" height="658" alt="image" src="https://github.com/user-attachments/assets/ff3f11ba-aea6-4da7-aa96-5704c9ad5f4a" />


gzip backup.tar

ls .gz
<img width="2172" height="724" alt="image" src="https://github.com/user-attachments/assets/c73fd1be-126a-4f25-a826-74c5b1c72a3c" />

 
gunzip backup.tar.gz
## OUTPUT
<img width="272" height="224" alt="image" src="https://github.com/user-attachments/assets/cdd7ced6-11e3-416b-8e58-86f13235dcd4" />

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT
<img width="228" height="216" alt="image" src="https://github.com/user-attachments/assets/9cc0c7ad-1dc1-4937-89b6-6533e39b76e6" />



 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT
<img width="475" height="274" alt="image" src="https://github.com/user-attachments/assets/1fc0c955-4949-40bd-bd17-b6754d90e24b" />





cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
<img width="1428" height="1101" alt="image" src="https://github.com/user-attachments/assets/56ffb9f5-5c16-408b-bca8-8c0fbe445ad5" />



 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 

abcd
 
echo $?
 ## OUTPUT



 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
##OUTPUT
<img width="451" height="336" alt="Screenshot 2026-08-01 001746" src="https://github.com/user-attachments/assets/6dbff509-f94a-44c1-812f-2748f382f786" />




chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT
<img width="778" height="99" alt="Screenshot 2026-08-01 001718" src="https://github.com/user-attachments/assets/48e32ecb-2e54-46e9-ab43-841d0ee60166" />


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
<img width="838" height="106" alt="Screenshot 2026-08-01 001641" src="https://github.com/user-attachments/assets/58af86b0-91c5-418c-8c4a-f6e09f231be9" />


# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT
<img width="829" height="147" alt="Screenshot 2026-08-01 001620" src="https://github.com/user-attachments/assets/7e3e1eb4-39f6-4e1b-98d6-cb896cba2506" />




# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
##OUTPUT
<img width="829" height="147" alt="Screenshot 2026-08-01 001620" src="https://github.com/user-attachments/assets/7e3e1eb4-39f6-4e1b-98d6-cb896cba2506" />


# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
##OUTPUT
<img width="873" height="156" alt="Screenshot 2026-08-01 001601" src="https://github.com/user-attachments/assets/750f3c59-3d57-47f5-a139-f01a6aa85c58" />


# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
<img width="858" height="145" alt="Screenshot 2026-08-01 001543" src="https://github.com/user-attachments/assets/c5186bba-9125-4e2e-8f87-f507051b3201" />



# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
<img width="849" height="88" alt="Screenshot 2026-08-01 001501" src="https://github.com/user-attachments/assets/c0683481-544e-478a-a894-838de5b4c7a4" />

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh
 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
<img width="437" height="367" alt="Screenshot 2026-08-01 001435" src="https://github.com/user-attachments/assets/ca3da067-edd8-4944-9a30-13951b80da2c" />

 
 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 <img width="861" height="272" alt="Screenshot 2026-08-01 001420" src="https://github.com/user-attachments/assets/8c821d1c-a34f-437d-99dc-e59c50f2f461" />

 
 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
<img width="820" height="313" alt="Screenshot 2026-08-01 001346" src="https://github.com/user-attachments/assets/a548bff6-ba40-489d-b181-c172f0466272" />

 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
<img width="415" height="241" alt="Screenshot 2026-08-01 001320" src="https://github.com/user-attachments/assets/0671b638-90a2-4f37-a1ae-e45b6a6e9dcb" />

cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT
<img width="820" height="313" alt="Screenshot 2026-08-01 001346" src="https://github.com/user-attachments/assets/09ff25bd-3780-4937-94ff-52e2b856cc5f" />



cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
<img width="206" height="105" alt="Screenshot 2026-08-01 001256" src="https://github.com/user-attachments/assets/4d5604e1-911e-4090-b49e-4a77af147d26" />


cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
<img width="206" height="105" alt="Screenshot 2026-08-01 001256" src="https://github.com/user-attachments/assets/35e39dca-f46b-4acb-95be-8f428b86b85d" />


cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT
 <img width="362" height="386" alt="Screenshot 2026-08-01 001234" src="https://github.com/user-attachments/assets/93289ad7-e3d1-4439-81db-3b53480075d3" />


 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT
<img width="362" height="386" alt="Screenshot 2026-08-01 001234" src="https://github.com/user-attachments/assets/92265cde-1e5c-4240-9c9a-44cc8825dcb0" />


$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
<img width="778" height="161" alt="Screenshot 2026-08-01 001200" src="https://github.com/user-attachments/assets/4452527f-6d28-487c-ac71-37f47e79726a" />

 
cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 



 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 
 <img width="523" height="200" alt="Screenshot 2026-08-01 001133" src="https://github.com/user-attachments/assets/8c1611b0-d184-49a4-ad8d-6c38ffbde12d" />

 

 
 ./funcex.sh 1 2
<img width="1716" height="917" alt="image" src="https://github.com/user-attachments/assets/f3d80b43-1563-4c48-84e7-cff5aea34cbe" />


 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
<img width="1718" height="915" alt="image" src="https://github.com/user-attachments/assets/329ce215-d989-4026-a437-978e609ae1c8" />

 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 <img width="574" height="267" alt="Screenshot 2026-08-01 001100" src="https://github.com/user-attachments/assets/f781bb0c-823c-4161-a543-f04eafbdc469" />

 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
<img width="485" height="416" alt="Screenshot 2026-08-01 001017" src="https://github.com/user-attachments/assets/4440666c-55a2-4b62-a1ad-2f7a3f60d875" />

 
cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 
<img width="602" height="610" alt="image" src="https://github.com/user-attachments/assets/1c17dd7c-1d30-4710-b653-4d2d99202b74" />

<img width="436" height="224" alt="image" src="https://github.com/user-attachments/assets/f1e28587-eabe-444c-b12f-47082542d944" />




# RESULT:
The Commands are executed successfully.
