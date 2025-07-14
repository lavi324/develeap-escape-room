https://develeap.academyocean.com/course/linux-bash-copy-copy/lesson/task-2-bash-escape-room

**Mission: Zip a file with all the passwords from all rooms and a screenshot of the last room.**



**Room 1:**
**Instructions:**
1. Navigate to the 'room_files' directory and remove all files with the '.txt' extension (It's recommended to backup the folder before proceeding)
2. Sort the remaining files by size (including hidden files) Look at the first letter of each filename to reveal a hidden message
3. Use the hidden message (in lowercase) as the password to access the next room's README file

**Commands:**

1) cp -r room_files room_files_backup && rm room_files/*.txt

2) ls -laSr | awk 'NF && !/^d/ {print $9}' | sed 's|^\./||' | sed 's/^\.//' | cut -c1 | tr -d '\n'; echo

3) **whatsupman** (password for room 2 readme file)

   

**Room 2:**
**Instructions:**

1.Find out the White Rabbit's user ID. 

2.Search the users_list file in this room for the ID from step 1.

3.Find the name of the user who has the IP that starts with this ID. 

4.Search for all the appearances of the name you found in Logs folder.

5.Sort the results (content only) by alphabetical order, you will find the key to the next room.

**Commands:**

1) cat /etc/passwd | grep -i white 

2) cat users_list | grep 521

3) cat users_list | grep 521

4) grep -ri jackie Logs/

5) grep -ri jackie Logs/ | sort -t':' -k2 | cut -d':' -f3-        //////// **472**


