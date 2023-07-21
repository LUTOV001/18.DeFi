# **UCB FinTech Bootcamp Module 18 Challenge**
# *Decentralized Finance : Blockchain using Python*
## **Introduction**
### The Bootcamp Module 18 Challenge - Decentralized Finance : Blockchain using Python requires creation of a blockchain-based ledger system, accessible to the user via a web interface to facilitate data entry. The blockchain ledger should record transactions sent (by a 'Sender') to a destination ('Receiver") for an 'amount' while validating the data to keep the ledger's integrity
---
## **Goals and Objectives**
### *Part I. Create a Record Data Class*  : A new data class named Record is defined with attributes sender, receiver, and amount. This class serves as a blueprint for the financial transaction records to be stored in the blocks of the PyChain ledger.
### *Part II.  Modify the Existing Block Data Class to Store Record Data* : The existing Block data class is modified by replacing the generic data attribute with a record attribute of type Record. Now, each block contains a record of a financial transaction, including the sender, receiver, and amount.
### *Part III. Add Relevant User Inputs to the Streamlit Interface*  : In the Streamlit application, additional input areas are created to capture user inputs for sender, receiver, and amount. When the "Add Block" button is clicked, a new block is created with the provided data and added to the PyChain.
### *Part IV. Test the PyChain Ledger by Storing Records* : The user can test the complete PyChain ledger by running the Streamlit application. They can enter values for the sender, receiver, and amount, and click the "Add Block" button to store multiple blocks in the ledger. The blockchain validation process can also be tested using the web interface.
### The Block class includes a hash_block() method that calculates the SHA-256 hash of the block's data, creator ID, timestamp, previous block's hash, and nonce (a value used in the proof-of-work algorithm). The PyChain class manages the chain of blocks and includes methods for proof-of-work mining, adding blocks to the chain, and validating the blockchain's integrity.
### Overall, this code demonstrates the basic implementation of a blockchain with financial transaction records using Streamlit for user interaction
---
## **Technologies and Tools**
### The following list includes the main technologies and tools using during the preparation and deployment of the solution:
### 1. *Python* - Programming language used to code the solution. Version 3.7.13 was used. Required libraries and frames listed in the Installation section below
### 2. *GitHub* - Reposotory for code deployment, version management and documentation of the presented solution
### 3. *Jupyter Labs* - IDE tool for coding, code testing/debugging and solution documentation. Version V3.4.4 was used
### 4. *Git Bash console* - Local console used to test the coded solution and sync wiht GitHub Version 2.40.0.windows.1 was utilized
### 5. *Slack* - Collaboration tool to communicate and brainstorm with other FinTech Bootcamp participants
### 6. *Operative System* - This solution was prepared in a PC running Windows 11 v H22
### 7. *[dataclasses](https://docs.python.org/3/library/dataclasses.html)* - The dataclasses module provides a decorator and functions for creating classes with minimal boilerplate code. It is used for creating data classes, which are classes primarily used to store data rather than providing complex behavior. No installation needed.
### 8. *[typing](https://docs.python.org/3/library/typing.html)* - The typing module provides support for type hints in Python, allowing developers to specify the types of variables, function arguments, and return values. Type hints improve code readability and can be used by type checkers and code editors to provide better hints and warnings. No additional installation needed.
### 9. *[datetime](https://docs.python.org/3/library/datetime.html)* - The datetime module provides classes for working with dates and times in Python. It is used in the code to manage timestamps in the blocks of the PyChain ledger. No additional installation needed.
### 10. *[pandas](https://pandas.pydata.org/docs/)* - Pandas is a popular Python library for data manipulation and analysis. It provides data structures like DataFrames for handling and analyzing structured data effectively. In the code, Pandas is used to display the PyChain ledger as a DataFrame. Indysllation details below.
### 11. *[hashlib](https://docs.python.org/3/library/hashlib.html)* - The hashlib library in Python provides interfaces to various secure hash and message digest algorithms. In this code, it is used to compute the SHA-256 hash of the blocks' data as part of the blockchain's hashing process. No additional installation needed.
---
## **Installation Guide**

### 2. [pandas](https://pandas.pydata.org/docs/) : Pandas is a popular Python library for data manipulation and analysis. It provides data structures like DataFrames for handling and analyzing structured data
#### 1.1. Open the GitBash terminal
#### 1.2 Type the following command and press Enter:
```python 
pip install pandas
```
### 2. [Streamlit](https://docs.streamlit.io/) : Streamlit is a Python library used for building web applications for data science and machine learning projects. It allows developers to create interactive web interfaces with minimal code, making it easy to turn data scripts into shareable web apps.
#### 2.1. Open the GitBash terminal
#### 2.2 Type the following command and press Enter:
```python 
pip install streamlit
```
---
## **Solution Structure**

### The **[18.DeFi](https://github.com/LUTOV001/18.DeFi)** repository in GitHub contains the solution components. The repository consists of the following folders and contents as described below:
 
###   *1. Results :* Contains the files showing the Streamlit application, the block contents and hashes in the application and the multiple blocks in the blockchain, plus the validity verification results for the blockhain.
###   *2. gitignore :* Instructions for which files/file types to exclude from the sync process between GitHub and the local environment.
###   *3. README.md :* The present file containing this outline of the challenge and its components and results.
###   *4. pychain.py:* This is the Python program with the code for the challenge solution.
---
## **User Instructions**
### 1. Launch the GitBash terminal and navigate to the folder containing the repository. Once there, execute the program using the following command line:
```python 
streamlit run pychain.py
```
### 2. In the launched streamlit web page, input the data for the **"Sender"** and press Ctr+Enter, intput data for the **"Receiver"** and presse Ctr+Enter, and finally input data for the **"Amount** and press Ctr+Enter.
### 3. Press the **Add Block** button to have the application validate the data, create the block and it to the blockchain (See the balloons!)
### 4. Press the **Validate Chain** button to have the application validate the data in the blockchain and observe the **"True"** result appearing at the bottom.
### 5. Repeat steps 2-4 to add multiple blocks to the blockchain and validate its integrity
####
---
## **Results**
#### Below is the screen shot showing the application and results from executing the steps described above:  
### ***1. Streamlit Application***
#### Shows the initial screen of the launched Streamlit web application with no data other than the Genesis block (e.g. the first block in the blockchain)
##### ![streamlitapp.png](https://github.com/LUTOV001/14.AlgoTrading/blob/main/Results/svc_returns_plot.png)
#####
### ***2. Blockchain contents and validation***
#### Shows the blocks in the blockchain and the validation result
##### ![PyChain screenshot.png](https://github.com/LUTOV001/14.AlgoTrading/blob/main/Results/svc_returns_plot.png)
#####
##### ***Note*** For more info on the "Sender", "Receiver" and "Amounts" data used, refer to this [video](https://youtu.be/Pg4bStWrk4M)
---
### **Credits**
#### Prepared by Luis Torres 
#### [LUTOV001](https://github.com/LUTOV001)
#### July 2023