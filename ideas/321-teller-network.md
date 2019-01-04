---
id: #321-teller-network
title: Teller Network
status: research
lead-contributor: Iuri @iurimatias
contributors:
    - Anthony @alaibe
    - Barry @bgits
    - Iuri @iurimatias
    - Jonathan @jrainville
    - Ricardo @3esmit
    - Richard @richard-ramos
budget:
- actual: xxx
- estimate: yyy
- currency: ETH/USD/SNT
---


Teller Network
=

## Summary and Goals

DApp inside of Status, which provides borderless, peer-to-peer fiat-to-crypto ‘Teller Network’ that allows Stakeholders to find nearby users to exchange their cash for digital assets and currency, giving any smartphone owner in the world the ability to take control of their personal wealth.

## Contributors

- Anthony @alaibe
- Barry @bgits
- Iuri @iurimatias
- Jonathan @jrainville
- Ricardo @3esmit
- Richard @richard-ramos

(+ Janitor swarm)

## Communication

- `status channel`: #321-teller-network
- `sync schedule`: brainstorming on Mondays / stand ups on Wednesday
- `pivotal link`: https://www.pivotaltracker.com/n/projects/2231548
- `research notes`: https://github.com/status-im/status-teller-network/wiki
- `github repo`: https://github.com/status-im/status-teller-network

## Research
1. Sellers: 
- Will the seller receive the full SNT used to obtain the license once it is released or will a fee be deducted.
- Determine if a Harbinger tax mechanism could be used somehow for the acquisition of licenses or map location.
- Where will the seller information be stored at?

2. Escrow:
- How will arbitrage work for a descentralized escrow. What protections does a buyer and seller have when performing a transaction in case one of them is an evil actor.
- Most teller network buyers will not have ETH to perform transactions. Gas Abstraction might be useful for covering this scenario
- Escrow not necessarily has to be onchain. It might be handled offchain and use signatures.
- Can any ERC20 token be sold/bought? or only those that handled by the status wallet.
- If users are locking up funds in escrow, from a user perspective it may not be that different from locking up in a plasma contract which can allow more frequent transacting with lower costs. An interesting expansion on that is with offchain transactions you might be able to setup atomic swaps cross chain, so BTC/SNT direct trade possibly using lightning for the BTC side.

3. Interactions with other SNT use cases, and Status Features

    3.1 Indicators of Trust
    - License contract should be associated to this trust system. 
    - Obtaining a license should allow you to sell crypto to fiat up to an amount determined in function of the SNT deposited against the username.
    - Slashing of the SNT stake would decrease the amount of SNT staked, and max amounts of crypto that can be selled / escrows open at the same time?


    3.2 Tribute to Talk
    - Probably we should allow communication between a buyer and the seller so they could perform agreements on how will the payment be done. Research needs to be done to determine how will TtT affect this communication, since if a seller sets a fee, most likely he wont be able to talk with potential buyers (It's highly likely that buyers do not have SNT to pay for the tribute). This could be potentially mitigated by introducing Identities in Status, where a seller could create an identity exclusive for selling and this one wouldn't have TtT fees associated.

## Specification
TODO

## Implementation

#### Sprint 1
**Front end**
- License acquisition flow
- Component to obtain prices using cryptocompare.
- Maps component to see sellers. (not yet connected to smart contract / datasources)

**Smart contracts**
The following smart contracts were created for the initial sprint of Teller Network
- *License*: allows an address to act as a seller inside the tellet network. Acquiring a license requires N amount of SNT which is set by the controller of the contract (which should be a multisig, and later, a DAO component like Topic Democracy. A license can be released after a period of time and the SNT used to obtain the license will be returned to the user.
- *Escrow*: Allows a seller to send an amount of ether or a number of ERC20 tokens and have them held by the contract and later released to the buyer. Current implementation is naive and does not have arbitrage. A buyer can rate a transaction after it's released.

## Maintenance
TODO

## Copyright

Copyright and related rights waived via CC0.
