Backup the room_files directory / cp -r room_files room_files_backup
Delete all .txt files in room_files / rm room_files/*.txt
List and sort remaining files by size and first letter / ls -1aS room_files | grep -v '^d' | tail -n +2 | while read f; do echo -n "${f:0:1}"; done; echo
**whatsup**
