# Assignment-4
**Ques 1: Create a directory named "MyFiles" in your home directory. Navigate into this directory and list its contents.**

``` 
cd /home
```
```
sudo mkdir MyFiles
```
```
cd MyFiles
```
```
 ls
```

**Output**

![Screenshot from 2024-02-03 20-54-45](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/1dfb67c7-c8b6-47ed-8ded-55947a7282d7)


**Ques 2: Copy a file named "document.txt" from your home directory to the "MyFiles" directory. Move the file to a subdirectory named "Documents" within "MyFiles."**

``` 
cd /home
```
```
sudo touch document.txt
```
```
sudo cp document.txt MyFiles/
```
```
cd MyFiles/
```
```
sudo mkdir -p Document
```
```
sudo mv MyFiles/document.txt MyFiles/Document
```

**output**


![Screenshot from 2024-02-03 21-13-59](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/c1b76cee-36c4-44f5-ab5b-dc6124b36972)


**Ques 3 : Create an empty file named "notes.txt" in the "MyFiles" directory. Afterward, delete the file.**

``` 
cd /home/MyFiles/
```
```
sudo touch notes.txt
```
```
sudo rm -rf notes.txt
```



**Output**


![Screenshot from 2024-02-03 21-17-39](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/6fc629a1-7e45-4148-9716-c90982a7aeac)


**Ques 4 : Create a hard link named "hardlink.txt" for the file "document.txt" within the "Documents" subdirectory. Also, create a symbolic link named "symlink.txt" in the same location.**

```
cd /home/MyFiles/Document
```
```
ln document.txt hardlink.txt
```
```
ln -s document.txt symlink.txt
```
**Output**


**Ques 5 : In the "MyFiles" directory, use a single command to list all files that start with the letter "a" and have a ".txt" extension.**

```
sudo ls /home/MyFiles/a*.txt
```

**Output**


![Screenshot from 2024-02-03 21-20-42](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/bfe7b4d3-be67-4b30-9143-f54f557d47bd)


**Ques 6: Rename all files in the "Documents" subdirectory of "MyFiles" with a ".bak" extension. Ensure the original file names are preserved.**

```
cd /home/MyFiles/Document
```
```
sudo touch a.txt b c.txt d.txt
```
```
sudo rename -n 's/\.txt$/.bak/' *.txt
```
```
sudo rename 's/\.txt$/.bak/' *.txt
```
**Output**


![Screenshot from 2024-02-03 21-26-16](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/63353f70-652a-43cf-a77d-203a0295cb03)



**Ques 7: Use a wildcard character to copy all files from the "Documents" subdirectory of "MyFiles" to another directory named "Backup."**

```
cd /home
```
```
cd MyFiles
```
```
sudo mkdir backup
```
```
cd
```
```
sudo cp /home/MyFiles/Document/* /home/MyFiles/backup/
```

**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/80763311-395c-4e74-a235-d73e7ec21508)

**Ques 8 :Execute the ls command to list files in the current directory. Save the output to a file named "file_list.txt." Then, use a pipe to filter the output through grep to display only files with a ".txt" extension.**

```
sudo su
```
```
cd /home/MyFiles/
```
```
touch file_list.txt
```
```
cd Document
```
```
chmod +rwx a.txt b
```
```
cd ..
```
```
chmod +rwx file_list.txt
```
```
cd Document
```
```
ls > ../file_list.txt
```
```
grep '\.txt$' file_list.txt
```

**Output**




![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/56cfb342-9a88-4e5b-bc4a-fc7a74ca86eb)

**Ques 9: Create a new text file named "my_notes.txt" using the touch command. Open the file in the Vim editor, add some text, and save the changes.**
```
cd /home/MyFiles/
```
```
sudo touch my_notes.txt
```
```
sudo vim my_notes.txt
```
**Output**



![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/288bbedf-7571-437c-bae9-03c1cb8ea40b)


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/3a3a5a25-2e44-4faf-a8c2-da446a3b3d1a)

**Ques 10 :Run the date command and store the output in a variable named "current_date." Display the value of the variable and append it to the "my_notes.txt" file.**

```
cd /home/MyFiles/
```
```
sudo su
```
```
current_date=$(date)
```
```
echo "current date : $current_date"
```
```
echo "$current_date" >> my_notes.txt
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/5d680281-1960-4247-87cf-775fa2c9b33a)


![Screenshot from 2024-02-03 23-13-13](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/be42316d-140e-4894-9617-71b9914955dc)


**Ques 11 : Edit the Bash startup script (e.g., .bashrc) to set an environment variable named "CUSTOM_PATH" to a specific directory path. Ensure the variable is available in new shell sessions.**
```
vim .bashrc
```
```
export CUSTOM_PATH="/home/MyFiles/Document"
```
```
source ~/.bashrc
```
```
echo $CUSTOM_PATH
```
**Output**

![Screenshot from 2024-02-02 14-08-23](https://github.com/MOINUDDIN0786/Linux-Assignment-4/assets/64195957/4e3eb4d2-84aa-4618-9db8-baf1270593f4)


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/e6a99e1e-a3df-4a0f-824d-255b8fb74047)

**Ques 12 : Use the echo command to add a new line of text to the "my_notes.txt" file without overwriting existing content. Verify that the new text is appended.**

```
cd /home/MyFiles
```
```
sudo su
```
```
echo "I am writing text in new line" >> my_notes.txt
```
```
cat my_notes.txt
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/6bd417d7-646f-45a7-bafb-3a9c3975632e)

