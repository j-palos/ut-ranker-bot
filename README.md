# summoner-ranker
Will automatically rank and display the players of the UT Diamond+ discord server.

Currently takes, as input, a file named "players.txt", a plain text file with summoner names seperated by new lines, and outputs a descending ranked order of players
to a file named "sorted-players.txt". 

You will need to provide your own riot api dev key in a file called RiotConsts.py and configure the api calls for your region.
Later I'll add the ability to drag and drop region names.

!Important! There is currently NO error checking implemented, so if an api call returns invalid data, 
ie the summoner doesn't exist and so there is no summoner ID, the program will crash. This needs to be fixed asap for production

Ver 0.0.1
Set up the riot api calls, basic skeleton

Ver 0.0.2
Added primary functionality to sort summoners given a file of igns, formatting of output still needs cleaned up.

TODO:
1. Finish the discord bot part.
2. Clean format of output.
3. Make comparison cleaner, using cmp override or equivalent in python 3
4. Implement Fluid Error checking

