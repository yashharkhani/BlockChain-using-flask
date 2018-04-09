# BlockChain-using-flask

implementation of a blockchain for a cryptocurrency made in Python. Extract the the contents of the zip file in some directory then open a terminal there and execute
 "pip install -r requirements.txt". Make sure you have python 3. 

Then to simulate a node and mining process execute "python miner.py" from that directory.
To simulate transactions execute "python wallet.py". This should be done only when the miner is running and in a separate terminal.

On running miner.py, it will create a node (like a server). From here you can connect to the blockchain and process transactions (that other users send) by mining. As a reward for this work, you receive some coins. The more nodes exist, the more secure the blockchain gets.

This has has 2 process running in parallel:

1. The first process takes care of mining, updating new blockchains, and finding the proof of work.

2. The second process runs the flask server where peer nodes and users can connect to ask for the entire blockchain or sumbmit new transactions.

Running wallet.py allows you to generate a new address, send coins and check your transaction history (keep in mind that if you are running this in a local server, you will need a "miner" to process your transaction).
When creating a wallet address, a new file will be generated with all your security credentials.