**Ques 13 : List all files in the "/etc" directory, filter the output to include only those containing the word "conf," and save the result to a file named "conf_files.txt."**

```
ls /etc | grep 'conf' > conf_files.txt
```
```
vim conf_files.txt
```
**Ques 14 : Open the "my_notes.txt" file in Vim. Use Vim's search and replace functionality to replace all occurrences of the word "important" with "critical." Save the changes.**

```
cd /home/MyFiles
```
```
sudo vim my_notes.txt
```
**After opening file write below  command after press shift + colon
```
%s/important/critical/g
```
**Output**

![Screenshot from 2024-02-03 10-39-06](https://github.com/MOINUDDIN0786/Linux-Assignment-4/assets/64195957/b519ffe1-db4e-4530-8ac2-45400c9cd356)


**Ques 15 : Create a new user account named "john_doe." Set the user's home directory to "/home/john_doe" and assign the user to the "users" group.**

```
sudo useradd -m -d /home/john_doe -g users john_doe
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/eeb67481-6fd7-40d1-9a70-64e0f640b6d0)

**Ques 16 : Add the user "john_doe" to the sudoers file, allowing them superuser privileges. Confirm that "john_doe" can execute commands with sudo.**

```
sudo visudo
```
**Inside visudo file write below content and save it and exit**

```
john_doe ALL=(ALL:ALL) ALL
```
**Write any desire path**
```
sudo ls /Desktop
```
```
sudo su
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/9709ffdf-358b-4954-9be3-66804256f124)

**Ques 17 :Modify the user account "john_doe" to change the default shell to "/bin/bash" and set the account's expiration date to one month from today.**

```
sudo chsh -s /bin/bash john_doe
```
```
sudo chage -E $(date -d "+1 month" +"%Y-%m-%d") john_doe
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/6037a588-7d36-451d-af6f-b3d9a20f46c7)


**Ques 18 :Create a new group named "development_team." Add "john_doe" to this group and verify the group's existence.**

```
sudo groupadd development_team
```
```
sudo usermod -aG development_team john_doe
```
```
getent group development_team
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/a4471702-5104-4ecc-8a3e-d32b67d5211b)

**Ques 19 : Remove "john_doe" from the "users" group and add them to the "development_team" group. Confirm the changes.**

```
sudo gpasswd -d john_doe users
```
```
sudo usermod -aG development_team john_doe
```
```
groups john_doe
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/4e1ad7ed-f38d-4e6e-92f5-5aa9de3a4744)

**Ques 20 :Delete the user account "john_doe" and ensure that their home directory is also removed.**

```
sudo userdel -r john_doe
```
```
groups jhon_doe
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/cd088c15-b370-4d98-9a3a-4a50163093ed)

**Ques 21 : Delete the group "development_team" and ensure that all users previously belonging to the group are appropriately handled.**

```
getent group development_team
```
```
sudo usermod -g users jhon_doe
```
```
sudo groupdel development_team
```
```
getent group development_team
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/a8f1bcc3-f100-4f47-8070-8765adfe92b2)


**Ques 22 : Implement a password policy that requires users to change their passwords every 90 days. Apply this policy to all existing and new user accounts.**

```
sudo chage -M 90 -m 0 -W 7 -I 30 -E -1 $(cut -d: -f1 /etc/passwd)
```
```
sudo vim /etc/login.defs
```
**Inside this file add max pass day as 90 and min pass day as 0**

```
PASS_MAX_DAYS   90
PASS_MIN_DAYS   0
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/4367d0db-b1c8-4ef3-9337-30607f21cb9c)



![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/306fa487-69b1-4bdb-8de4-79a76ab76919)

**Ques 23 : Manually lock the user account "john_doe." Attempt to log in as "john_doe" to confirm that the account is locked. Then, unlock the account.**

```
sudo passwd -l john_doe
```
```
su - john_doe
```
```
sudo passwd -u john_doe
```
**Output**


![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/07c93f99-8899-4522-b222-0c9ad33d6ff8)

**Ques 24 : Use the id command to display detailed information about the "john_doe" user, including user ID, group ID, and supplementary groups.**

```
id john_doe
```
```
id -u john_doe
id -g john_doe
```
```
id -G john_doe
```
**Output**

![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/a3c49f1a-b36c-404f-8881-dd44f5b162e5)


**Ques 25 : Configure the password aging for the user "john_doe" to enforce a maximum password age of 60 days. Confirm that the changes take effect.**

```
sudo chage -M 60 john_doe
```
```
sudo chage -l john_doe
```
**Output**



![image](https://github.com/mrhimanshuydv03/Himanshu/assets/153823337/d356abad-20b7-48fd-b2ba-c60962a9e21d)
