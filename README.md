## Linux-Network&Command-Notes

1. Identify the service on port -> i.e :list the port 80

$ netstat -tulpn | grep --color :80

-----------------------------------------------------------------------

2. All port listed

$ lsof -i 

$ lsof -i :<port_number>

-----------------------------------------------------------------------

3. Kill the service working on ports

$ fuser -k 80/tcp

-----------------------------------------------------------------------

4. Find the large file in the given directory

$ find <path_of_direc>  -size +10000k

-----------------------------------------------------------------------

5. Search a file for a pattern of characters, then display all matching lines.

$ grep [options] pattern [files]

For example, grep directory recursively:
$ grep -r "texthere" /home/

For example, grep the word printf:
$ grep printf /path/filename.txt

For example, find previously used commands which include systemctl
$ history | grep systemctl

For example, find the last login(s) for username:
$ last | grep username

-----------------------------------------------------------------------
