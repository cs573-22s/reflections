This week I found a visualization from r/dataisbeautiful about the game Wordle. I have been obsessed with
Wordle for the past few weeks so it was fun to see what people have made in terms of visualizations.

Link: https://www.reddit.com/r/dataisbeautiful/comments/sgc5g6/oc_how_good_is_your_favorite_wordle_starter/

The visualization looks at a subset of a ranking of different starting words in the game. From what I can tell
after a cursory glance of the source provided in the citations, they use a bot to make guesses for particular words
then ranks them based on how many guesses it took to guess all available words in the game, the word salet being the most popular
word. The visualization provides a histogram for the number of guesses it took to get a valid solution. The author also 
provides statistics for the average number of combinations after the first guess such as an average value of the score that you
would get after the first guess.

Personally I have a number of issues with the visualization just as someone reading it for the first time. First, I am not sure about the 
meaning of the colored letters at the top of each word in this context, it's not clear whether or not this is some sort
of histogram or an indication of ranking. Second, the fact that the author is using terms of statistics they came up with
such as "Match Score" and "Avg. Remaining" and only provides the meaning of these terms in small text at the bottom of the visualization
is very confusing. I would recommend the author to possibly document what each field means at the top of the visualization with
an example. Finally, it would have been nice if the author had labeled their axes just so that at first glance I would have had
an idea of what the chart was instead of guessing.
