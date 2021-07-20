# CryptoCurrency101

This is a learning project to learn more about cryptocurrency by building one. I have implemented various components of a cryptocurrency like blockchain, wallets, miners, and proof of work. I have also made few Flask routes to test these functionalities and simulate how cryptocurrency would work in real life.

## Installing Dependencies 

After cloning the project to the workstation enter the following command in cmd/terminal to install all the dependencies.

```bash
pip install -r requirements.txt
``` 

## How to run the code

First, move into the src folder

```bash
cd src
``` 
1. To start a blockchain node, execute the command below:
```python blockchain.py -p 5000```
2. You can add a new node to blockchain by executing the same command and specifying a port that is not already used. For example, ```python blockchain.py -p 5001```
3. To start the blockchain client,
```python blockchain_client.py -p 8080```
4. Now you will need an application like postman to send requests to routes you want to access.
5. You can create a new wallet by sending a get request at route ```localhost:8080/wallet/new``` 
6. Now you can send a post request to make the transaction at route ```localhost:8080/generate/transaction``` 
7. Now as a node you can mine a block by sending get request at route ```localhost:5000/mine```
8. To add new nodes to the network you can send post request at route ```localhost:5000/nodes/register```
