# blockchain-app
Example of blockchain application with Solidity

## Steps to configure environment
- Download and install/execute local blockchain network from https://www.trufflesuite.com/ganache
- Install `truffle` npm dependency: `npm i -g truffle@5.0.2`
- Install `metamask` extension in your browser: https://metamask.io/

## Truffle commands to use
- `truffle compile` -> compiles contracts
- `truffle migrate [--reset]` -> execute migrations files
- `truffle console` -> opens truffle console
    - Commands to check the contract
        - `todoList = await TodoList.deployed()`
        - `taskCount = await todoList.taskCount()`
        - `taskCount.toNumber()`
    - When we have created at least one task
        - `task = todoList.tasks(1)`
        - `task`

## Web application
- Here we are going to interact with `metamask` browser's plugin.
    - Make sure you are connected to the development network created by `truffle ganache` application.
    - Import an account using the first private key from the ganache development server keys.

## Testing
We are using `Mocha` along with `Chai.js`.

Just type `truffle test` from the terminal command line to run the tests.
