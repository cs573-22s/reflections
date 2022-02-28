# Week 5 Reflections
*[Link to Visualization]*

For this week, I looked at a visualization made by a redditor to show the hottest and coldest temperatures around the
world based on latitude. The author ([u/neilrkaye]) explains in a comment that they created this visualization by first 
using ggplot to create a number of images corresponding to different latitudes. Those images were then stitched together
using ffmpeg to create the animation shown in the post. At the moment there is no interactive version, however the
visualization definitely has the potential to be converted into one. The most obvious option being to make the latitude
line draggable. It might also benefit from being able to select a smaller portion of the globe on the longitudinal axis. 
It is also somewhat unclear where/how the data was sampled. The author linked the public dataset ([Berkeley Earth]) used
to create the visualization, but without reading through their sources it is not immediately clear how the data was
collected. The  visualization would also benefit from more use of color on the world map as it could help provide a
better overview of the entire world.

[Link to Visualization]: https://www.reddit.com/r/dataisbeautiful/comments/sq0pgh/temperature_range_between_coldest_and_hottest/?utm_source=share&utm_medium=web2x&context=3
[u/neilrkaye]: https://www.reddit.com/user/neilrkaye/
[Berkeley Earth]: http://berkeleyearth.org/data/
