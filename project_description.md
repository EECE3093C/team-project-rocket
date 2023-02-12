# **Vision**

Our project is a card database which a user can organize a card collection with and trade it with other users. 
This product is for the following two users:
  1. Trading Card Game Players. These are players who aim to organize and keep track of their physical collection. They may also enjoy theory-crafting and      building decks.
  2. Trading Card Game Collectors. These are players who collect cards more than they play, and would greatly benefit from a tracked collection.
  
This software significantly simplifies the process of tracking and organizing a collection. There currently is not an easy to use, efficient method of keeping a digital collection. Players currently use either Microsoft Excel or less optimal solutions like MTGGoldfish's collection feature. Our software will fulfill players' needs for a better card collection software.

Our approach will be the most efficient iteration of a card collection software. Firstly, ease of use will be a top priority, so that users can record their collections as quickly and simply as possible. They will also be able to filter and search through their own collection with precise options. Secondly, users will be able to compare collections with each other and even set up in-person trades. This will be extremely unique to our software.



# **Software Architecture**
At a very high level we will be using the external Magic:The gathering API to populate information. We will also use the MySQL database to track the user's playing cards. 


# **Challenges and Risks**

The single most serious challenge we anticipate is users maliciously flooding the database. If we were to give a new user a collection they can freely add cards to, we run into problems when they add 5,000,000 Storm Crows to their collection and crash our server because the database can't store that. Furthermore, a person could run multiple users in an attempt to do this.
We will attempt to minimize this risk by setting a soft limit on the amount of cards any new user can add to their collection, at around 500 cards. So long as a user doesn't create large influxes of cards to the database, isn't spamming additions of the same card repeatedly, or otherwise indicating poor behavior deserving of restrictions, they will be free to add cards as they please. If they approach the limit and are in good standing, the limit will be raised for them. This way we will be able to mitigate poor user behavior and malicious acts towards our database, while sustaining genuine players and collectors.
