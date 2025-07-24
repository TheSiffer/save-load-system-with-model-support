# Save and Load System with container support

This is a forked project based on the Save & Load System in Unity by ShapedByRainStudios.

Find their channel below with the original explanation
`youtube.com/@ShapedByRainStudios`


Forked changes explained below

The original project features a solid save and load system with the exception that it only saves data of one system. If you have multiple systems that need to store and read data, then this approach poses problems in keeping data consistent across all individual systems of a game. Data forms like GameData, PlayerData, PreferenceData are implemented in this fork, but you can add as many as you'd like easily. 


Technical Explanation

The GameData file is a container that contains multiple fields and is written and read from the save file. When in reality, a game will have multiple parts that need to individually store data like PreferenceData, PlayerData and many more. These have to then be wrapped in another container such that the structure is consistent and any other data types can be stored as well.  

This save and load system will be built on top of the existing system and allows the developer to add as many data containers as they want and have the save and load system adjust automatically. 
