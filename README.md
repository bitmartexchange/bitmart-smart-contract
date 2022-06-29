### bitmart-smart-contract
smart contracts for token and crowd sale.

BMX.sol : BMX Contract 

SafeMath.sol: SafeMath Contract lib, used by Timelock.sol

Timelock.sol: Time lock for BMX Contract Owner

### Contract Relationship
1. Set the owner of BMX contract to the contract address of timelock.

2. The owner of a timelock contract can be set to a common address or a contract multi sign address.

3. The owner of timelock initiates the transaction, and calls the owner method of the BMX contract through the queuetransaction() and executetransaction() methods.