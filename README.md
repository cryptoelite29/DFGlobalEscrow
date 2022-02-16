1. Review
In broad, an escrow arrangement flow is as follows: - 
1) Recipient/Sender (or a third-party) may create an escrow account(s) with an Escrow Agent;  2) Sender may initiate fund transfer to the Escrow Account; 
3) Both Sender and Recipient (2 out of 3 parties) can agree to the release of funds to the Recipient or a  revert of funds to the Sender;  
4) In the event that both the Sender and the Recipient are unable to jointly agree to the release or  revert of funds, an Escrow Agent may adjudicate the release or refund of funds based on the terms of  the escrow agreement; and  
5) Recipient/Sender’s signature can be based on a signing mandate/multi-signature approach where all  relevant signatories must authorise the particular blockchain action. 
Based on your understanding of the escrow use case, kindly review the LFGlobalEscrow.sol file (see next  page) and identify possible weakness, missing functions and areas of improvements. 


2. Task: Integration Component  

Your next task is to make the necessary changes to the LFGlobalEscrow.sol file to allow the user to have  the option of supplying either Ether or any ERC 20 token (supported by Compound) locked in the smart  contract escrow to the Compound protocol via Solidity (see https://github.com/compound developers/compound-supply-examples).  
To elaborate:- 
- If the user decides to earn yield off their Ether/ERC20, the tokens will be deposited to  Compound (and c Tokens will be stored in escrow); or  
- However, should the user choose not to earn yield, the Ether/ERC20 tokens will be locked in  escrow. 
Ether/ERC20 should be supplied to Compound at the point of deposit (e.g. only store c(ETH) in the smart  contract escrow).  
Ether/ERC20 should subsequently be retrieved only at the point of withdrawal.  *** 
