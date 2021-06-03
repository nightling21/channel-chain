# channel-chain
Inspired by the Telegram group [Rings of Fire](https://t.me/joinchat/Uao0Z_hBequXkeB0) and the [LNTrustChain](https://www.takethetorch.online/).

### Purpose
The aim of this project is for your Lightning Node to get a free channel with inbound liquidity, for every channel you open to another node.

### How it works
If you want to join the chain, you have to open a channel to the node on top of the chain. After that, you are on top of the chain. So the next node that wants to join the chain, will have to open a channel to your node.

### Procedure
1) Wait until your predecessor has it's channel confirmed.
2) Request to put your node on top of the list by submitting a PR. If you don't manage to create a PR, seek help from the [Telegram group](https://t.me/channel-chain).
3) Once the PR is merged, open a channel with (at least) the defined amount to the node below you.
4) After the channel is confirmed, create a PR with a Link to the created channel (on [1ml.com](https://1ml.com))
5) Leave the channel open.

### Rules
1) The chain can always only grow by one single successor node. If someone is waiting for their spot in the chain (existing PR), you have to wait until their channel is confirmed to request your spot.
2) As soon as your accepted on the list, you must open the channel.
3) PRs are only accepted if they contain all the information needed.
4) Only channels with at least the defined amount are valid channels.
5) Don't open channels until you are confirmed on the list.
6) If your channel doesn't open within 6 hours, you may be kicked out of the chain, so someone else can take your spot.
7) You can join a channel-chain multiple times.
8) Don't open channels to nodes you are already connected with. Those channels will be ignored and someone else will take your spot.
9) If you don't play fair (e.g. closing your channel quickly after you got your inbound capacity), you will be blocked from further participation.

### Comparison to Rings of Fire
Think of a Ring of Fire that never closes. A Ring of Fire that grows forever. Infinitely.  
**Advantage**: Less overhead. Much faster setup. Very little communication needed from your part.  
**Disadvantage**: No rebalancing.

### PR template:
```
Property | Value
---|---
Chain Index | <INSERT INDEX HERE>
Node Alias | <INSERT YOUR ALIAS HERE>
Node Key | <INSERT YOUR PUB KEY HERE>
Node Address | <INSERT YOUR ADDRESS HERE>
Channel | <LEAVE THIS EMPTY FOR THE REQUES, ADD CHANNEL LINK HERE AFTER OPENING OF CHANNEL>

```
(newline at the end is necessary)
