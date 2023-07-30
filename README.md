# Module18_FinTech

## Introduction
This repository contains the implementation of a blockchain ledger called PyChain. The ledger includes functionality to create blocks, perform the proof of work consensus protocol, and validate blocks in the chain. The PyChain Challenge involves adding new features to the existing PyChain implementation, including the creation of a Record Data Class, modification of the Block Data Class to store record data, adding user inputs to the Streamlit interface, and testing the PyChain ledger by storing records.

## Languages and Concepts
The implementation for the PyChain Challenge is based on the following languages and concepts:

Languages:
Python
Concepts:
Blockchain
Data classes in Python
Proof of work consensus protocol
Streamlit (for building the user interface)
Test-driven development (TDD) principles
Code organization and modularity
Comments and documentation
Git version control


### Step 1: Create a Record Data Class
In this step, we define a new Python data class called Record. This class formalizes the data structure for the sender, receiver, and amount attributes. The steps to create the Record Data Class are as follows:

Define a new class named Record.
Add the @dataclass decorator immediately before the Record class definition.
Add an attribute named sender of type str.
Add an attribute named receiver of type str.
Add an attribute named amount of type float.

### Step 2: Modify the Existing Block Data Class to Store Record Data
In this step, we modify the existing Block data class to store the record data. The data attribute in the Block class is renamed to record, and its data type is set to the Record class that we created in Step 1.

### Step 3: Add Relevant User Inputs to the Streamlit Interface
In this step, we enhance the Streamlit interface to allow users to input values for sender, receiver, and amount for each transaction. The following actions are taken to complete this step:

Delete the input_data variable from the Streamlit interface.
Add an input area to capture the sender value from the user.
Add an input area to capture the receiver value from the user.
Add an input area to capture the amount value from the user.
Update the Add Block button functionality to include the Record with sender, receiver, and amount in the Block along with attributes for creator_id and prev_hash.

### Step 4: Test the PyChain Ledger by Storing Records
In this step, we test the complete PyChain ledger and the user interface by running the Streamlit application and storing some mined blocks in the ledger. After storing multiple blocks, we verify the blockchain validation process using the Streamlit interface. The following actions are performed to complete this step:

Navigate to the project folder where the PyChain Challenge is coded.
Run the Streamlit application using the command streamlit run pychain.py.
Enter values for sender, receiver, and amount and click the Add Block button multiple times to store several blocks in the ledger.
Verify the block contents and hashes in the Streamlit drop-down menu and take a screenshot of the Streamlit application page displaying the blockchain with multiple blocks.

Test the blockchain validation process and take a screenshot of the Streamlit application page displaying "Blockchain is Valid." (See file Module18_1)


#### Conclusion
The PyChain Challenge involves enhancing the existing PyChain implementation by adding a Record Data Class, modifying the Block Data Class, and enhancing the user interface using Streamlit. By completing all the steps and meeting the requirements, we ensure that the PyChain ledger can successfully store records, validate blocks, and maintain a secure blockchain.
