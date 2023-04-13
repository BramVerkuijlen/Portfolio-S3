
# Game API
*From Console to Code: A Research Analysis of Top Game APIs"*


## Reasons for Using an Existing Game Data API
***

As part of my project, I needed to gather a significant amount of game data. While I could have tried to collect this data manually, I quickly realized that this would be an extremely time-consuming and challenging task.

Using an existing API to collect game data made a lot of sense for several reasons. Firstly, it saved me a lot of time and effort. By tapping into an already established API, I didn't need to spend time developing custom data collection scripts or trying to reverse engineer game mechanics to gather data. Instead, I could quickly and easily retrieve the information I needed in a standardized format.

Additionally, using an existing game data API would most likely give me access to reliable and accurate data. Game data APIs are usually maintained and updated by the game developers themselves or other reliable sources, which means that the data provided is likely to be current and accurate.

## Steam API
***

Initially, I planned to use the Steam API, a platform developed by Valve for purchasing and playing games, for my research project. My decision to select the Steam API was based on my familiarity with the platform and the convenience of accessing user data via Steam's account system, including game libraries and friends lists.

However, during my research on the Steam API, I discovered that it did not offer the specific information I required for my project, namely detailed information about games. While the Steam API provides basic information about games such as their title and description, it does not offer more comprehensive information such as genre, rating, or multiplayer capabilities.

Therefore, I had to consider alternative data sources to obtain the necessary game-related information for my research project.

## RAWG and IGDB
***
After determining that the Steam API did not provide the detailed game data I needed, I began to explore other possible APIs. Two options that stood out were RAWG and IGDB.

RAWG is a video game database and game discovery platform that provides an API for developers to access game-related data. RAWG's API offers a wide range of information about games, including game descriptions, release dates, ratings, platforms, and more.

IGDB, or the Internet Game Database, is another popular option for game data API. Similar to RAWG, IGDB provides developers with access to a vast amount of game-related information, such as game descriptions, ratings, and release dates.

### Diferences
Although RAWG and IGDB have similar functionality, there are some differences between them:

Data Coverage: The RAWG API has more extensive data coverage, with over 500,000 games in its database, while the IGDB API has around 200,000 games.

Data Quality: Both APIs provide high-quality data, but the RAWG API relies on user contributions to update and verify data, while the IGDB API has a team of editors that review and update the data.

Pricing: The RAWG API offers a free plan that includes 1000 requests per day, while the IGDB API offers a free plan with limited access and a paid plan for higher usage.

Features: Both APIs offer similar features such as game search, game details, and reviews, but the RAWG API also provides game recommendations, collections, and user profiles, while the IGDB API has a more advanced search capability with a range of filters.

API Structure: The RAWG API is RESTful, while the IGDB API uses GraphQL. RESTful APIs rely on endpoints to access resources, while GraphQL APIs allow clients to specify the data they need, reducing the amount of data transferred over the network.

### Why I Chose IGDB

After looking further into both API's I eventually decided on using IGDB for a couple of reasons:

Firstly, IGDB had more reliable and consistent data quality, which was important for the accuracy of my application. While RAWG relies on user contributions to update and verify data, IGDB has a dedicated team of editors who review and update the data, ensuring a higher level of accuracy.

Secondly, I found that IGDB's API was easier to use and had more detailed documentation, making it simpler for me to integrate the data into my application. Additionally, IGDB's API offered more advanced search capabilities with a wider range of filters, which was important for the complexity of my project.

Lastly, I found that the pricing plans for IGDB were more reasonable and flexible for my needs. While RAWG does offer a free plan, the limitations on requests per day were more restrictive than IGDB's free plan, which provided me with enough access to test and develop my application before needing to upgrade.

Overall, while both RAWG and IGDB are great options for accessing game-related data, IGDB's superior data quality, API functionality, and pricing plans made it the better choice for my project.

## Conclusion
***
While the Steam API was my initial choice, it did not provide the detailed game data I required. This led me to consider alternative options, such as RAWG and IGDB, both of which are game data APIs that offer extensive game-related information.

After weighing the differences between RAWG and IGDB, I ultimately chose the IGDB API for my project. Its superior data quality, more advanced search capabilities, and flexible pricing plans made it the better option for my needs. Additionally, the Steam API provided me with access to user data, which was crucial for personalizing the gaming experience.

Overall, the IGDB API and the Steam API are excellent choices for any game-related project due to their comprehensive data coverage and powerful functionality.

