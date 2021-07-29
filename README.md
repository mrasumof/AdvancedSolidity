# Advanced Solidity Homework

The objective of this homework is to develop and deploy 3 smart contracts. Each of them have a different purpose and I will explain each in detail below.

### 1.	Associate Profit Splitter (Source Code: “AssociateProfitSplitter.sol”)

The objective of this smart contract is to split the value deposited in the contract among the three wallets selected during contract deployment time.

How it works:
- At deployment time, we need to provide 3 wallet addresses. In our case I am picking the following 3 addresses from Ganache:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 1](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture1.gif?raw=true)


- The initial balance for these 3 wallets is 104 ETH. We will use the ending balance to demonstrate that a deposit had been made into the contract and moved to the accounts as the smart contract is programmed for.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 2](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture2.gif?raw=true)


- Proof of Contract Deployment:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 3](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture3.gif?raw=true)


Contract deployed at: 0xAa7B045Dc459889Eb46b6B8c9d8987847904EdFb

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 4](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture4.gif?raw=true)


Now we will proceed to the distribution. The first step is to insert a value of ether that we want to distribute. In this case I am using 24 ETH.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 5](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture5.gif?raw=true)


Then in the deployed contract, click “deposit”:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 6](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture6.gif?raw=true)

Authorize the payment of the transaction in the wallet:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 8](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture8.gif?raw=true)


Once the transaction is confirmed, means that the execution of the contract was completed.

If we look the balance of those 3 accounts used for deploying the smart contract, we would see that they increased by 8 ETH each as it was programmed in the smart contract to distribute evenly.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 9](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture9.gif?raw=true)


### 2.	Tiered Profit Splitter (Source Code: “TiredProfitSplitter.sol”)

The objective of this smart contract is to split the value deposited in the contract among the three wallets selected during contract deployment time, using a 60-25-15 ratio to split the ETH deposited in the contract. In case there is a reminder, it should go to the holder of the highest value wallet, which in this case is the 60% receipient.

How it works:

Like In the previous case, at deployment time, we need to provide 3 wallet addresses. In our case I am picking the following 3 addresses from Ganache (for simplicity of calculations, I am using the same 3 addresses as in the previous case):

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 10](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture10.gif?raw=true)


The initial balance for these 3 wallets is 112 ETH. We will use the ending balance to demonstrate that a deposit had been made into the contract and moved to the accounts as the smart contract is programmed for.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 11](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture11.gif?raw=true)


Proof of Contract Deployment:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 12](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture12.gif?raw=true)


Contract deployed at: 0xC82074Fc81413675aeF73430753503Ef43916198

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 13](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture13.gif?raw=true)



Now we will proceed to the distribution. The first step is to insert a value of ether that we want to distribute. In this case I am using 100 ETH.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 14](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture14.gif?raw=true)


Then in the deployed contract, click “deposit”:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 15](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture15.gif?raw=true)


Authorize the payment of the transaction in the wallet:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 16](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture16.gif?raw=true)


Once the transaction is confirmed, means that the execution of the contract was completed.

If we look the balance of those 3 accounts used for deploying the smart contract, we would see that they increased by:

60 ETH the first wallet
25 ETH the second wallet
15 ETH the third wallet

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 17](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture17.gif?raw=true)

Wallet ending in f86e: initial balance of 112 ETH + 60 ETH = 172 ETH
Wallet ending in 1Ca8: initial balance of 112 ETH + 25 ETH = 137 ETH
Wallet ending in 75AC: initial balance of 112 ETH + 15 ETH = 127 ETH


### 3.	Deferred Equity Plan (Source Code: “DeferredEquityPlan.sol”)

The objective of this smart contract is to distribute 1000 shares every year to the beneficiary of the smart contract

How it works:

In this case, at deployment time we need to provide only 1 wallet address, the one of the person that will be beneficiary of this smart contract. We will use address 0xAE5d9aDDdcF93D5947EEC2De6F42684049d411DC, although this smart contract do not produce any change in the balance of the wallet, only transfers a number of shares to the account.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 18](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture18.gif?raw=true)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 19](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture19.gif?raw=true)


Proof of Contract Deployment

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 20](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture20.gif?raw=true)


Contract deployed at: 0xAcCa360C20c72A4Ad66c3F1663f894a3EB8AaE83

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 21](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture21.gif?raw=true)


Now we will proceed to the distribution. We need to make sure that the “value” field in remix is set to 0 and then click on distribute.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 22](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture22.gif?raw=true)


Distribution Executed:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 23](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture23.gif?raw=true)


As this is a yearly distribution, the contract has a feature that does not allow for it to be executed more than once a year. So, when we execute it again, we obtain an error:!

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 24](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture24.gif?raw=true)


We included a feature that allows us to bypass this limitation so we can test the functionality. In order to do so, we created the “fastforward” functionality which simulates moving in time 400 days in advance so we can re-run the distribution.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 25](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture25.gif?raw=true)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 26](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture26.gif?raw=true)


Then we can distribute again:


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 27](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture27.gif?raw=true)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![pic 28](https://github.com/mrasumof/AdvancedSolidity/blob/main/Images/Picture28.gif?raw=true)
