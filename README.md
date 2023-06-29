cd ~
mkdir althea
mkdir althea-bin
cd althea-bin
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/althea-0.0.3-4-g30eddc7-linux-amd64
mv althea-0.0.3-4-g30eddc7-linux-amd64 althea
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/client
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/orchestrator
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/register-delegate-keys
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/relayer
chmod +x *
sudo mv * /usr/bin/
cd ~/althea
althea init nodesguru --chain-id althea-testnet1v4
althea keys add nodesguru – that is the name of node
wget https://github.com/althea-net/althea-chain/releases/download/v0.0.4/althea-testnet1-v4-genesis.json
cp althea-testnet1-v4-genesis.json $HOME/.althea/config/genesis.json
