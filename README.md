HARMONYCOIN

Algorithm: X13
~3,479,154 Total Coins
POS & Anon
6% Annual Interest once coin becomes Pure POS
Block Height: 60 Seconds
Confirmations: 6
Block Reward: 400 coins per block
No Pre-Mine


NATIVE TOR SUPPORT

How to use TOR? (installation of TOR requirement)

Option 1: use the "-onlynet=Tor" and "-tor=IP:PORT" argument when you execute your daemon 

Option 2:

Put this in your config file:
onlynet=tor
tor=127.0.0.1:9050
addnode=any running TOR-node


HOW to setup a TOR-node:

If you have your TOR-proxy already running at localhost:9050
simply run:  ./harmonycoind -proxy=127.0.0.1:9050 -externalip=YOUR_URL.onion -listen

replace the onion address ("YOUR_URL.onion") with your own address.

NOTICE: add the following lines to your torrc file: (Unix/LINUX)
    HiddenServiceDir /Library/Tor/var/lib/tor/hidden_service/
    HiddenServicePort 80 127.0.0.1:8080

On Windows: 
    HiddenServiceDir C:\Users\username\Documents\tor\hidden_service
    HiddenServicePort 80 127.0.0.1:8080
    
Now save the torrc and restart your tor.
Tor will now create the HiddenServiceDir that you specified above and
add two files to them.

"private_key" & "hostname"

"hostname" = your onion-address. 

NEVER PUBLISH YOUR PRIVATE KEY!!! (if you do everybody will be able to impersonate your hidden service.



