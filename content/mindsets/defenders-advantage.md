---
title: Defenders' Advantage
image: /img/wall.png
iama: mindset
---

In 2016, Vitalik Buterin, founder of Ethereum, shared [new modes for collaboration](https://medium.com/@VitalikButerin/a-proof-of-stake-design-philosophy-506585978d51), advice for what we now know as DAOs. 


It built heavily on the concept of Defenders' Advantage, well-known in Game Theory and Cryptography, 

While investigating ways to make Proof Of Stake coordination work on a technical level, he realised that Defenders' Advantage also needed to be applied to the human side, to decentralised coordination and communication of the people taking care of the network.

## Applying the cryptographic principles to DAO communication 

> Cryptography is truly special in the 21st century because cryptography is one of the very few fields where adversarial conflict continues to heavily favor the defender. 

> Castles are far easier to destroy than build, islands are defendable but can still be attacked, but an average person’s ECC keys are secure enough to resist even state-level actors. 

Vitalik looked at the power we all have in our computers, to encrypt messages than nobody, not even governments, can decode. The reason is [down to the math](https://www.youtube.com/watch?v=M7kEpw1tn50), basically because it's hard for computers to calculate the [factors](https://www.mathsisfun.com/algebra/factoring.html) of [large prime numbers](https://math.stackexchange.com/questions/7377/why-are-very-large-prime-numbers-important-in-cryptography). 

So the cryptography used by your blockchain wallet is makes it very light for your computer to encrypt something, but almost impossible for an attacker to decrypt, even if they had a building full of computers.  This is an asymmetrical advantage to the defender of the message.

> Cypherpunk philosophy is fundamentally about leveraging this precious asymmetry to create a world that better preserves the autonomy of the individual.

> Cryptoeconomics is to some extent an extension of that, except this time **protecting the safety and liveness of complex systems of coordination and collaboration**, rather than simply the integrity and confidentiality of private messages.

The big idea here is that Defenders' Advantage can be designed into coordination systems, protecting a group's direction and momentum, their workspaces and culture.

There's a lot going on here, so we'll start with understanding how Defenders' Advantage works in various computer systems, then expand that to defending human coordination and collaboration.


## The Internet itself is built on Defenders' Advantage
The Internet itself formed from ARPANET, a military communication network that used [decentralision](/mindsets/decentralisation) to create resilience against attack. If one router goes down, the messages just finds another path. So an attacker can't just unplug something, they have to invest in unplugging a whole bunch of things to have any effect at all. The Defenders have a big advantage. 

### Denial Of Service
When websites like Facebook go down, that's because they chose centralised infrastructure instead of decentralised.  

With Internet servers, a common attack is called Denial Of Service. If you overload a server, it can't respond anymore.  Just hit it with enough useless noise, and it has no capacity to communicate with its real users. 

It's like a flashmob at a store. The staff are too overwhelmed by the flood of people to deal with the normal customers.

### Sender vs Receiver advantage
Sometimes, DAOs end up with centralisation in various places, and the noisier they get, the harder it is for people to communicate.

In this case, we have a choice.  Do we favour the sender or the receiver?  Do we make it easy for people to send messages at the cost of overwhelming receivers, or do we increase the cost or barriers to send, in order to protect the receivers?  

When an environment is too noisy, it's time to start favouring the receivers.

## Proof-Of-Stake is built on Defenders' Advantage
Modern Proof-Of-Stake blockchains design for Defenders Advantage as well.  They must ensure the cost for bribing the miners is never worth it. 

The [Chainlink v2 Whitepaper](https://research.chain.link/whitepaper-v2.pdf) explains how they've looked at this from an economic point of view.  Chainlink's blockchain provides us with data, and often that data is used to make decisions for much larger sums of money than the Chainlink network earns. For example, if a smart contract relies on Chainlink for the price of gold, it might only pay Chainlink a few dollars to direct a transaction worth millions in gold.  So in some cases, it makes sense for an attacker to bribe those nodes to give false information, for example to lie and say the price is lower to allow the attacker to buy gold under market price. This would be a kind of economic attack on the Chainlink network.

This gives us a nice illustration of Defenders' Advantage.

Each Chainlink data provider needs to stake their own money to provide data services and earn fees.  But if one provider thinks another is corrupt, they can call it out, and take the stake of the other provider if the accusation is true. So now the briber needs to bribe *every* data provider.

On top of this, Chainlink's *super-linear staking mechanism* forces the briber to overpay each time they have another provider to bribe. So overall they have to massively overpay, making it not worth doing. 

> The main such feature is super-linear staking impact (specifically, quadratic). An adversary must have resources considerably in excess of nodes’ deposited funds in order to subvert the mechanism.

As Chainlink gets bigger, the cost to bribe the network rises quadratically.  The cost of attack grows while the cost of defense decreases in relation. The bigger the network, the easier it is to kick out corrupt nodes since the network depends on them less.

## Defending against internal threats
When we think about internal threats, it's not all about bribes or antagonistic intentions.

Vitalik explains it's a mistake to assume this is always about rational incentives:

> Economics is not everything. Individual actors may be motivated by extra-protocol motives, they may get hacked, they may get kidnapped, or they may simply get drunk and decide to wreck the blockchain one day and to hell with the cost.

Vitalik's advice is to protect communication from bad actions, both external **and internal.**

Usually these don't look like attackers.  In most DAOs we see a variety of complex motivations that lead to behaviours that work against the DAO as a whole.

New joiners look for their place, somewhere they can be useful, get paid, maybe make new friends. So far no worries. But what about those that are looking to build their professional portfolios, to gain reputation, or for insider information? These motives aren't necessarily bad but start to show misalignment. Good intentions, but maybe not good actions.

Whales have their own agendas too. Some whales participate in private groups that coordinate price manipulation. This isn't always through direct collusion either.  It happens more often and more more naturally by signalling to each other through their behaviours.  Whales tend to buy in and sell of in groups, and signal intention to each other through their participation (or lack of participation) in governance. So here, even more transparency doesn't help, since they can still collude implicitly and in the open.

We can't limit ourselves to thinking of adversaries as trying to fud and short the token for pure financial gain. We have to consider people trying to help as well.

Bad actions often come from people motivated to collaborate, but based on their various other agendas, they may slow down or act against the more common needs of the group.  

A regular example is weekly coordination meetings and open chat channels for project teams. Every week, those same meetings and chat conversations are slowed down by new joiners. The effect starts to resemble a flashmob or denial of service attack; the channel gets too noisy for the important messages to get seen.  

There are other cases, like people who join in to learn, people who want to build their professional portfolio, who're just looking to hang out and make friends. None of these are negative agendas, but they create noise in a communication channel.

So even though everyone is there to help, it's the same effect as a Denial-Of-Service attack.

## Not all transparency is equal

The reality with blockchains and DAOs is that to be open, we have to accept that bad actions will come from people with internal access, and people who are trying to help.

We've seen that [centralisation is a natural tendency](/mindsets/decentralisation), and it naturally leads to collusion, with or without transparent communication channels. 

More transparency is usually the kneejerk response, but that actually favours the centralised cartels, since they can see what's going on while still coordinating in private or through signalling.

So pure transparency, especially when combined with Sender's Advantage, favours the attackers.  

As DAO contributors, we have to organise our own communication to work against this.

## Autonomy in communication
For decentralisation to work, participants need to be able to act autonomously, free from centralised control.

But how do we allow such autonomy while at the same time dissuading that same autonomy to be used for collusion?

> It is important to have both layers of defense: economic incentives to discourage centralized cartels from acting anti-socially, and anti-centralization incentives to discourage cartels from forming in the first place.

In Game Theory, there are the famous [Generals' Problems](https://www.youtube.com/watch?v=s8Wbt0b8bwY) which are all about defending communication through a hostile environment.  One of the classics involves two allied armies meeting on two hills, where the valley between in is patrolled by their common enemy.  How can they send messages and coordinate?  All the solutions rely on **designing for a Defenders' Advantage for the messengers and coordinators.**

Put another way, creating more transparency only helps when it favours the autonomous nodes and not the centralised cartels.


## Finding the balance
The right balance between openness and defense is usually a matter of:
 - knowing where you are on the [Actiocratic Axis](/mindsets/permissionless), do you need to favour the doers who create, or the vetoers who protect?
 - distinguishing between rights to see, and rights to participate

If the coordinators are protecting a common good, design for Vetocracy and visibility. The Defenders Advantage needs to be done optimising for transparency. Everyone affected needs access to see the decision-making apparatus. This is usually done with a combination of on-chain voting, public forums and anti-collusion incentives.

If the coordinators are creating something new, then Defenders' Advantage goes to the doers.  This requires an Actiocracy where a team can form, capable and committed to the results, and with complete control over their own scope and communication. If they are held accountable to their results, then their autonomy supersedes full transparency.  (When they succeed, and create a common good, transparency and vetocracy get introduced then to defend the assets they created.)

This is usually done with subDAOs, squads or other lighter gates on joining collaboration, like multi-sig rights and private communication channels.  And when it comes to incentives, they're usually aligned to results over participation.

## Put this in action

- [Introduce gates on collaboration](/practices/gates)
- [Work in squads](/practices/squads)

