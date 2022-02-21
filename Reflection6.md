CS 573 - Data Visualization

Botao Han

Reflection 6

Source: https://www.reddit.com/r/dataisbeautiful/comments/swg5el/oc_comparing_play_time_vs_number_of_players_for/

This week I found a interesting post on dataisbeautiful Reddit forum. It's a chart that Comparing relationship Play Time and Number of Players for Popular BoardGameGeek Categories.

I am not much a board game lover. But I found some interesting properties in this graph. For each game, there is quite a high probability of a 0 hour playtime. Some people guess that the creator of this graph use some kind of smoothing tool to make the graph more elegant. The author later proved that the assumption is right, the underlying probability densities are estimated with kernal density estimators which don't obey boundary constraints. 
