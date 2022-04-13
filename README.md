
## Server
**gcc s.c -L/usr/local/v6/lib -lm -lsctp -o server**
<!-- parameter 2 is the maximum number of input streams, parameter 3 is the number of output streams -->
**. /server 5 100 10**

## Client
gcc c.c -L/usr/local/v6/lib -lm -lsctp -o client
<!-- parameter 2 is the server address, parameter 3 is the maximum number of input streams, parameter 4 is the number of output streams, parameter 5 must be less than parameter 4-->
. /client 192.168.124.4 100 81 8
