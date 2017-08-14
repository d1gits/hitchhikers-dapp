# hitchhikers-dapp

Hitchhikers guide to Dapp development, source for 

https://medium.com/@kaspermeilgaard/hitchhikers-guide-to-dapp-prototyping-1eb3264e556a

## Warning

Don't ever deploy anything written in this repo on a production blockchain. The contracts in here have been written to contain exploits. And the exploit has been added as an example. Your Ether will get stolen.

## Installation

1. Install truffle and an ethereum client. For local development, try EthereumJS TestRPC.
    ```javascript
    npm install -g truffle // Version 3.0.5+ required.
    npm install -g ethereumjs-testrpc
    ```

2. Clone repo
    ```javascript
    git clone git@github.com:d1gits/hitchhikers-dapp.git
    ```

3. Enter folder
    ```javascript
    cd hitchhikers-dapp
    ```

3. Compile and migrate the contracts.
    ```javascript
    truffle compile
    truffle migrate
    ```

4. Run the webpack server for front-end hot reloading. For now, smart contract changes must be manually recompiled and migrated.
    ```javascript
    npm install
    npm start
    ```

5. Truffle's own suite is included for smart contracts. Be sure you've compile your contracts before running jest, or you'll receive some file not found errors.
    ```javascript
    // Runs Truffle's test suite for smart contract tests.
    truffle test
    ```

6. To build the application for production, use the build command. A production build will be in the build_webpack folder.
    ```javascript
    npm run build
    ```
