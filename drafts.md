### ⚙️ Node & Wallet Setup

1. **`createwallet "mywallet"`**  
    → Creates a wallet for managing funds.  
    🟡 _Shows how wallets are isolated data stores within the node._
    
2. **`getwalletinfo`**  
    → Displays wallet-specific information (balance, tx count, etc).  
    🟡 _Great to show that wallets are separate from nodes and track UTXOs._
    
3. **`getnewaddress`**  
    → Generates a new receiving Bitcoin address.  
    🟡 _Demonstrates address creation using HD (hierarchical deterministic) wallets._
    
4. **`getbalance`**  
    → Shows wallet's total confirmed balance.  
    🟡 _Simple but powerful way to illustrate UTXO ownership._
    

---

### ⛏ Mining & Block Control

5. **`generatetoaddress 101 <address>`**  
    → Instantly mines 101 blocks to any address (required to unlock coinbase funds).  
    🟢 _Teaches mining and how coinbase rewards mature after 100 blocks._
    
6. **`getblockcount`**  
    → Displays the current block height.  
    🟢 _Helps students track blockchain growth._
    
7. **`getblockhash <height>`**  
    → Gets block hash from a height (e.g., height = 0 for genesis block).  
    🟢 _Introduces block references._
    
8. **`getblock <blockhash>`**  
    → Shows full block details (txs, time, size).  
    🟢 _Allows exploration of how blocks are structured._
    

---

### 💸 Transactions

9. **`sendtoaddress <address> <amount>`**  
    → Sends BTC to another address from wallet.  
    🔵 _Very intuitive way to show value transfer._
    
10. **`listtransactions`**  
    → Lists wallet transaction history.  
    🔵 _Provides a historical view of wallet activity._
    
11. **`gettransaction <txid>`**  
    → Returns full details of a single transaction.  
    🔵 _Dives deeper into UTXOs, confirmations, and fees._
    
12. **`decoderawtransaction <hex>`**  
    → Decodes a raw tx to human-readable JSON.  
    🔵 _Shows how transactions are encoded and broadcast._
    

---

### 🔍 UTXO & Mempool Insight

13. **`listunspent`**  
    → Lists all unspent outputs (UTXOs) in wallet.  
    🟠 _Perfect for teaching the UTXO model of Bitcoin._
    
14. **`getmempoolinfo`**  
    → Shows mempool stats (txs waiting to be mined).  
    🟠 _Useful for understanding transaction propagation._
    

---

### 🧪 Advanced Capabilities (Bonus)

15. **`createrawtransaction`, `signrawtransactionwithwallet`, `sendrawtransaction`**  
    → Used together to build, sign, and send custom transactions.  
    🧠 _Optional advanced topic for showing full control over tx construction._