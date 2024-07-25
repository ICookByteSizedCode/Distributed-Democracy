# Distributed Democracy

## Introduction

Distributed Democracy aims to revolutionise the process of voting by introducing the concept of blockchains and self-sovereign identity.
In this project, we have created a voting system that allows officers of the election commission to register new candidates and new voters. The registered candidates can upload their name, age, picture and stance. The registered voters can also do the same as well as cast a single vote to a registered candidate of their choice. Their vote will be recorded on the blockchain. This ensures immutability and by extension transparency for the election to be freely audited by an independent third party. Transparency is our main goal here since it gives citizens the confidence that they participated in a free and fair election.
By incorporating SSI (Self Sovereign Identity), we have also ensured that the voters’ privacy and security is given the utmost care. Using SSI, a voter’s PII (Personally identifiable information) is kept safe from data breaches by only giving information in a form that cannot be used to distinguish them from other voters, thus ensuring their privacy. Since the votes are recorded on the blockchain, this ensures the security and integrity of the election by preventing any attempts at committing fraud.

An extensive report about this project can be found (here)[https://drive.google.com/file/d/1RaybDD0mtVOovGBOBpIt42fr3lul00WA/view?usp=sharing].

## Motivation

Elections in India are often faced with violence due to the ever growing dissatisfaction and distrust in the EVM (Electronic Voting Machines) systems. People don’t trust the audits being conducted. We wanted to create a system that allowed anyone to independently verify the integrity of the voting whilst safeguarding everyone’s PII.

## Architecture

<img src="unnamed (1).png" width="200" height="200">

## Installation Instructions

1. Download this repository from the main branch as that is the default branch in the repository.
2. Setup your own Infura IPFS dedicated gateway.
3. Ensure you have the relevant node packages installed.
4. Open a terminal in the root directory.
5. Run

```
npx hardhate node
```
This should provide you with 20 mock Ethereum accounts with mock currency to execute operations in the website.
6. Run

```
npx hardhat run scripts/deploy.js --network localhost
```
This should deploy the solidity contracts onto the localhost network.

7. In another terminal, run
```
npm run dev
```
This should start the server and the website should now be live.

8. Ensure you have the Metamask extension for Chrome installed. This will allow you to load your currency.
9. You can now register candidates/users and cast votes.
10. Candidate information, voter information and votes are now stored on the blockchain and can be audited to assess election fairness and integrity.

## Future Works

1. Introduce SSI to protect and enhance voter privacy and election transparency.
2. There is always room for improvement. We are currently working on introducing ranked choice voting, a system which improves fairness in elections by allowing voters to rank candidates in order of preference.
3. This system can be produced as a mobile app ensuring widespread adoption.
