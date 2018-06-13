# WHY?
The video game item market is a $50 billion industry. Virtual items carry tremendous value, yet there is neither proof of ownership nor regulation on these trades. For instance, in 2011, a virtual planet in Entropia Universe, a massively multiplayer online virtual universe, sold for a record-breaking $6 million USD. Fraud and simple software glitches represent far more than minor headaches--for some people, it can be a huge financial crisis. 

The high value of these items in turn creates a huge black market. This is an inherently flawed practice. In order to acquire special items, players resort to breaking the rules, risking getting banned. Furthermore, this creates a toxic playing environment. For instance, the League of Legends account selling market creates a system where players can buy "status", leading to games with huge skill discrepancies that are no fun to anyone.  

# HOW?
Non-fungible tokens solve these problems by providing permanent, safe storage of an item and a regulation on item trading. This gives players a concrete proof of ownership on an item that will exist long after a game goes offline. The blockchain provides economic regulation which has no means of circumvention. Players can trade items without worrying about fraudulent transactions or software glitches, giving this huge market its much needed security. Furthermore, developers can regulate and even profit from trade. They can specify which can be traded while charging a royalty on others. Whereas allowing players to trade items like League of Legends skins would negatively impact profits, leading to the broken system of selling accounts, developers can now charge users a fee to transact. 

Our Ethereum Smart Contract is build on the OpenZeppelin template for ERC-721 tokens. We add a layer of functionality that makes these tokens more friendly to games, such as creating a token when an item is created, specifying the transferability of tokens, and others. 

Inventory relies heavily on Javascript and web3 calls. However, most games are not written in this language. To make integration easier, we have built an easy-access Docker server that requires a simple HTTP GET request to interact with the Smart Contract. This makes integration into any online game seamless. 

# WHAT'S NEXT?
The tokens developers create promise big changes for the gaming industry. They can choose to mint tokens for achievements and in-game checkpoints, giving other players a way to quickly verify the progress and skill of their peers. Or, developers can work with each other to agree on a class of items to create for both their games. A player can easily transfer between games, using a favorite item without any pause. 

Many of our features are still in beta. We are currently working on allowing developers to limit which tokens can be traded and to charge royalties on those that can be. 

With such big potential, it'd be hard for us not to continue working Inventory. Some companies working in the video game space have reached out to us, so we're excited to see what continued work holds. 

# FAQ

**How have you protected yourself from malicious third parties sending their own traffic to your Docker server, or from minting their own items?**

We have limited Inventory's use case to online games that are run on some remote server. This prevents malicious gamers from messing around underneath the hood. Furthermore, since developers will run the Docker server locally, there is no chance for anybody else to interact with it.

# USAGE
### As a player
1. Check if you have any items by entering your address on the "View Items" page.
2. Go to the "Play a Game" page and move your square to the far right side to complete the game.
3. Wait for your item to be awarded.
4. Re-enter your address on the "View Items" page and check that you have the Champion's Hat.
5. See your new hat in action on the "Play a Game" page.
### As a developer
1. Go to the "Manage Games" tab.
2. Register your wallet as a game with the name of your choice.
3. Add new rewards to the game that you might assign to users.

Developed by Derek Huang and Ryan Holmdahl 
