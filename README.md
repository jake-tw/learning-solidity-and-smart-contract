## Solidity and Smart Contract

#### Account

![account](./images/001.png)

- Externally Owned Account ( EOA )
    - Address: 160-bit length, locate to this account
    - Account State
        - nonce: tx's sequence
        - balance

- Contract Account
    - Address: 160-bit length, locate to this contract, contract address will base on EOA and nonce
    - Account State
        - nonce
        - balance
        - code hash: bytecode's location
        - storage hash: global variable

#### Transaction

- Transfer Ether
    - From: sender
    - To: recipient
    - Value: Ether amount
    - Data: note

- Create contract
    - From: sender
    - To: empty
    - Value: empty or send Ether to your contract
    - Data: bytecode

- Call contract function
    - ***smart contract will never execute by itself***
    - function runing on Ethereum Virtual Machine ( EVM )
    - every opcode and storage has the same price ( gas )
    - doesn't have random opcode ( 0.1 + 0.9 = 0.999... )

#### EVM

![account](./images/002.png)
