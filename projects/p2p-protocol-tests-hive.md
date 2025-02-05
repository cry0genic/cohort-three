# Project Template

Hive is a system for running integration tests against Ethereum clients. This project goal is to extend further the current p2p tests.

## Motivation

The more tests we have on Ethereum the more confidence we can have that the protocol is working as intented. There are Ethereum clients written by different teams with different programming languages and they all must be done accordingly to the specs. Having a robust test framework helps Ethereum Core Developers to identify potential implementation bugs in early development stage thus making the network more secure and reduce production errors.

## Project description

Currenty there are p2p tests for 'eth', 'discv4' and 'discv5' as we can see [here](https://github.com/ethereum/go-ethereum/tree/master/cmd/devp2p/internal). This project aims to increse the scope of those tests and to add new tests for the Ethereum execution clients.

## Specification

The p2p networking specification can be found [here](https://github.com/ethereum/devp2p).

To implement the solution, first I'll go over the current p2p tests that were done for 'eth', 'discv4' and 'discv5' (<https://github.com/ethereum/go-ethereum/tree/master/cmd/devp2p/internal>) to understand the code pattern then later I'll further extend the scope of those tests.

## Roadmap

- 1st month: I'll be going deeper on the [devp2p specs](https://github.com/ethereum/devp2p) to better understand the bits and bytes of the devp2p protocol.
- 2nd month: Run the current tests and understand how the current tests are done.
- 3rd and 4th month: Start implementing the new p2p tests.

## Possible challenges

In order to be able to write tests for the p2p protocols, a deep understand of how the networking protocol works is necessary. This means understand on the low level the RPLx handshake, the messages format that are exchanged between nodes, the ECIES Encryption etc. The main challenge would be to understand the bits and bytes of how the current p2p networking stack for ethereum execution clients works.

## Goal of the project

The goal for this project is to expand further the p2p tests that we currently have on hive.

## Collaborators

### Fellows

- [strykerin](https://github.com/strykerin)

### Mentors

- Felix Lange
- Mario Vega

## Resources

- p2p tests are implemented [here](https://github.com/ethereum/go-ethereum/tree/master/cmd/devp2p/internal)
- [hive](https://github.com/ethereum/hive): Ethereum end-to-end test harness
- [devp2p specification](https://github.com/ethereum/devp2p)
