# A Brief History of DAOs — where it all started

“Decentralized autonomous organization”... a somewhat pretentious phrase that was bluntly shortened to “DAO”.

DAOs, like NFTs, are a concept that have seen an exponential increase in interest of late. Plenty of blockchain initiatives become a DAOs nowadays, and whenever traditional media refers to DAOs, the term “craze” is not far behind.

So what‘s it all about? To put it simply, DAOs are more or less what they claim to be: decentralized, on-chain entities (to certain degrees) making decisions based on a voting mechanism.

There are more precise definitions, but in their quest to accurately describe what an ideal DAO is, these definitions fail to cover the superabundance of implementations that are out in the wild. Ideally, they should represent a bottom-up organizational system, in contrast with a centralized company model…but for a big chunk of them, that’s not the case in reality. “Power users”, “core members” or simply “whales” could drastically affect the outputs of a DAO.

Again, in theory, all the activity of a DAO should be represented on-chain in a seamless manner (an initiative is proposed, a vote is held, according to the result of the vote an action is conducted), in practice, the majority of those initiatives truncate their workflow in a way or another and are in a transient status to achieve a unified on-chain flow.

A more explicit definition could be made by simply listing the constituent parts present in basically every existing DAO:

* a mission
* a treasury
* a set of governance rules
* members
* ...all glued together by smart contracts

To look at how DAOs came to be, we should look at their overall history.

## Block 1428757

That’s when the first DAO ever was created on the Ethereum chain. In more conventional terms: the date was 30 April 2016. It was simply called “The DAO”, and the expectations were high (where “high” is a gross understatement).

As one can see the concept, again like in the case of NFTs, is not at all a new one, in terms of blockchain history. The similarities stop here. Until 2020 NFTs were mostly a quiet piece of tech. DAOs, however, shook the world from their inception.

I assume that there are at least a few of you who don’t know the history behind “the DAO”, so strap in - you're about to hear one of the wildest crypto stories of them all: black hats, white hats, an existential threat to Ethereum itself, an astute resolution; all mixed in a way that Dan Brown would be jealous of.

The DAO was a digital construct created by members of the Ethereum community; one could pinpoint the Jentzsch brothers (two German coders involved in a blockchain startup called Slock.it) as the founders, but given the open source character of the code repository and the ethos around it, it’s hard to conclude with certainty the actual number, identity, and contribution of the founders.

It was built with the objective to become:

