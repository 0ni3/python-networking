# python networking

-l --listen - listen on [host]:[port] for incoming connections
-e --execute=file_to_run - execute the given file upon receiving a connection
-c --command - initialize a command shell
-u --upload=destination - upon receiving connection upload a file and write to [destination]


Examples: 
listener.py -t 192.168.0.1 -p 5555 -l -c
listener.py -t 192.168.0.1 -p 5555 -l -u=c:\\target.exe
listener.py -t 192.168.0.1 -p 5555 -l -e=\"cat /etc/passwd\
echo 'ABCDEFGHI' | ./bhpnet.py -t 192.168.11.12 -p 135
