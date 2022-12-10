# Overview

*certDAO* is a decentralized autonomous organization (DAO) that verifies domain to contract address mappings for the Ethereum community. Think of *certDAO* as a certificate authority for Web3.

## How does *certDAO* work?

![certDAO workflow diagram](/images/certDAO-arch.jpeg)

### Simple Workflow:
1. Contract owner navigates to *certdao.net*, connects their wallet, enters their domain and contract address, and submits the information to the *certDAO* backend which validates that.
   - The smart contract lives on the domain entered.
   - The user connected wallet is the owner of the contract.

2. Returns the above information to the contract owner and asks if the owner wants to proceed with the registration process.

3. If the contract owner proceeds, the contract owner pays a small fee (currently **0.05 ETH**) to the DAO. This fee is used to help support the DAO and prevent spam.

4. Once the transaction is mined (initial registration status set to `pending`), a governance discussion on discourse is created with the information provided by the contract owner.

5. For the next 7 days, the community can vote on the registration request. If the registration passes both of the above heuristics (contract owner submitted, contract lives on domain), contract will be auto-approved if no issues raised in governance.

If the registration request is approved, the registration status is set to `approved`. If the registration request is rejected, the registration status is set to `rejected`.

### Other Workflows:
The beauty of `certDAO` is that if the community raises an issue with a site (contract), the DAO can immediately flag the contract/URL and all wallets and interfaces can read from the contract and flag and warn the user!

All of this in a transparent and decentralized fashion!

## What is *certDAO*?

- A way for users to verify that a smart contract is the intended contract for a given domain by the contract owner and not a malicious actor.

- A way for the community to flag malicious smart contracts on domains (hosts) and that information be read by all interested parties (wallets/interfaces) in a decentralized manner.

- A way to help prevent phishing attacks on the Web3 community.

- A way to help prevent frontend exploits on the Web3 community.

- A way to create a common standard/interface to be used by wallets and interfaces to verify that a contract is the intended contract for a given domain when navigated to by the user.

## What *certDAO* is **not**

- A smart contract auditing service.

- A way to enforce an outside regulatory framework on smart contracts*.

*flagging a contract as malicious does **not** mean that the contract is illegal or violates any regulatory framework. It simply means that the contract does something outside of what the site promises/user intends to happen.

## The goal of *certDAO*

Eventually, if *certDAO* is successful, we will be able to create a standard interface for wallets and interfaces to use to verify that a contract is the intended contract for a given domain when navigated to by the user.

All wallets/interfaces will integrate *certDAO* and all contract owners will have to register their contract with *certDAO*. *certDAO* creates a first line of defense against malicious actors trying to exploit the user.

## Who is behind *certDAO*?

*certDAO* is a community project. Anyone can contribute to the project. The project is currently being developed by a single developer: [certy](www.github.com/0xcerty). We need your help!

There is currently **no** outside funding for the project. All development is done in the developer's free time.
