# For-Makerere
here will see all the commands relatd with what. we said

[] ->
cd 

->
pwd

->
vim
->
`my_var=10`
`echo $my_var`




lets Make sure you're running `bitcoind` with `-regtest`:
./bitcoind -regtest

each time you run it , there is no wallets loaded .


./bitcoin-cli -regtest listwalletdir
to check the wallet dir using the bitcoincore 

ls ~/Library/Application\ Support/Bitcoin/regtest/wallets

rm -r ~/Library/Application\ Support/Bitcoin/regtest/wallets/mywallet


to check the wallet dir using terminal


./bitcoin-cli -regtest listwallets
to check the current loaded wallets 

./bitcoin-cli -regtest createwallet "mywallet2"

 ./bitcoin-cli -regtest loadwallet "mywallet2"

./bitcoin-cli -regtest unloadwallet "mywallet2"

./bitcoin-cli -regtest -rpcwallet=mywallet2 getnewaddress

->note (check the address again restart the node)

1->bcrt1qqvz809fl94swsgcw2l03j8g08s7l56g54j7utz
2->bcrt1qm7llnurczxjwkjsd7u62hgwcch64x2u4l5d95c

🥉 Step 3: Generate Blocks to Get Coins (Mining)

./bitcoin-cli -regtest -rpcwallet=mywallet1 generatetoaddress 101 ADDRESS1

Generates 101 blocks to mature the coinbase rewards (first 100 are needed for maturity).

./bitcoin-cli -regtest -rpcwallet=mywallet1 sendtoaddress bcrt1qm7llnurczxjwkjsd7u62hgwcch64x2u4l5d95c 10

output -> transaction ID (txid)
6676a62c62ccee70618084be9f2d1cd38f64d9c3ddfadb5fe7631c3287e4fd58


./bitcoin-cli -regtest getrawtransaction 6676a62c62ccee70618084be9f2d1cd38f64d9c3ddfadb5fe7631c3287e4fd58 true

- inputs and outputs
    
- ScriptPubKey types
    
- Address outputs
    
- Block hash (if confirmed)

./bitcoin-cli -regtest -rpcwallet=mywallet1 getbalance

./bitcoin-cli -regtest -rpcwallet=mywallet2 getbalance



./bitcoin-cli -regtest -rpcwallet=mywallet1 generatetoaddress 1 ADDRESS1

./bitcoin-cli -regtest -rpcwallet=mywallet2 sendtoaddress bcrt1qqz2auqmw4zg6haldp7t8jzaehphqyn55wmmeqf 3


output -> ed7df298cbea0db8a00b338a55a6659c18738dc1cd4b830ed41f82e1a226231e

./bitcoin-cli -regtest -rpcwallet=mywallet1 generatetoaddress 1 bcrt1qqz2auqmw4zg6haldp7t8jzaehphqyn55wmmeqf

output ->524553dc7520b5d2ff5c6d077b86711031251ee6099917f04c1070ff923b7559


./bitcoin-cli -regtest -rpcwallet=mywallet1 listtransactions

