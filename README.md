https://develeap.academyocean.com/course/linux-bash-copy-copy/lesson/task-2-bash-escape-room

**Mission: Zip a file with all the passwords from all rooms and a screenshot of the last room.**

**Room 1:**

Backup the room_files directory ///////////////// cp -r room_files room_files_backup

Delete all .txt files in room_files /////////////// rm room_files/*.txt

List and sort remaining files by size and first letter /////////////// ls -laSr | awk 'NF && !/^d/ {print $9}' | sed 's|^\./||' | sed 's/^\.//' | cut -c1 | tr -d '\n'; echo

**whatsupman** (password for room 2 readme file)

**Room 2:**
**Instructions:**

1.Follow the white rabbit!....Find out the White Rabbit's user ID . Hint: read about users in Linux.
2.Search the users_list file in this room for the ID from step 1.
3.Find the name of the user who has the IP that starts with this ID. Hint: use find/grep/cat/vim and etc.
4.Search for all the appearances of the name you found in Logs folder.
5.Sort the results (content only) by alphabetical order, you will find the key to the next room.
