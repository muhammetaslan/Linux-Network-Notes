# Linux-Network-Notes
Linux Network Notes

1. Identify the service on port

list the port 80

$ netstat -tulpn | grep --color :80

alternative

all port listed

$ lsof -i 

$ lsof -i :<port_number>

2. Kill the service working on ports

$ fuser -k 80/tcp
