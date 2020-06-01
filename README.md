# client-server-socket
to run this program:
gcc -o server server.c
gcc -o client client.c
open 2 terminals run server - ./server then in the other terminal run client - ./client

to change packet loss:
sudo apt install iproute
sudo tc qdisc add dev lo root netem loss xx%

to disable packet loss:
sudo tc qdisc del dev lo root netem
