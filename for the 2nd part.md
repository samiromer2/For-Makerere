📅 1-Hour Regtest Bitcoin Session Plan
0–5 min: Introduction & Context

    Command: (none, just explain)

    Target:

        Make sure students understand why regtest exists.

        Relate to real Bitcoin, but explain the difference.

    Why:

        Without context, the commands will feel like random terminal magic.

    Emphasize:

        Regtest = private, instant, free test environment.

        Same rules as Bitcoin mainnet, but without the risks.

    Goal:

        Students see regtest as a safe playground for learning.

5–15 min: Wallet Basics

    Command:

    ./bitcoin-cli -regtest listwalletdir
    ./bitcoin-cli -regtest createwallet "mywallet1"
    ./bitcoin-cli -regtest loadwallet "mywallet1"
    ./bitcoin-cli -regtest -rpcwallet=mywallet1 getnewaddress

    Target:

        Understand wallets as key managers.

        Get their first Bitcoin address.

    Why:

        Without a wallet, no Bitcoin can be stored.

    Emphasize:

        Wallet ≠ coins. Wallet = keys + addresses.

        Address is public, private key is secret.

    Goal:

        Students create their own wallets and addresses.

15–25 min: Mining Coins

    Command:

    ./bitcoin-cli -regtest -rpcwallet=mywallet1 generatetoaddress 101 <ADDRESS>
    ./bitcoin-cli -regtest -rpcwallet=mywallet1 getbalance

    Target:

        Understand how Bitcoin is created through mining.

        Learn about coinbase maturity (100 blocks).

    Why:

        Mining gives new coins to miners.

    Emphasize:

        First 100 blocks = immature coins, can’t be spent yet.

    Goal:

        Students mine enough blocks to have spendable BTC.

25–35 min: Sending Transactions

    Command:

    ./bitcoin-cli -regtest -rpcwallet=mywallet1 sendtoaddress <ADDR2> 10
    ./bitcoin-cli -regtest getrawtransaction <TXID> true
    ./bitcoin-cli -regtest -rpcwallet=mywallet2 getbalance

    Target:

        Show how to transfer Bitcoin between wallets.

        See transaction structure: inputs, outputs, scriptPubKey.

    Why:

        Sending BTC is the core of cryptocurrency usage.

    Emphasize:

        TXID = fingerprint of the transaction.

        Block hash shows confirmation.

    Goal:

        Students complete their first BTC transfer.

35–45 min: Confirming & Tracking Transactions

    Command:

    ./bitcoin-cli -regtest -rpcwallet=mywallet1 generatetoaddress 1 <ADDRESS>
    ./bitcoin-cli -regtest -rpcwallet=mywallet1 listtransactions

    Target:

        Understand confirmations and blockchain history.

    Why:

        Transactions are not final until confirmed in a block.

    Emphasize:

        “1 confirmation” means it’s in a block.

        “n confirmations” means more blocks built on top.

    Goal:

        Students track transactions through the blockchain.

45–55 min: Real-Life Case Simulations

Here are 5 scenarios you can run:
Case 1 – Paying for a Service

    Student A mines coins, sends 5 BTC to Student B as “payment for web hosting”.

    Show transaction, confirm with 1 block.

Case 2 – Escrow Simulation

    Student A sends BTC to a 2-of-3 multisig wallet (you set up keys).

    Release funds only when Student C (escrow) signs.

Case 3 – Mining Reward Split

    Student A mines 101 blocks, sends 50% to Student B, 50% to Student C.

Case 4 – Lost Wallet

    Create a wallet, send BTC to it, delete wallet files.

    Show that BTC is now unspendable (keys lost).

Case 5 – Double Spend Attempt

    Try sending the same coins to two different addresses without confirming the first.

    Show why Bitcoin rejects the second TX.

55–60 min: Wrap-Up & Q&A

    Summarize:

        Wallets, addresses, mining, transactions, confirmations.

        Real-life parallels: salaries, online shopping, escrow.

    Encourage:

        Trying bitcoin-cli help to explore commands.