> … a[ decentralized autonomous organization](https://en.wikipedia.org/wiki/Decentralized_autonomous_organization) that exists as a set of[ contracts](https://en.wikipedia.org/wiki/Smart_contract) that resides on the[ Ethereum blockchain](https://en.wikipedia.org/wiki/Ethereum); it did not have a physical address, nor people in formal management roles. The original theory underlying the DAO was that by removing delegated power from directors and placing it directly in the hands of owners the DAO removed the ability of directors and fund managers to misdirect and waste investor funds.


> The DAO was intended to operate as “a hub that disperses funds (currently in Ether, the Ethereum value token) to projects”. Investors received voting rights by means of a digital share token; they vote on proposals that are submitted by “contractors” and a group of volunteers called “curators” check the identity of people submitting proposals and make sure the projects are legal before “whitelisting” them. The profits from the investments will then flow back to its stakeholders.

In other words, the DAO worked as a VC firm: people pitched business ideas and investors voted on how much and under which conditions should the DAO invest in those ideas. The voting power was proportional to the number of DAO tokens one held.

The mechanism described above drew a lot of attention from the Ethereum community - attention that further translated into money pouring into the DAO’s treasury. Keep in mind that at the moment Ethereum was in its infancy and there was little to do inside the ecosystem. Creating an autonomous entity, that cut the management cost burden and let crypto users directly invest in “real life” ventures, sounded pretty cool. 

In a single month, the DAO managed to raise over 14% of the total existing Ethereum coins, at the time representing over $150 million. Over 11,000 individuals flocked to become a part of this new and enticing community.

## For want of a nail

It may seem that there’s no drama to be found here. Another crypto success story!

That’s obviously not the case. So what happened?

On the fateful day of 17 June, 2016, the DAOs treasury started to be drained by around 100 ETH/second. An unknown black hat hacked the DAO and he threatened to steal all the ETH in its custody.

Wait. Pause for a second. _Why didn’t he just take all the money in a single transaction and run? That’s how bank heists work, don’t they? A masked man storms into the facility, grabs all the money and disappears in a cloud of dust._

Hold your horses. I promised you a thrilling story, not an action movie. The attacker exploited a vulnerability that allowed him to withdraw only limited amounts of ETH/transaction, so he had to call that function in a loop and withdraw only a portion at a time. There were some built-in limitations, like the balance of DAO tokens that the attacker had initially and so on.

There is a recurrent analogy made to understand better what actually happened: Imagine that you are the attacker and you want to defraud a faulty ATM. You have a card linked to a bank account that has a balance of 100 dollars. You ask for the $100 from your account, and the ATM outputs them. The flaw in the ATM is that it can read your balance and execute your withdrawal. Only after the withdrawal is executed will it try to update your balance. Meanwhile, you can ask the ATM to give you another $100, and it will, given the fact that it didn’t update the balance to 0 in the first place. One could do this virtually forever.

This is called a reentrancy attack. One has to understand that at the moment of this particular hack, Solidity, the programming language that Ethereum uses, was only several months old. In this case, a lot of stuff was yet to be discovered - in this case, with dire consequences. Now you can write a smart contract with a reentrancy guard, and it simply prevents a similar exploit with only a few lines of code. Yep - just a handful of lines could have prevented this attack. 


## A small detour: Vitalik’s fault?

The flaw that was exploited can be considered so trivial today that it can make you wonder what the programmers were thinking. How could they not see such an obvious mistake?

Well… they were probably thinking of this:

DOs [Decentralised Organizations] and DAOs [Decentralised Autonomous Organizations] are both vulnerable to collusion attacks, where (in the best case) a majority or (in worse cases) a significant percentage of a certain type of members collude to specifically direct the D*O’s activity. However, the difference is this: in a DAO collusion attacks are treated as a bug, whereas in a DO they are a feature. In a democracy, for example, the whole point is that a plurality of members choose what they like best and that solution gets executed; in Bitcoin’s on the other hand, the “default” behavior that happens when everyone acts according to individual interest without any desire for a specific outcome is the intent, and a 51% attack to favor a specific blockchain is an aberration.

This is an extract from an [article](https://blog.ethereum.org/2014/05/06/daos-dacs-das-and-more-an-incomplete-terminology-guide/) called “DAOs, DACs, DAs and More: An Incomplete Terminology Guide”, written in 2014 by Ethereum founder Vitalik Buterin.

What’s the connection? I suppose that when you are building “THE DAO” on Vitalik’s chain…there is a huge chance not only that you are aware of Buterin’s thoughts, but you are actually using them as a blueprint.

As you can see, the bar was very high, even by current standards, when most DAOs probably fall into the DO category, if we were to use the classification proposed in the paragraph above.

Back then, they were dreamers, trying to construct “something that has a large degree of autonomous intelligence of its own”. Before all, a DAO was “automation at the center, humans at the edges”. With those ideas in mind, the developers behind The DAO created a baroque construct, the first of its kind. It was so vast and new that the little error that passed unaddressed was almost inevitable.

The whole story is basically a layered construct of crude ironies of fate, one laying on top of another, most of them linked with this article Vitalik wrote in 2014. 

The first irony I’ll address is the fact that the exploited loophole existed in the function that aimed to achieve that _collusion attack-proof feature. _The function which would have turned “The DAO” into a real DAO in the acceptance of Vitalik, killed the entire project. Below you will find the explanation:


The DAO had a “split DAO” function which was identified and published as a vulnerability days prior to the attack. This function was designed to enable participants of the DAO to transfer account balance and branch off to a new DAO, called the “child DAO”, in case they decided to go in a different direction after the conclusion of the vote. The process was simple, the network would check the participant’s balance and then transfer it to the child DAO. When the split is finished, the participant’s balance in the original DAO will be zeroed out.


However, this function had an issue. While the function itself worked perfectly fine, it allowed the participant to perform another split before the first one was completed. The balance was not zeroed out until the end of the split, the attackers used this vulnerability to their advantage. They were able to perform this split over and again for about two hundred times leaving the DAO almost empty.

The _child-making function_ was assuring the “A” in the DAO. Its purpose was to secure the continuity of the _default behavior, _disregarding the different points of view that could occur between humans while voting was carried out. In theory, it should have been working like this: You don’t like the project chosen by the majority? Fine, but don’t run off with your Ethereum and weaken the entity. Instead, make a little DAO that wants to invest in other projects, you can even work to make it bigger than the initial DAO, you can do anything as long as you keep the logic of investing running.

Of course, not the function itself represented the problem, and definitely not Vitalik’s thoughts about what it takes to be a DAO, but you have to acknowledge the irony.


## The time factor

Back to our boiler room. What was the Jentzsch brothers’ response? What about the Ethereum community?

Clearly, it was a race against time. With the money being slowly drained to the evil’s DAO child treasury, there were two tickers: one represented by the actual period needed to drain all the funds and one represented by a feature built-in into the DAO. Remember, the attacker didn’t direct the funds into his personal wallet, but in another DAO treasury, identical to the one he hacked, bound by the same smart contracts to the same rules. One of the rules stipulated a 28 day locking period for the funds entering a new DAO from the moment of its creation.

So, on one hand, the good guys had to devise a short time play to minimize the damage, and on the other hand, they had to solve all the mess entirely in 28 days. 

The first issue was solved rather unceremoniously. Jentz’s brothers pulled their white hats on and used the same exploit to drain The Dao faster than the evil genius. The aftermath of this race favored the white hats: 70% of the funds were safe for 28 days in the _good_ child DAO and only 30% were deposited in the _evil_ one. But what would have happened after 28 days? The hacker allegedly gained direct control over 2 million and probably tried to target the funds saved in the first phase.

Definitive action was needed. 


#### ## Block 1920000

After fierce debates, a solution was implemented on 20 June 2016. A “hard fork” starting from block 1920000 erased all the effects of the hack. By the will of the majority of the miners, all the funds that were initially in the DAO smart contract were safely deposited in another smart contract and the rightful owners of the funds were refunded.

This resolution was preferred over two other potential action courses: a soft fork (the miners would no longer process any transactions that came from the DAO smart contract) and doing nothing. While some further technical complications would have hit the first alternate solution (the soft fork), so, in the end, it wasn’t taken into consideration, the second one, as crazy as it may sound, partially happened. 

Have you ever heard of ETC? It’s a coin that now ranks in the 28 positions on Coin Market Cap. It represents the reality where the Ethereum chain never made a hard fork ar block 1920000. On this chain, the hacker still owns all the coins he stole.

Some miners continued to consider this version as the one that deserved to be kept. Why? Some did it for money (the hacker made some promises for miners who will continue to back this version of the chain), some did it because they believed in the “code is law” narrative, it doesn’t matter. What matters is the aftermath.


## Takeaways

The DAO never managed to prove its potential. A flaw in the execution of the code killed not only that particular endeavor but the core philosophy behind the concept. 

The chain of ironies becomes now visible: the Ethereum foundation was forced to prove that not even Ethereum was a DAO (by Vitalik’s 2014 standards), by making a hard fork to correct the outcomes of an ill-coded DAO.

At the same time, the “default behavior” of the Ethereum chain was kept by implementing that hard fork, not by doing nothing, which meant that human input was still needed to counter rouge inputs. 

Even now, years after the event, DAOs still won’t venture too much into the unknown territory of machine autonomy. They seem to stick more to the _simple_ Decentralised Organization route. 

Maybe it’s time to forget the fear provoked by the abovementioned events and start to dream again!


## The story never ends

Those were the beginnings. What happened after? Well, for a rather long time, DAOs existed without drawing too much attention to them. After all, the DAO didn’t make ripples only in the crypto space. 

On July 25 2017, a little more than a year after the narrated events, the United States Securities and Exchange Commision (SEC), released a report that specified in clear that the tokens issued by The DAO were securities. This ruling bound the other entities incorporating operating principles similar to those of a DAO to keep a low profile, or to mold their mechanics in order to stay out of the loop. The majority of the decentralized exchanges (DEXs) that exists nowadays, are in fact DAOs, but their tokens, when it comes to the DAO part of their business, are used strictly for governance purposes. 

Years passed, the SEC’s focus in the matter of DAOs somehow diluted, the legal framework around the issue became a little more clear and the open source code repositories for various use cases grew and become more reliable. All these factors favored the emergence of a DAO renaissance. If we were to follow the standards that were set in 2014, it is still in its incipient phase. 

What do DAOs look like now? How are they built nowadays? How many types of DAOs are there? Those, and many other questions will be answered throughout this series. 

## Useful resources


* [A History of ‘The DAO’ Hack](https://coinmarketcap.com/alexandria/article/a-history-of-the-dao-hack)
* [The DAO of accrue](https://www.economist.com/finance-and-economics/2016/05/19/the-dao-of-accrue)
* [Analysis of the DAO exploit](https://hackingdistributed.com/2016/06/18/analysis-of-the-dao-exploit/)
* [DAOs, DACs, DAs and More: An Incomplete Terminology Guide](https://blog.ethereum.org/2014/05/06/daos-dacs-das-and-more-an-incomplete-terminology-guide/)
* [BOOTSTRAPPING A DECENTRALIZED AUTONOMOUS CORPORATION: PART I](https://bitcoinmagazine.com/technical/bootstrapping-a-decentralized-autonomous-corporation-part-i-1379644274)
* [BOOTSTRAPPING AN AUTONOMOUS DECENTRALIZED CORPORATION, PART 2: INTERACTING WITH THE WORLD](https://bitcoinmagazine.com/technical/bootstrapping-an-autonomous-decentralized-corporation-part-2-interacting-with-the-world-1379808279)
* [BOOTSTRAPPING A DECENTRALIZED AUTONOMOUS CORPORATION, PART 3: IDENTITY CORP](https://bitcoinmagazine.com/technical/bootstrapping-a-decentralized-autonomous-corporation-part-3-identity-corp-1380073003)
* [CRYPTOGRAPHIC CODE OBFUSCATION: DECENTRALIZED AUTONOMOUS ORGANIZATIONS ARE ABOUT TO TAKE A HUGE LEAP FORWARD](https://bitcoinmagazine.com/technical/cryptographic-code-obfuscation-decentralized-autonomous-organizations-huge-leap-forward-1391849871)