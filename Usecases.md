---
layout: default
title: Usecases
description: "Find out how you can use TruCol"
---



# Example

Suppose Alice wants some well-defined challenge, such as an n*n sudoku, to be solved. She writes a set of unit tests that check any given solution, using random inputs. Instead of creating the solution herself, Alice publishes the unit tests in a smart contract and sets a bounty for any other smart contract that solves it. Bob, the bounty hunter, finds the contract and codes a solution in a smart contract, in order to receive the bounty. If Alice's requirements are fulfilled, the smart contract automatically pays out the reward. This repository presents the protocol to do this completely trustless and decentralised, without taking any fees, thus increasing market efficiency.

<img src="/assets/images/concept.png" alt="Concept of Trucol" width="400"/>


# For Employers

You can off-load all your programming tasks that are automatically and deterministically verifiable into the TruCol protocol. This guarantees you get the lowest labour cost around the world. Furthermore, it eliminates the need of HR for these tasks. 

## Code Quality
This is one of the weaknesses of the TruCol protocol, we currently cannot guarantee high quality code solutions. To mitigate this, we recommend you enforce pre-commit like test requirements, which can consist of [well over 30 different automated code quality verifications](https://github.com/a-t-0/Networkx-To-Lava-NC/blob/main/.pre-commit-config.yaml). This ensures the code quality adheres to at least some basic standards. To go beyond this, we would like to build more code-quality compliance tools, for example an open-language tool that verifies the documentation is written with valid grammar. This does not imply that the documentation is of good quality, yet it does mean bounty hunters must put in effort to writing enough sensible documentation. Then it is still a gamble on whether it is applicable documentation or not.

This means that the TruCol protocol is particularly suited for difficult problems where the solution is more valuable than the explanation. Examples may be scheduling instances, algorithmic optimisations and even black-box machine-learning classifiers. 

## Regulatory Compliance
Our core value is user freedom, an that goes both ways, so if you need regulatory compliance, or if you need to hire from certain positions, we would love to help you integrate these requirements into the smart-contract. For example, suppose you work at ESA, and would like to see some algorithmic optimisation, yet you are bound to hire x% of workers from country y. A solution could be to only accept solutions from bounty hunters that can prove they are from country y, using a self sovereign identity, such as provided by [IRMA](https://irma.app/). We would like to go further with this, to ensure bounty hunters from all over the world automatically receive pensions and other digitally verifiable benefits. Please contact us if you are interested in collaborating on this topic.

# For Hunters
This is a winner-take-all protocol, meaning the first person to submit a valid solution retrieves the full bounty. Employers have to specify an expiration date on their bounty, and the bounty contracts are immutable after deployment. That means you know before you start to work on a task, how much you earn, and your payout is direct. To verify your solution is valid, you can run the chain locally, and verify the smart contracts pay out, by simulating the test specs in a locally hosted CI.  