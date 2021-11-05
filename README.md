## About

I've put together using the following technologies:

* [Ethereum Javascript API (Web3.js) 1.0-beta](https://github.com/ethereum/web3.js/tree/1.0)
* [Truffle](https://github.com/trufflesuite/truffle)
* [Parity](https://github.com/paritytech/parity)
* [React Redux Universal Hot Example](https://github.com/bertho-zero/react-redux-universal-hot-example) (implements [React](https://github.com/facebook/react), [React Router](https://github.com/reactjs/react-router), [Babel](http://babeljs.io), [Webpack](https://webpack.js.org/), [Redux](https://github.com/reactjs/redux), [Redux Dev Tools](https://github.com/reactjs/redux-devtools), [React Router Redux](https://github.com/reactjs/react-router-redux), [ESLint](http://eslint.org), and more)

This starter repository for building react/redux dapps uses the latest bleeding-edge Ethereum development technologies. Please note that the repository is still under development; I will be adding additional smart-contracts/UI examples.

## Installation

Download the latest verion of Parity [here](https://github.com/paritytech/parity/releases).

Also ensure that you have the latest verion of Truffle installed globally:

```bash
npm install -g truffle
```

Finally install all package dependencies:

```bash
npm install
```

## Running Dev Environment

Run all of the following commands inside the project directory.

### 1) Start Parity Development Chain

```bash
parity --chain dev --ws-origins "*"
```

Note: we set `--ws-origins` so that we can use websockets to subscribe to blockchain events.

### 2) Compile and Migrate smart-contracts

```bash
truffle compile && truffle migrate
```

NOTE: after running open parity (at [`http://127.0.0.1:8180/`](http://127.0.0.1:8180/)) in a browser and confirm all of the transactions to complete the migration.

### 3) Start Dev Javascript Server

```bash
npm run dev
```
