---
layout: default
title: Getting Started
description: A short introduction to working with the TruCol protocol
last_modified_at: 2021-07-01
---

## Truffle Testing
Documentation is [here](https://www.trufflesuite.com/docs/truffle/getting-started/installation), video instructions is [here](https://www.youtube.com/watch?v=2fSPn0-8ORs) (starts at 1:34). The following installations are written for a Linux system:
 
1. install npm on device
```
sudo apt install npm
```
2. Install truffle
```
sudo npm install -g truffle
```
5. Run truffle test to verify if your bounty contract works.
```
truffle test
```

## Manual Testing

Besides the automated testing using Truffle, you can also manually test your smart contracts. To do so you can look at [AskContract](https://github.com/v-bosch/TruCol/blob/main/contracts/AskContract.sol) which consists of a square root problem and the [SolveContract](https://github.com/v-bosch/TruCol/blob/main/contracts/SolveContract.sol) which is able to solve the problem.

Test:
- Open both contracts in https://remix.ethereum.org
- Compile (ctrl+s) and select the AskContract (Not the template!),  deploy it (optionally add a value to it)
- Copy the contract address of the AskContract
- Compile and select the SolveContract (Not the template!), paste the copied address in the deploy field and deploy it
- Finally, click on the SolveContract and click on the 'solve' function
- Now the funds should be transferred to the owner of the SolveContract

TestRefund:
- Change the expiry value in the contract to a future experidate (unix timestamp)
- Compile and select the AskContract, deploy it with a value
- Click on the AskContract and try to get the refund, when it is past your timestamp it should self-destruct otherwise it should not work

Note that only the owner of the contract (which is the person who either created or solved the contract) can activate the refund function.
