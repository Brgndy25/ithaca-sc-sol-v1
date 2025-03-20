# Ithaca Protocol Anchor Program v1


## Purpose
The Ithaca smart contract serves as the on-chain post-match settlement layer for the Ithaca Protocol. 
It enforces trade settlement rules and manages collateral custody after orders are matched off-chain via an auction-based matching engine. 
The contract ensures that risk is shared optimally and trades are settled in a secure, transparent, and efficient manner.

## Modules
### Access Controller
Manages permissions and user authentication, ensuring only authorized parties can perform sensitive operations.

### Token Validator
Used by protocl admins to whitelist SPL tokens for trading

### Fundlock
Secures collateral by locking funds during trade settlement until all conditions are met as well as managing user funds.

### Ledger
This module is responsible for receiving settlements and updating balances on-chain after off-chain trade matching. 
