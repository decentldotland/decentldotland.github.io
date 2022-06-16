# Decent.Land update #7

Welcome to our biggest update yet. We just shipped a proof-of-concept for Ark - a multichain upgrade for ANS - plus more lore, deeper integrations with Lens, and more.

## Ark Protocol
The major piece of work behind the scenes lately has been on Ark. Ark is a protocol which will power decent.land's token-gated communities **and** will be useful for any Arweave-based app that needs to read user data from other chains.

We see Ark as the _multichain identity protocol for web3 social_. It integrates with ANS as a universal identity for the permaweb and other chains. When it is live, you will be able to sign into Ark with both your Arweave and Ethereum addresses simultaneously, and link the two in your ANS profile.

This mechanism will make it possible for decent.land token-gated communities to read assets from any chain to allow or deny access to particular groups. We are also already working on a Telegram integration to gate access based on held assets!

## Lore
On the lore side, decent.land’s story is starting to get more visual. Since our last update the decent.land Art Director, [Lee Tyrrell](https://twitter.com/GreenT128), has shaped individual art objects for beaches of Yowunas Maias. Check a sneak-peek of the art created so far: [spent campfire](https://github.com/decentldotland/decentldotland.github.io/blob/main/img/spent_campfire.jpg?raw=true), [wormskin](https://twitter.com/GreenT128/status/1534113121958338560?t=dCctOGkv88odoS9cRGJBRw&s=19), and [fortified settlements](https://twitter.com/GreenT128/status/1535817353111420929?t=8J0Zj8ELC9gf-B-xghu4yw&s=19).
 
Missed the story? Read chapters [one](https://leetyrrell.medium.com/a-decent-land-chapter-one-ae611cdd4e08), [two](https://leetyrrell.medium.com/a-decent-land-chapter-two-f489272e3c69) and [three](https://leetyrrell.medium.com/a-decent-land-chapter-three-abd06717b599).

## Product development

* We integrated [phaver.com](https://phaver.com/) in the Lenster feed. Now it aggregates from Lenster.xyz and phaver.com. Check the details [here](https://github.com/decentldotland/weave-aggregator/releases/tag/v0.3.4).
* We published a drop-in module to utilize ANS identity badges in React apps. Check it [here](https://github.com/nanofuxion/ans-for-all). 
* The [Lens protocol v4](https://github.com/decentldotland/public-square-ui/pull/4) was integrated into the upcoming public square UI. 
* [Ark Network](https://github.com/decentldotland/ark-network), a protocol for linking verified multi-chain addresses (identities), which consists of an oracle address on Arweave network and other data registry contracts on EVM (and possibly non-EVM chains) with a validation backend, was finished. The protocol supports Telegram identity linkage with the multi-chain addresses as well.

## Ongoing developments

*[Ark Network](https://github.com/decentldotland/ark-network) will experience some upgrades and further development.
* ANS 2.0 UI is in progress and will bring you more to look at.
* A cache layer for weave-aggregator to enhance the UX of the Permaweb Explorer is  undergoing performance improvements for next week

## Previous updates
* [#1](https://blog.decent.land/2022/04/11/decentland-update-1.html) 
* [#2](https://blog.decent.land/2022/04/25/decentland-update-2.html)
* [#3](https://blog.decent.land/2022/05/06/decentland-update-3.html)
* [#4](https://blog.decent.land/2022/05/13/decentland-update-4.html)
* [#5](https://blog.decent.land/2022/05/24/decentland-update-5.html)
* [#6](https://blog.decent.land/2022/06/03/decentland-update-6.html)
