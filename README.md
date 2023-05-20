# Article DAO Overview #

https://valleydao-front-qioz-git-main-block-chain-valley.vercel.app/

https://www.youtube.com/watch?v=irwLxuqjb5A

[![Article-DAO](https://img.youtube.com/vi/irwLxuqjb5A)](https://www.youtube.com/watch?v=irwLxuqjb5A)

[<img src="https://github.com/Glitch-valleydao/Article-DAO/assets/113398351/6b175bbc-9c54-41bc-887f-da9011c9bc60" width="50%">](https://www.youtube.com/watch?v=irwLxuqjb5A)

DAO, decentralized autonomous organization is a concept that was introduced back at 2016, perceived to posits high potential as a concept that would potentially lead the advancement of Blockchain system and its community. It had shown to have high scalability, expanding its branches to fields ranging from labor, games, DeFis and many others that none would have thought blockchain would have implemented to. Practically in any space that required any means of governance, DAO had the potential to decentralize the underlying system. The success of NFT markets depend highly on whether the NFT was introduced to large groups of consumers, and the methods involved. In the case where the NFT itself is a kick-off brand where not much recognizes, its highly likely for them to collaborate with advertisers – mainly twitters in case of NFTs – to advertise the NFT, which associated benefit in return. However, the whole process from finding appropriate advertisers, and rewarding the advertiser for the work they have provided, is solely processed in the Web2 world, most likely communicated from peer to peer. No middleman nor any institution plays a role of it, which leads to lack of safety cautions, and even if so exists, it will lead to high dependency on the subject. Furthermore, advertisers’ low reputation will have no chance to take participation in the promoting procedures as it is hard for the NFT creator to reach them. 

We came across to a solution for the mentioned problems, which is to implement DAO with NFT promotion systems. This is expected to remove the role of a middleman, embrace transparent and fair promotion reward process, and along with all the good side effects that comes with decentralization. In the previous model of NFT promotion, the NFT creator would seek for writers that would write an article to promote the NFT. When the creator finds a writer that meets the standards, then both would agree upon a deal, creating a verbal/written contract. However, this contract’s safety is not guaranteed nor secure. When the writer has written the promotion article, the creator validates it and rewards the writer with the amount of the tokens mentioned in the deal. However, by interacting with Article DAO, it drastically changes the whole NFT promotion process to a point where both creator and writers, and even the NFT consumers would benefit from. A big picture of the Article DAO is as following. The NFT creator proposes a proposal to ADAO (Article DAO), with details regarding her standards and characteristics of how the articles she demands to be, along with tokens to be used to reward the writers that writes the articles. Whitelisted writers could then write articles and register it to the proposal. In case of writers that are not whitelisted, they must go through an approval process, in which they submit their Twitter handle for the community to decide whether the writer is a valid writer. Voters a.k.a. token holders will then vote on the articles whether the article is reliable, helpful, and meets the standards presented by the creator. 

<img width="987" alt="Screen Shot 2023-05-20 at 11 49 16 PM" src="https://github.com/Glitch-valleydao/valleydao-contract/assets/113398351/e8a6a2e9-09c5-4cc1-bb8b-2ec255acae89">
<img width="987" alt="Screen Shot 2023-05-20 at 11 49 26 PM" src="https://github.com/Glitch-valleydao/valleydao-contract/assets/113398351/c7aeec41-562f-4397-90af-579e992ba647">


Though the idea is innovative, yet it still encounters problems that are to be solved. First problem regards a situation where a user mints large quantity of tokens and use it to manipulate any vote results.  Let’s say there is a case where VoterA votes 1,000 d-tokens, and VoterB votes 1,200 d-tokens, both agreeing upon the acceptance of a certain proposal. However, VoterC who is a voter that shares interests with the denial of the proposal minted d-tokens a total of 2,201 barely passing the vote. In other words, whales (voters with large quantity of tokens) could easily decide the pass/denial of a vote by just minting more tokens. This is the natural problem of DAO as it renders the voting system useless, especially in early stages of DAO when there are not enough voters to create a fair voting progress. We have reached to a simple and efficient solution to ADAO. Our solution is to create two new variables associated to the voter – the number of votes the voter has won, and the number of challenges the voter had passed. Then these variables would be calculated arithmetically on-chain, creating a new trust-factor variable. The new variable would be used to vote, and the pending result will be based on the comparison of it.



<img width="425" alt="Screen Shot 2023-05-20 at 11 45 48 PM" src="https://github.com/Glitch-valleydao/valleydao-contract/assets/113398351/8df16af7-0dfc-4a47-87a1-7f5fc9fa1534">



In previous model of ADAO, when a whale decides to mint tons of tokens to barely win the poll, it will require harder efforts as the new model from ADAO applies other factors that are not buyable in calculation for the votes.

The other problem we have encountered comes from a situation where all the recent vote polls have passed, and users decides to render the vote and the DAO useless and unhelpful. We have come across the idea of implementing Markov Chain, which is a model that deduces a probability of each event using data of previous state events. For instance, in a situation where 5 writer registries were accepted in a row, using the Markov transition matrix calculation, we could deduce the fact that the next Boolean value will result to True in a probability of 3/4. This value, will then be used to be a standard for the next vote to pass, meaning 75% of the votes should turn to be true for the poll to be accepted. Markov values are able to be used to be the standards because we perceive it as means to measure voting tendencies. When writer registrations consecutively passes, we can assume that the standard for the registry is too low, hence we need to raise the standards (requirements for poll passing are harder).

<img width="787" alt="Screen Shot 2023-05-20 at 11 52 23 PM" src="https://github.com/Glitch-valleydao/valleydao-contract/assets/113398351/dca4873f-4f06-4b9c-8987-a705511c1bc4">

Overall, ADAO benefits all the NFT creators, writers, and even NFT consumers. NFT Creators, with the same number of tokens that would have been used to hire writers in Web2, could receive more promotion values as several writers participate in the process, creating more articles. Writers benefits from ADAO, especially writers with low reputation because they are also given chances to promote their articles through a fair competing environment. Lastly, since consumers are able to view promotion articles that are approved by a group of people, consumers now have greater accessibilities to better and more informative information. Potential function implementation would involve Avalanche’s gasless transaction. For a DAO to function properly, it is essential for it to have enough participants in the voting process. Implementation of gasless-transaction on Avalanche is the answer to rapid progression into a self-powered DAO, since easier accessibility by gasless votes participation allows explosive newcomers, enlarging the DAO community. 
