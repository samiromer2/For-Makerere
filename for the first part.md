https://andersbrownworth.com/blockchain/

in github
https://github.com/anders94/blockchain-demo/
https://github.com/anders94/public-private-key-demo

Map
link:https://txstreet.com/

address:
https://www.bitaddress.org/bitaddress.org-v3.3.0-SHA256-dec17c07685e1870960903d8f58090475b25af946fe95a734f88408cef4aa194.html

🔗 What the site offers

    []Hashing: Explore how SHA‑256 turns inputs into a fixed-length string. It shows sensitivity to even tiny changes.

    []Blocks & Mining: View block structure (data, nonce, previous hash) and “mine” blocks to meet a hash difficulty target.

    []Building a Chain: See how blocks link via previous-hash pointers, and how immutability arises .

    []Distribution/Diffusion: Simulate multiple peers and how chains stay in sync across the network.

    []Tokens & Coinbase: Simulate transactions and token creation (like mining rewards).

    []Public/Private Key & Signing Demo: Learn how digital signatures secure and verify transactions.

✅ Final take

    Great for learning hash functions, block mining, immutable chains, P2P consensus, transactions, and crypto‑signatures.

    Highly interactive, beginner‑friendly, and visually clear.

My Game plan:
✅ SESSION STRUCTURE (1 hour)
🕒 0–5 mins: Intro

    Who you are, and why blockchain matters today (finance, supply chain, decentralization).

    Your goal: to give a technical feel of how blockchain really works, not just theory.

🕒 5–15 mins: Hash Function & SHA256

    Tool: Hash page

    Show how a hash converts any input into a fixed 64-char string.

    Change one letter → watch hash change completely (avalanche effect).

    Emphasize:

        It's one-way (can't reverse it).

        It's deterministic (same input = same output).

        No two inputs should produce the same output (collision resistance).

🕒 15–25 mins: Public & Private Keys

Tool: Public-Private Keys

    Show how a public-private key pair is generated.

    Private key = secret

    Public key = shared

    Use the tool to sign a message with the private key, and verify it using the public key.

🎯 Emphasize:

    You don’t encrypt with private key, you sign.

    You verify identity and data integrity (no tampering).

    This is the backbone of wallets and transactions.

✅ Optional Demo: Show Metamask or Bitcoin wallet and link keys to addresses. <-this could be added after johns part .

🕒 25–40 mins: Blockchain Basics & Mining

Tool: Blockchain tab

    Start from a block:

        Data, nonce, previous hash

    Show how changing data invalidates the hash

    Show how mining adjusts the nonce until the hash starts with zeros (difficulty)

    Then link several blocks together → blockchain!

🎯 Key Points:

    Tampering one block changes all future hashes (immuability)

    Proof-of-Work makes tampering hard

🕒 40–50 mins: Distributed Blockchain

Tool: Distributed tab

    Show 3 peers A, B, C

    Mine a block on A

    See how other peers "adopt" the longest valid chain

🎯 Emphasize:

    All nodes verify and copy the longest valid chain

    This is the heart of decentralization and trust

✅ Optional: Briefly show how forks happen

🕒 50–60 mins: Wrap Up / Q&A / Advanced Ideas

    How real chains work: Bitcoin, Ethereum

    Mention:

        Smart contracts

        Gas fees

        Layer 2s / scalability

    Ask:

        “Any questions about how blocks are mined or verified?”

        “Want to try the demo yourself?”

💡 keeping this in mind:

    Ask questions during the demos (“What do you think happens if I change the data?”)

    Keep the flow fast, don’t get stuck in math

    Use analogies if needed (e.g., fingerprint = hash, sealed envelope = signed message)

    Consider letting one person try the demo in front of others
