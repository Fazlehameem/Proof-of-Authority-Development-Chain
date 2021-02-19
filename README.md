# Proof-of-Authority-Development-Chain

My first project at ZBank will be to set up a private testnet to explore Blockchain technology and its potential at ZBank.



For this project, I will set up a testnet using following skills/tools: 



1.) Puppeth, to generate my genesis block 
2.) Geth, a command-line tool, to create keys, initialize nodes, and connect the nodes together. 
3.) The Clique Proof of Authority algorithm  


Step 1: Puppeth

a.) Open Gitbash for Windows user and change directory to the folder you've downloaded the Goethereum. 
b.) Type in the following code ./puppeth
c.) Follow the steps in the picture below 

Step 2: Geth

a.) Create accounts for two (or more) nodes for the network with a separate datadir for each using geth.
b.) Use the following code for creating two nodes 
  b.1) ./geth account new --datadir node1
  b.2) ./geth account new --datadir node2
c.) Initialize the nodes 
  c.1) ./geth init yournetworkname.json --datadir node1
  c.2) ./geth init yournetworkname.json --datadir node2
  
Step 3: Mining 
  
  a.) Run the first node, unlock the account, enable mining, and the RPC flag. Only one node needs RPC enabled.
  b.) Set a different peer port for the second node and use the first node's enode address as the bootnode flag.
  c.) Be sure to unlock the account and enable mining on the second node
  
  You should now see both nodes producing new blocks, congratulations!

MyCrypto: 

Open MyCrypto app
[Change_Network](Screenshots/change-network.png)

Change network to your custom network

[Setup_Customnode](Screenshots/Custom_Node.png)
Follow the steps. You can find the chain id at your network.json folder 

After completing the above step, go to Keystore File and add your key from node1 folder 

[Key_node1](Screenshots/Key.png)

The results should be an account with enormous account balance
[Account_balance](Screenshots/Crypto_balance.png)

Send transaction to Node2 by typing in the public address of Node 2 in "To Address" 

Click on TX Status to confirm the transaction 

[TX_Status](Screenshots/MyCrypto.png)

Congratulations! The assignment is completed successfully.
