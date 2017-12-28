# DIN

A Decentralized Identification Number (DIN) is a unique product identifier that is adminstered by the global **`DINRegistry`** Ethereum smart contract.

**[DINRegistry.sol](./contracts/DINRegistry.sol)**

```
Address (Ethereum Main Net): 0xd8096aBb6ff38b912Ff7dCebdDcF6bd2bed468BB
ABI:
[{"constant":false,"inputs":[{"name":"_resolver","type":"address"}],"name":"selfRegisterDINWithResolver","outputs":[{"name":"_DIN","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"_DIN","type":"uint256"}],"name":"resolver","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"index","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_owner","type":"address"},{"name":"_resolver","type":"address"}],"name":"registerDINWithResolver","outputs":[{"name":"_DIN","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_DIN","type":"uint256"},{"name":"_owner","type":"address"}],"name":"setOwner","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_owner","type":"address"}],"name":"registerDIN","outputs":[{"name":"_DIN","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"_DIN","type":"uint256"}],"name":"owner","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"selfRegisterDIN","outputs":[{"name":"_DIN","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"genesis","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"_DIN","type":"uint256"}],"name":"updated","outputs":[{"name":"_timestamp","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_DIN","type":"uint256"},{"name":"_resolver","type":"address"}],"name":"setResolver","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"inputs":[{"name":"_genesis","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"anonymous":false,"inputs":[{"indexed":true,"name":"DIN","type":"uint256"},{"indexed":true,"name":"owner","type":"address"}],"name":"NewOwner","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"DIN","type":"uint256"},{"indexed":true,"name":"resolver","type":"address"}],"name":"NewResolver","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"DIN","type":"uint256"},{"indexed":true,"name":"owner","type":"address"}],"name":"NewRegistration","type":"event"}]
```

## Registration

The **`DINRegistry`** contains four methods to register a new DIN:

**`selfRegisterDIN`**

Self-register a new DIN.

**`selfRegisterDINWithResolver`**

Self-register a new DIN and set the resolver.

**`registerDIN`**

Register a new DIN for a specific address.

**`registerDINWithResolver`**

Register a new DIN for a specific address and set the resolver.
