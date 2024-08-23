# buffer overflow exploit lab

## usage

- compile vulnerable server 
    - `cd server-vulnerable`
    - `make`
- run the vulnerable server in gdb-peda
    - `gdb -q tcp_server`
    - `run 1233`
- prepare a reverse shell listener
    - `nc -vlp 5555`
- run the exploits in either python or node
    - `node exploit-nodejs/index.js`
    - `python exploit-python/exploit.py`

## files
- packetdump file available to see the exploit and reverse shell connection in wireshark

## credits

based on taishi8117's https://github.com/taishi8117/bof_lab/tree/master
