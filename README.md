# EchoChain Tutorial

In this project, we will cover the following topics:

1. Creating a simple wallet.
2. Sending signed transactions using our blockchain.
3. Feeling extra cool.

## 1. Preparing a Wallet

In cryptocurrencies, coin ownership is transferred on the Blockchain as transactions. Participants have an address to which funds can be sent to and from. Wallets can store these addresses and make new transactions on the Blockchain.

## 2. Transactions & Signatures

Each transaction carries the following data:

- The public key (address) of the sender of funds.
- The public key (address) of the receiver of funds.
- The value/amount of funds to be transferred.
- Inputs, which are references to previous transactions that prove the sender has funds to send.
- Outputs, which show the amount relevant addresses received in the transaction.
- A cryptographic signature that proves the owner of the address is the one sending this transaction and that the data hasn’t been changed.

### What is the purpose of signatures and how do they work?

Signatures allow only the owner to spend their coins and prevent others from tampering with their submitted transaction before a new block is mined. The private key is used to sign the data, and the public key can be used to verify its integrity.

## 3. Testing the Wallets and Signatures

We are almost halfway done. Let’s test if everything is working. In the EchoChain class, let’s add some new variables and replace the content of our main method.

## 4. Inputs & Outputs 1: How cryptocurrency is owned

To own cryptocurrency, you must receive it. The ledger references previous transactions, showing that cryptocurrency was sent to your address.

## 5. Inputs & Outputs 2: Processing the transaction

Blocks in the chain may receive many transactions, and the blockchain might be very long. To get around this, we keep an extra collection of all unspent transactions that can be used as inputs.

## 6. Adding transactions to our blocks

We need to implement the transaction system into our blockchain. We should replace the useless data in our blocks with an ArrayList of transactions.

## 7. The Grand Finale (In the beginning, there was EchoCoin)

We should test sending coins to and from wallets and update our blockchain validity check. But first, we need a way to introduce new coins into the mix. We will release all the coins we wish to have in the first block (the genesis block).

### Updates to EchoChain class:

- A Genesis block that releases 100 EchoCoins to WalletA.
- An updated chain validity check that takes into account transactions.
- Some test transactions to ensure everything is working.

You have successfully created your own cryptocurrency (sort of!). Your blockchain now:

- Allows users to create wallets with `new Wallet();`
- Provides wallets with public and private keys using Elliptic-Curve cryptography.
- Secures the transfer of funds using a digital signature algorithm to prove ownership.
- Finally, allows users to make transactions on your blockchain with `Block.addTransaction(walletA.sendFunds(walletB.publicKey, 20));`

### Dependencies:
[bouncy castle bcprov-jdk15on-159.jar](http://www.java2s.com/example/jar/g/download-gson282jar-file.html#google_vignette) <br>
[gson gson-2.8.2.jar](http://www.java2s.com/example/jar/b/download-bcprovjdk15on159jar-file.html)
  ### Output:
  <img width="617" alt="echocoin" src="https://github.com/gaurav-aditya/create-your-own-blockchain--II/assets/110540811/1154023b-c031-4298-b822-06e5a903cc93">


You can download these project files on [Github](https://github.com/gaurav-aditya/create-your-own-blockchain--II).

Meet me 😉 [echoaditya](https://gaurav-aditya.github.io)

Contact me: 
- Email: echoaditya@proton.me
- [Linktree](https://linktr.ee/echoaditya)
