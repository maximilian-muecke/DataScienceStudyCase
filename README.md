# DataScienceStudyCase
Data Science Study Case June 2022 / Think-Tank

Here you can find the Case Study for the Data Scientist position of Think-Tank BMW Group. 
This Case Study is the opportunity for us to assess some skills you will need as a Data Scientist in our Team and to show us your capacity to come up with innovative ideas when you face new challenges.
You have 4 days to submit your results. Afterwards, you will have the opportunity to present and discuss your results to different members of our team for 10-15 min.

**IMPORTANT : If you have any ideas but you didn't implement them, please list them at the end of your solution.**


## Task 1 : Model building

Context :  You work in a Crypto startup and you want to identify malicious Ethereum addresses. Fortunately, you have found 3 interesting datasets :

- malicious_adresses : Dataset of malicious addresses with the comments explaining the reason of suspecting the adresses. 
- malicious_transactions : Transaction data related to malicious adresses.

            * acc_name : Malicious address involved in the transaction.
            * blockNumber : The block number that the transaction was included in.
            * timeStamp : The time (in UTC) at which the block was mined.
            * hash : A unique identifier that can be used to locate a specific transaction.
            * nonce : The count of transactions sent out from the account. The number is initialized at 0 and is incremented by 1 for each transaction sent.
            * blockHash : A unique identifier of the block. 
            * transactionIndex : Index transaction.
            * from : The acc_name from which the transaction was sent.
            * to : The acc_name to which the transaction is addressed.
            * value : The amount of Ether sent via the transaction.
            * gas : The upper limit of how much computational work and storage the sender is willing to spend on the transaction.
            * gasPrice : The amount of Ether per unit of gas the user is willing to pay for the transaction, commonly denoted in a subunit of Ether known as Gwei. 1 Gwei = 1x10^-9 Ether.
            * isError : boolean which indicates if an error occured during the transaction
            * txreceipt_status : status of the transaction, "1" means the transaction succeded, "0" means the transaction failed. 
            * input : Information that is passed to a smart contract when a transaction is sent to its address. However, if the transaction is creating a contract, the contract’s bytecode is placed in the input data field.
            * contractAdress : The contract address related to the input.
            * cumulativeGas : Sum of the gasUsed by this transaction and all preceding transactions in the same block.
            * gasUsed : The amount of computational work and storage used in the transaction.
            * confirmations : Block number that confirmed the transaction. 
            
- normal_transactions : Transaction data related to normal adresses.

Leading points :

1) Explore the datasets, if necessary clean them and create or keep the revelant features.
2) Analyze the accounts' behavior. What helpful statements can you make?  
3) Group the malicious accounts (acc_name) in several categories based on their behavior. Justify your grouping decision. 
4) Given the different groups you have created, what would you advise the business to do?  
5) Train a prediction model that predicts maliciousness based on financial behavior. How good does your model perform? How would you tweak it?
4) Given the prediction you have created, what would you advise the business to do?  
 
Feel free to use your own methodology to solve this problem. 


## Task 2 : Innovative ideas

Context : In Supply Chain process, a company should rely on their suppliers. However, some of your suppliers have made some mistakes in the delivery (missing or wrong items shipped) and the production has been stopped. As a Data Scientist, working in a famous Food Company, your manager asks you to detect bad suppliers. Give some ideas to solve the problem. 

Leading points : 

1) Explain the process/methodology/models and justify it.
2) What kind of data do you need to solve this problem? 
3) What are the limits of your ideas?


Hint : 
- The level of escalation can be measured according to some features : Missing and wrong items at the delivery, Delays...
- Bad suppliers are not the majority of the suppliers. 


# Enjoy the task and blow our minds !

