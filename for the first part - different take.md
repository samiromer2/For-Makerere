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
🧪 1-Hour Technical Lab Plan
0–5 min — Introduction & Lab Setup

Goal: Set the stage for why these tools matter in security and privacy.

    Explain:

        Security tools protect confidentiality, integrity, and authenticity.

        These tools are used in secure communication, digital signatures, data verification, identity authentication.

    Mention real-life applications outside Bitcoin:

        Secure email (PGP/GPG)

        Software updates (signed packages)

        Secure document verification (PDF signatures)

    Open Anders Brownworth’s site or local demo.

5–15 min — Hash Functions & SHA256

Tool: Hash Demo

Technical Points:

    What is a hash?

        A fixed-length output from any input (fingerprint of data)

    Properties:

        Deterministic

        One-way (irreversible)

        Collision-resistant (two different inputs shouldn’t give same hash)

        Avalanche effect (tiny change → big change in output)

    Lab Activity:

        Input “hello” → record SHA256 output

        Change to “Hello” → compare new output

        Try longer text, files, or numbers

        Highlight avalanche effect visually

15–30 min — Public & Private Keys

Tool: Public/Private Key Demo

Technical Points:

    Asymmetric cryptography = key pair: public key + private key

    Private key → kept secret, used to sign data

    Public key → shared, used to verify signatures

    Applications outside Bitcoin:

        Secure email (S/MIME, PGP)

        SSH authentication

        Signing software updates

    Lab Activity:

        Generate a key pair

        Write a message (“Lab Session Test”)

        Sign message with private key

        Verify signature with public key

        Change one letter in message → verify again (should fail)

30–45 min — Blockchain Technology (Non-Bitcoin View)

Tool: Blockchain Demo

Technical Points:

    Blockchain = linked list of blocks secured by hashes

    Each block contains:

        Data

        Nonce (proof-of-work)

        Previous block’s hash

    Security Features:

        Tamper-evident (change data → all future hashes break)

        Distributed verification possible

    Non-Bitcoin uses:

        Secure audit logs

        Digital identity

        Supply chain tracking

    Lab Activity:

        Show one block → edit its data → watch hash turn red (invalid)

        Re-mine the block to fix hash

        Add multiple blocks, show how one edit breaks the chain

45–55 min — Distributed Blockchain Concept

Tool: Distributed Demo

Technical Points:

    Multiple copies of the same ledger exist

    Nodes synchronize by accepting the most valid chain

    Lab Activity:

        Show 3 peers (A, B, C)

        Mine a block in peer A → watch it sync to B and C

        Edit data in peer B → chain becomes invalid until re-mined

55–60 min — Wrap-Up & Q&A

    Recap:

        Hashes → integrity

        Keys → authentication

        Blockchain → tamper-evidence

    Discuss real-life, non-Bitcoin applications:

        Digital certificates (HTTPS)

        Secure health records

        Electronic voting systems

    Answer questions

    Suggest extra reading/tools:

        GPG/PGP for encryption

        CyberChef for hashing

        Keybase for key management
