Backup the room_files directory ///////////////// cp -r room_files room_files_backup

Delete all .txt files in room_files /////////////// rm room_files/*.txt

List and sort remaining files by size and first letter /////////////// ls -laSr | awk 'NF && !/^d/ {print $9}' | sed 's|^\./||' | sed 's/^\.//' | cut -c1 | tr -d '\n'; echo


**whatsupman**
