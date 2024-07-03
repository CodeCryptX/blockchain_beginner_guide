# Basics of the Blockchain

### Centralized vs. Decentralized Systems

### Centralized Systems

Centralized systems are controlled from a single point, like Amazon's servers. Transactions involve paying Amazon for products and services.

- **Single Point of Failure:** 🎯 Vulnerable to disruptions affecting the entire system.
- **Service Charges:** 💸 Fees are imposed for intermediary services.

### Decentralized Systems

Decentralized systems operate without a middleman or central authority. Transactions are direct, enabling peer-to-peer interactions without fees or a central entity.

- **No Single Point of Failure:** 🛡️ Resilient against failures affecting the entire system.
- **No Service Charges:** 🚫 Direct transactions without additional costs.
- **No Central Entity:** 🌐 Users have full control over their interactions and data.

### Distributed Systems

(To be discussed later)

Decentralized systems, like those facilitated by blockchain technology, promote transparency and autonomy by removing intermediaries and central points of control, fostering a more direct and efficient way of exchanging value and information.

![Systems](https://berty.tech/blog/decentralized-distributed-centralized/decentralized_hu2a947e948837dda4cae19249962e6048_1303145_1312x0_resize_q95_mitchellnetravali.jpeg)

### What is the Blockchain?

A decentralized computation and information-sharing platform that enables multiple authoritative domains, which do not trust each other, to cooperate, coordinate, and collaborate in rational decision-making.

![Blockchain](https://www.thestreet.com/.image/ar_4:3%2Cc_fill%2Ccs_srgb%2Cq_auto:good%2Cw_1200/MTkwMDY1MDA1NDgyMjIzMjYy/blockchain-top-image.png)

### Working of the Blockchain

To make a transaction, people must be on the same network. Let's take Bitcoin as an example. If you want to send someone Bitcoin, both parties need to be on the Bitcoin network. Here are the steps, which we will discuss in detail later:

1. When someone makes a transaction, all the nodes validate whether it is valid or not. For example, if I am sending 1 Bitcoin to someone, all the nodes will check if I have 1 Bitcoin in my account. Validation requires 50% approval, but anyone can validate.
2. Once validated, the transaction is added to the ledger (we will go into this later) and stored in a block.
3. Finally, that block is added to the blockchain using consensus.

![Working of Blockchain](https://media.geeksforgeeks.org/wp-content/uploads/20220518004235/BlockchainF1.jpg)

## Components of the blockchain

### Node

A node is essentially a computer that holds a copy of the ledger and validates transactions and blocks. It plays a crucial role in building the blockchain.

### Types of Nodes:

1. **🖥️ Full Node:**
    - **Description:** Has a complete copy of the blockchain.
    - **Functions:** Can initiate, validate, and broadcast transactions to other nodes.
    - **Requirements:** Requires computers with large memory, like miners. 💾
2. **📱 Partial Node:**
    - **Also Known As:** Lightweight node.
    - **Description:** Cannot perform all functions like a full node because it does not have the complete copy of the blockchain; it only has the headers of the blocks.
    - **Dependency:** Relies on the full node for information, similar to mobile wallet apps. 📡

Nodes ensure the blockchain network remains decentralized, secure, and efficient by validating and propagating transactions and blocks.

### Ledger

A ledger is a distributed database containing all transactions and the time they occurred. It can be in various formats such as .txt or .JSON files. Here are the key features:

- **🌐 Publicly Available:** Anyone can access the ledger.
- **🔒 Immutable:** Once written, it cannot be altered or changed.
- **📑 Replicated:** Every node in the network has a copy of the ledger.

The ledger ensures transparency and security, making it a cornerstone of blockchain technology.

### Wallet

Wallets are used to store cryptocurrency or digital currency. They have both public and private keys. The public key is visible to everyone on the internet, while the private key is only accessible to the owner. 🔐

### Types of Wallets

1. **🔥 Hot Wallet:**
    - **Description:** Online and used for day-to-day transactions.
    - **Connectivity:** Connected to the internet. 🌐
    - **Security:** Vulnerable to hacking attempts. 🛡️
2. **❄️ Cold Wallet:**
    - **Description:** Offline and not connected to the internet.
    - **Purchase:** You need to buy them. 💸
    - **Security:** Much harder for hackers to compromise. 🔒

### Nonce

- 🔑 **The Key to Blockchain Rewards**

In the world of blockchain, a **nonce** is a crucial number used by miners to add their block to the blockchain and earn rewards. Here's a breakdown to make it simple and engaging:

- **What is a Nonce?**
    - A nonce is a short number that miners tweak to find a solution to a cryptographic puzzle. 🔢
- **The Puzzle of Proof of Work (POW)**
    - Every blockchain has a puzzle in the POW mechanism, which we'll delve into later. 🧩
    - Each blockchain sets a difficulty level for solving this puzzle. ⚙️
- **How Miners Use Nonces**
    - Miners aim to generate a hash using the nonce that meets the blockchain's difficulty criteria. 🎯
    - The common algorithm used for this is **SHA256**. 🔄
- **The Race to the Reward**
    - The nonce process involves a lot of trial and error. 🎲
    - The miner who first finds a valid nonce wins the reward. 🏆

Understanding the nonce is essential for grasping how miners secure the blockchain and earn their rewards. Keep this in mind as we explore more about blockchain technology!

### Hash

A hash is like a unique code generated based on the text you input into the hash function. It has several interesting properties:

1. **🔒 One-Way Function:** You can convert a message into a hash, but reversing it back to the original message is impossible.
2. **📏 Fixed-Length Output:** Regardless of the input length, the output hash will always be the same fixed length.
3. **⚡ Avalanche Effect:** A small change in the input results in a significantly different hash output.
4. **🔑 Collision Resistance:** While collisions (two different inputs producing the same hash) are theoretically possible, they are extremely rare. Modern algorithms like SHA256 ensure virtually no possibility of collisions.

Understanding these properties is essential for grasping how hashes secure information in blockchain technology.

### Block Structure

A block in a blockchain is divided into two main sections, each with specific components that ensure the security and integrity of the network.

### 1. Block Header

The block header contains crucial metadata, including:

- **🔗 Previous Block Hash:** Links the current block to the previous one, ensuring continuity.
- **🌲 Merkle Root:** The root hash of the Merkle tree, which securely and efficiently verifies transactions.
- **⏰ Timestamp:** The exact time the block was created.
- **⚙️ Difficulty Level:** The current mining difficulty target.
- **🔢 Nonce:** A value miners adjust to solve the cryptographic puzzle.

### 2. Block Body

The block body contains the actual transactions included in the block:

- **💼 Transactions:** A list of all transactions in the block, each with:
    - **🔗 Inputs:** References to previous transaction outputs being spent.
    - **📤 Outputs:** New outputs created by the transaction, specifying recipients and amounts.
    - **🆔 Transaction ID:** A unique identifier for each transaction.

## Types of the Blockchain

## Public Blockchain

A public blockchain is open for everyone to join, making it a permissionless ledger. However, joining without a purpose doesn't add value.

### Advantages:

1. **🌍 Inclusive:** Anyone can join.
2. **🤝 Community Impact:** Provides a sense of contributing to society.

### Disadvantages:

1. **⏳ Slow Transactions:** Transactions can be slow due to network congestion.
2. **📈 Scalability Issues:** Challenges in efficiently handling growth, leading to slower performance with increased users.

Improvements in scalability and transaction speed are ongoing to enhance the efficiency of public blockchains.

## Private Blockchain

In a private blockchain, access is restricted to verified users, often controlled by a centralized authority, which undermines decentralization.

### Advantages:

1. **🚀 Speed:** Transactions are faster due to fewer participants and controlled access.
2. **🔒 Lower Scalability Issues:** With fewer users, scalability challenges are reduced.

### Disadvantage:

1. **🎯 Centralized:** Controlled by a central authority, compromising the decentralized nature of blockchain technology.

While private blockchains offer speed and reduced scalability issues, they sacrifice the decentralization and openness inherent in public blockchains. **Hyperledger and Corda are the example.**

## Consortium Blockchain

Also known as a federated blockchain, it combines features of both private and public blockchains: anyone can join, but only chosen nodes can verify transactions.

### Advantages:

1. **🔐 Secure:** Transactions are secured by verified nodes.
2. **🚀 Efficient:** Faster transaction processing compared to public blockchains.
3. **📈 Scalable:** Handles growth and transactions efficiently.

### Disadvantage:

1. **🚫 Not Anonymous:** Transactions are not fully anonymous, as chosen nodes are known and verified.

An example is the Macropole blockchain, showcasing how consortium blockchains balance access, security, and efficiency while maintaining some level of transparency among participants.

## Merkle Tree

1. **🔗 Transaction Hashes:**
    - Each transaction in a block has a unique transaction hash.
2. **🌳 Pairing and Hashing:**
    - Transaction hashes are paired and hashed together sequentially until a single hash remains. This creates a binary tree structure.
3. **🌱 Merkle Root:**
    - The final resulting hash, known as the Merkle root, is stored in the block header.
    - It summarizes all transactions in the block.

### Benefits:

- **🚀 Efficiency:** Efficient verification of transaction integrity.
- **🔐 Security:** Changes to any transaction are easily detectable.
- **💡 Compactness:** Provides a concise proof of all included transactions.

### Example:

For transactions \( T1, T2, T3, T4 \):

- Calculate hashes \( H(T1), H(T2), H(T3), H(T4) \).
- Pair and hash them until you get the Merkle root \( Root \).

The Merkle root ensures the security and integrity of blockchain transactions by condensing them into a single, verifiable hash.

![Merkle tree](https://www.investopedia.com/thmb/1IGah2OLWcvEboCYQdaQR9_qBXo=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/MerkleTree-5590a1ca4e904b6e8e60b6257751e840.png)

## Consensus

Method to allow the node runner to add the block to the blockchain it has different types.

## **Proof of Work** (PoW)

PoW is a consensus method where node runners compete to add blocks and receive rewards, as used in Bitcoin.

### How It Works:

1. **🧩 Puzzle Assignment:**
    - A cryptographic puzzle is assigned to all nodes, known as the nonce puzzle.
2. **⛏️ Solving the Puzzle:**
    - Nodes attempt to find a nonce (a number) that solves the puzzle by hashing it with the block data.
    - The first node to solve the puzzle broadcasts its solution to others.
3. **✅ Verification:**
    - Other nodes verify the solution by checking the nonce against the puzzle criteria.
    - Once verified, the block containing valid transactions is added to the blockchain.

### Implications:

- **⏰ Time and Energy Consumption:**
    - PoW requires significant computational power and energy to solve puzzles, which can be seen as wasteful.
    - This competitive process ensures security and decentralization by making it computationally expensive to alter the blockchain history.

### Summary:

Proof of Work ensures that adding blocks to the blockchain is based on computational effort, securing the network against malicious activities like double-spending. While energy-intensive, it remains a robust method in decentralized blockchain systems like Bitcoin.

### Proof of Stake (PoS)

Proof of Stake (PoS) operates based on the amount of cryptocurrency staked by node runners. Validators who stake more ETH have a higher chance to validate blocks and earn rewards. The likelihood of becoming a validator also considers the age of the ETH staked.

### How It Works:

1. **Staking and Validation:**
    - Validators participate by staking a certain amount of ETH as collateral.
    - The more ETH staked, the greater the chance of being chosen to validate the next block of transactions.
2. **Block Validation:**
    - Validators selected to validate blocks propose new blocks and verify transactions.
    - They earn rewards in ETH for their participation and contribution to the network.
3. **Age of Staked ETH:**
    - The duration for which ETH has been staked (stake age) can influence the likelihood of being selected as a validator.

### Benefits:

- **🔒 Security:** Incentivizes validators to act honestly to protect their staked ETH.
- **💸 Efficiency:** Energy-efficient compared to Proof of Work (PoW).
- **🌐 Participation:** Allows broader participation in network validation based on staked ETH rather than computational power.

### Considerations:

- **🕒 Stake Age:** Validators may need to stake ETH for a certain period to maximize their chances.
- **📈 Rewards:** Earned rewards include transaction fees and newly minted ETH.

Proof of Stake aims to ensure blockchain security and efficiency by aligning incentives with the amount and age of ETH staked, promoting a sustainable and decentralized consensus mechanism.
