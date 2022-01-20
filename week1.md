### Wordle

# What is Wordle?
Wordle is a recent trend that has swept through social media and pretty much every friend group. It is a simple game where you try to guess a daily word with only 6 tries, but after each guess, you get more information about what letters are or are not in the word. 

# A Word on Wordle

In the [article I chose](https://towardsdatascience.com/a-frequency-analysis-on-wordle-9c5778283363), Behrouz Bakhtiari, a professor from DeGroote school of Business, did an analysis on the frequency of letter, their positions, and how many letters certain starter words revealed, to try to find the best "starter word". That is the first word you guess to try to get as much information as possible. The graph shown here:<br />
![frequency of letters graph](https://miro.medium.com/max/510/1*V30LAurxr-HSYJqQHPMAxQ.png)

Shows the frequency of each letter in 5 letter words. As you would expect letters like "a", "e", "s', and "o" are quite frequent. (Interestingly, the most common letter in the english language "e" is not the top letter, but rather second to "a".) Having those, you could try to get a word that contains the top 5 letters: (a, e, s, o, r) searo? reaso? Not sure if those are words. This might be a good idea to get the letters in the word, BUT if those letters are the most common, whats the point of knowing if they are in the word, if you don't know where they are in the word? The author goes on to study the frequency of the top letters by position in the 5 letter words, as shown here:<br />
![position frequency](https://miro.medium.com/max/510/1*z3-jyWXCvHkxM4SOZv7tcg.png)

This gives us a better idea of where we should place the letters in our perfect 5 letter word. The author finds some words that match this as close as possible and compares their scores in the below visualization:<br />
![top word scores](https://miro.medium.com/max/500/1*afGnRj1YwnzF0myGdVrJ8Q.png)

The author identified the top word to be "Aries" (the latin word for ram) and then found, on average, how many letters it identifies (around 2) and how many positions it identifies (~0.6). (Unfortunately this word isn't in the wordle list so the author sugguested Orias or Serio)

# A Word on A Word on Wordle

The methods in this article are pretty sound for finding out how well a given word would preform on 5 letter words, but it doesn't answer if those words would be good at identifying Wordle words. I think some analysis on specifically past Wordle words would yield better future results. For example, if wordle words are never plural, then the frequency of the letter "s" should drop significantly. I think there is also an opportunity to dive deeper and do the same scoring simulations the author did on every candidate starter word. This would give a clear ranking on every single 5 letter word available as to what is the best (and worst) words to start with. We could take this further and create some kind of method to determine the optimal guesses at each stage. 

# My Words on Wordle

There is further potential for visualization here as well. The famous Wordle emoji blocks are a marvel in visualization in and of themselves:<br />
Wordle 215 5/6<br />

⬛⬛⬛🟨⬛ <br />
🟩🟩⬛⬛⬛ <br />
🟩🟩⬛⬛⬛ <br />
🟩🟩⬛⬛⬛ <br />
🟩🟩🟩🟩🟩 <br /> (ignore my poor performance)

This little block clearly conveys how well you did, what your stuggles were, and, most importantly, it doesn't spoil anything to anyone else. everyone who played knows exactly what is happening and for new users it sparks thier curiosity. There are so many opporunities for using this brilliant little square. 