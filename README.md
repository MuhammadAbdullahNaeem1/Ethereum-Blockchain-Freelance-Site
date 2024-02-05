# Decentralized Freelancing Platform on Ethereum Blockchain

## Overview

This platform operates on the Ethereum Blockchain, connecting freelancers and employers in a decentralized manner.

## How It Works

Employers initiate projects by providing a name and a specified price in Ether. The project's initial status is Open, and the employer sends the price as a guarantee to the smart contract. Freelancers can select Open projects, changing the status to Not Done upon acceptance. After completing the project, freelancers commit to it, shifting the status to Done. Upon the employer's verification and closure of the project, the smart contract releases the payment to the freelancer, and the project is marked as Closed.

## Installation and Deployment

### Dependencies
- [Truffle](https://github.com/trufflesuite/truffle): Install with the following command:
  ```
  sudo npm install -global truffle
  ```

### Windows Users
Before installing Truffle, ensure you have Windows Build Tools:
```
npm install -global --production windows-build-tools
npm install -global truffle
```

To install project requirements, run the following command in the project root directory:
```
npm install
``

Compile and deploy the contracts:
```
truffle compile
truffle migrate --reset
```

Once the contract is added to the chain, test it with:
```
truffle test
```

### Running the Web Interface

To launch the web interface at `http://localhost:3000/`, use the following command in the project directory. The interface connects to the smart contract deployed on the `ropsten` test network:
```
npm start
```
