# **Vision**

Our project is a card database which a user can organize a card collection with and trade it with other users. Trading card game players/collectors generally accumulate a high volume of cards and may not have a good way of tracking their inventory and hence this software seeks to alleviate that.

This product is for the following two users:

1. Trading Card Game Players. These are players who aim to organize and keep track of their physical collection. They may also enjoy theory-crafting and building decks.
2. Trading Card Game Collectors. These are players who collect cards more than they play, and would greatly benefit from a tracked collection.

This software significantly simplifies the process of tracking and organizing a collection. There currently is not an easy to use, efficient method of keeping a digital collection. Players currently use either Microsoft Excel or less optimal solutions like MTGGoldfish's collection feature. Our software will fulfill players' needs for a better card collection software. 

Our approach will be the most user-friendly option available. Firstly, ease of use will be a top priority, so that users can record their collections as quickly and simply as possible. They will also be able to filter and search through their own collection with precise options. Secondly, users will be able to compare collections with each other and even set up in-person trades. This will be extremely unique to our software.

# **Software Architecture**

This project will be accomplished using Python at its core. The Qt library for Python will be used to create a functional, straightforward, and user-centric GUI. The official Magic: The Gathering API will be utilized to populate missing information about a user's cards. A MySQL database located on a remote server will be used to store information about each user's card collection.

The majority of data we will be accessing is card information, such as name, set, art, spell type, price, and more. The multiverseid variable or the id variable, which are unique card identifiers, will be the primary key for the  data we store. The project will be utilizing the client-server model where the server will be resposible for handling user and card data, while the client will be primarily used for user facing experiences. 

# **Challenges and Risks**

The single most challenging aspect of this project is the unfamiliarity some of us have with the game Difficult to code Magic: The Gathering  software having never played the game.
Solution: learn about the game first and foremost. Teach each other, maybe play a few rounds.






