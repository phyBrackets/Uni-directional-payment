# Uni-directional-payment
A Uni-directional payment channel implementation written in solidity. 
Payment channels allow participants to repeatedly transfer Ether off chain.

#Here is how this contract is used:

-A deploys the contract, funding it with some Ether.
-A authorizes a payment by signing a message (off chain) and sends the signature to B.
-B claims the payment by presenting the signed message to the smart contract.
If B does not claim his payment, A get the Ether back after the contract expires. 

This is called a uni-directional payment channel since the payment can go only in a single direction from A to B .

Importing contract reference : https://openzeppelin.com/contracts/ 
