#### Reflection 5 - 02/13/2022
#### Mingjie Zeng (671222265)
#### Email:mzeng2@wpi.edu
----

This week's reflection comes from The Pudding: https://pudding.cool/2017/05/song-repetition/. This is an investigation of the repetition of lyrics in pop songs.

The author analyze the repetitiveness of a dataset of 15,000 songs that charted on the Billboard Hot 100 between 1958 and 2017 based on the hypothesis that proposed by a computer scientist Donald Knuth about The Complexity of Songs.
It's not easy to translate the feeling of repetitive into a numerical feature. Even if there are the same number of repeated words in two versed of the same length, the repetition of these two verses may not be the same. 
So the author use the Lempel-Ziv algorithm to compress the repeated sequences to see the proportion of repeated parts in the lyrics. 
Through this way, the author get the distribution chart of compressibility of 15,000 songs from 1958 to 2017, excluding 20 outliners:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-main.jpg)

The percentages on the x-axis are not evenly spaced. The author use a logarithmic scale with the property that, for any given song, a song that compresses half as small is a fixed distance away. For example, the distance between 20% and 60% is the same as between 98% and 99%. 

And when the 20 outliners songs are included in this distribution, the chart would be like this:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-main2.jpg)

To achieve this goal, the author also visualize the process of lyrics compression. When the algorithm scans the lyrics to find chunks of text that exactly match earlier parts and after finding the repetition, the authoe replace the later one with a marker pointing back to the occurrence of the first time:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-compression1.jpg)

And here is the computation of the redution size:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-compression2.jpg)

And here is the whole prograss of the compression of texts:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-process.gif)

And the author also makes a list of the most repetitive songs among decades:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-most.jpg)

And finally, the author makes all repetition of popular music by year a folding line Chart to observe the trend:

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-whole.jpg)

In addition to the above, the author considers the repetition rate of lyrics by different authors, as well as comparing the repetition rate of lyrics by artists from different periods. 
This distribution also shows the phenomenon that the repetition rate of the lyrics gradually increases over time.

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-artist.jpg)
![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-artist2.jpg)

An even more interactive and interesting point is that users can view the repetition rate of lyrics of different songs by specific artists.

![image](https://github.com/JasmineZZZ9/reflections/blob/master/pics/r5-artist3.jpg)

----

I choose this investigation for several reasons:
- The topic is interesting creative, lots of people may be curious about this but may not get down to it.
- It's very nice about the idea of translating the repetition of lyrics into the compression rate of the lyrics, making this a comparision feature.
- The way of presenting the compression procedure is fun and intuitive.
- The use of a logarithmic scale with the propotion of the songs compressed is clever and flexible.
- This project is also very interactive, as users can view the repetition rate of lyrics of different artists in different periods, and can view the repetition rate of lyrics of their favorite artists separately, and the display is also very straightforward and easy to understand.





