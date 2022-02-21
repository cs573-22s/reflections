###### Marcus Chalmers 
###### CS573
###### 1/24/2022 
###### Reflection Week 2

["English Letter Frequency Counts: Mayzner Revisited"](http://norvig.com/mayzner.html)

While looking for different data visualizations, I started looking for those that show word frequency in English.
I found this one particular [youtube video](https://www.youtube.com/watch?v=7XQRduB6oTM) where someone made an animated display, reminiscent of much of the
work done with D3 however, I found the original article where they took the data from had much more information to
offer, and I felt would pose as a more interesting discussion topic. While word frequency studies have been done in the
past, modern computing and databases have made the process much easier. Peter Norvig took Google books' Ngram raw data
set, which already reports word counts for the number of times each word is mentioned in the books Google has scanned and compiled that data.
This massive data set included 97,565 distinct words mentioned over 743 billion times.

![Data for top 50 words](https://github.com/mchalmers/reflections/blob/master/week2-1.JPG?raw=true)

The data is displayed in many different ways in this article, however, they mainly consist of bar graphs. I don't think this
is a bad decision for comparing counts. It's a very effective way to show differences between word counts on a common
scale. However, for this first graph, it's an interesting point to mention that the distribution looks like that of a
[Zipf distribution](https://en.wikipedia.org/wiki/Zipf%27s_law). Considering the study of linguistics is where this trend was discovered it would be
reasonable to want to see a line graph overlayed on this bar graph to further show the correlation between word frequency
as you continue lower. The world length bar graphs are interesting and I would recommend looking at them for fun but,
they're just standard bar graphs.

When the article goes over letter frequency they create another bar graph which is easier to see the differences between letters, however, they also create this colored-bar chart. Showing the same proportions of the bar chart just without the standardized
axis. While they're still in descending order you can't tell how much less "s" is than "e" for example as easily as you
could with the bar graph. Although when showing letter popularity based on the position this condensed format is more intriguing 
it does still make comparing specific letters difficult if they aren't near each other. One interesting thing to note about 
this bar chart is the use of color. Since everything is in a line there's no need for each letter to have a distinct color 
so high contrast and bright colors can be reused, making it easy for most everyone to see the difference at a moment's glance.

![letter frequency](https://github.com/mchalmers/reflections/blob/master/week2-2.JPG?raw=true)
![letter frequency in words](https://github.com/mchalmers/reflections/blob/master/week2-3.JPG?raw=true)

The last representation of data that I thought was interesting in this dataset was the table of bigrams. Each two-letter pair
was displayed showing their frequency in a rather unique way. While most of the letter pairs hardly occur and are  
indistinguishable from any other, when a pair is used a significant amount they end up highlighting the letters
making them stand out more. The only problem here is the dark color of the bars and text make them just a little hard
to read.

![bigram frequency in words](https://github.com/mchalmers/reflections/blob/master/week2-4.JPG?raw=true)
