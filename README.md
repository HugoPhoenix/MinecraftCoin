MinecraftCoin(MCC) is a peer-to-peer cryptocurrency. MinecraftCoin uses proof-of-stake and proof-of-work systems and is open-source. Aimed to connect all Minecraft server with MinecraftCoin, unite the Players Community and we are going to setup a platform that people can buy and sell map, skin, plugin, mod, etc. on it using the coin.

Use the following instructions to set up the wallet (Linux)

wget "https://github.com/HugoPhoenix/MinecraftCoin/releases/download/v1.0.0.0/minecraftcoin-daemon-linux.tar.gz" -O minecraftcoin-daemon-linux.tar.gz

tar -xzvf minecraftcoin-daemon-linux.tar.gz

sudo mv minecraftcoind /usr/bin/

mkdir $HOME/.minecraftcoin
nano $HOME/.minecraftcoin/minecraftcoin.conf

Paste the following lines in minecraftcoin.conf.

rpcuser=xxx
rpcpassword=xxx
rpcallowip=127.0.0.1
listen=1
server=1
txindex=1
staking=0
daemon=1

Start your node with the following command.

minecraftcoind



Use the following instructions to set up the wallet (Window)

Open your wallet, and make sure your wallet is connected with a node.
Your wallet is connected when you see the icon  in the lower corner of your wallet.

Close your wallet and create the file minecraftcoin.conf in the folder “%APPDATA%\minecraftcoin\”.

Paste the following text(replace xxx) into minecraftcoin.conf and save the file.

rpcuser=xxx
rpcpassword=xxx
rpcallowip=127.0.0.1
rpcport=27731
listen=1
server=1
addnode=node1.minecraftcoin.online
addnode=node2.minecraftcoin.online
addnode=node3.minecraftcoin.online
