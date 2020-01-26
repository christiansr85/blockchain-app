# blockchain-app
Example of blockchain application with Solidity

## Steps to configure environment
- Download and install/execute local blockchain netwrok from https://www.trufflesuite.com/ganache
- Install `truffle` npm dependency: `npm i -g truffle@5.0.2`
- Install `metamask` extension in your browser: https://metamask.io/

## Truffle commands to use
- `truffle migrate` -> execute migrations files
- `truffle console` -> opens truffle console
    - Commands to check the contract
        - `todoList = await TodoList.deployed()`
        - `taskCount = await todoList.taskCount()`
        - `taskCount.toNumber()`