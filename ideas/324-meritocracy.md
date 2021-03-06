---
id: #324-meritocracy    
title: Meritocracy
status: implementation
lead-contributor: richard/jarrad
contributors: jarrad, ceri, jb, rajanie
  
budget:
- actual: xxx
- estimate: yyy
- currency: ETH/USD/SNT
---

# Swarm proposal

## Summary and Goal(s)
Kudos DApp - an experiment with awarding kudos each week between Status contributors. Heavily inspired by Giveth’s awesome RewardDAO concept, the idea is that contributors get a weekly allowance of SNT which they can distribute amongst other contributors as they see fit. The awarded totals can be withdrawn by contributors who have earned kudos.

More here: https://discuss.status.im/t/kudos-rewards-building-the-status-meritocracy/1019

**Swarm goals**
* Create DApp
* Launch DApp
* Encourage regular (weekly) CC interaction with DApp to recognise others

## Communication
Channel: [#324-meritocracy](https://get.status.im/chat/public/324-meritocracy)

Sync frequency: async via text

## Research
* Influenced by Giveth's Reward DAC [concept](https://wiki.giveth.io/dac/contributors-guide//).
* Initial proposal and discussion [here](https://docs.google.com/document/d/1QN2SZ8QO-7jfH8rAKLVDAB5LxuKvBScodWoiRfejFkM/edit#heading=h.tommnlxre23w).
* Idea developed on Discuss [here](https://discuss.status.im/t/kudos-rewards-building-the-status-meritocracy/1019).
* Collected sign-ups [here](@people-ops) - 42 people signed up 🎉


## Specification

* DApp spec [here](https://github.com/status-im/meritocracy) courtesy of @jarrad

## Implementation

**Timeline**
[Mid-Feb - 5 April]
- [x] Deploy DApp to Mainnet (@richard)
- [ ] Add @jb and @rajanie as additional `Admins` if possible (@richard) - only the contract owner (richard) can add admins
- [x] Seek help with adding Design to the UI (@richard/@people-ops) 
- [x] Test DApp and share feedback (@people-ops)
- [x] Create budget and plan for transfer of SNT into contract (@people-ops / finance)
- [x] Create People Ops site page / FAQ (@people-ops) - https://people-ops.status.im/meritocracy/
- [x] Draft launch post for Discuss (@people-ops)
- [x] Launch on 5 April with post on Discuss (@people-ops) - delayed to 8 April
- [x] Present/demo in TH (@richard / @people-ops)
- [ ] Schedule weekly reminders to ping all contributors to let them know a new reward cycle has started (@people-ops)
- [ ] Leaderboard UI

**Updates**
* 22 March - Added @ceri as admin in Ropsten testnet
* 25 March - @richard and @ceri walkthrough to get admin role set up, before doing allocations in mainnet.
* 26 March - pinged Finance about funding the wallet with SNT & ETH. Did another test run on Ropsten of the weekly allocation by admin of funds to the meritocracy contract.
    * DApp does not currently have leaderboard UI, but the contract can be queries for each individual's balance, so this info can be pulled manually if needed.
* 28 March - Finance have transferred a small amount of ETH and SNT into @ceri's Metamask wallet ready for first cycle (equivalent to SNT 5 per participant).
* 1 April - 5 SNT distributed to all participants.
* 3 April - troubleshooting issues with Richard. Drafting launch comms
* 8 April - launched with 10 SNT allocated.


## Maintenance

* @ceri, @rajanie, and @jb will act as DApp `admin` to make the weekly allocation of SNTs.
* Ask CCs to log any issues either in #324-meritocracy or creating an issue [here](https://github.com/status-im/meritocracy/issues).
* Review quarterly (first review early July 2019) to review success of DApp:
    * Engagement - > 50% of core contributors (currently = 32 people) using the DApp regularly (at least once a month)
    * Functionality - all open issues closed and volume of problems reported reduced
    * Feedback - anecdotal feedback from users positive, do CCs enjoy and benefit from using the DApp?
    * Utility - does the data generated through the DApp accurately represent a Meritocracy, or are there any concerns/issues.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
