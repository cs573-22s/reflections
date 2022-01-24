# Week 2 Reflections

![Flame Graph](https://www.brendangregg.com/FlameGraphs/cpu-mysql-updated.svg)

This week my reflection is on flame graphs visualizations and their use for profiling application CPU time. Flame graphs
visualize the hierarchical breakdown of a task into its component times. While they can be applied to a broad range of
topics, they see the most use in profiling applications.

I found this great [post by Brendan Gregg] on what flame graphs are and how they can be used to more efficiently express
how an application spends its time. Most display libraries will allow a user to click on specific bands to zoom in on
the x-axis for easier viewing. Additionally, color can be applied to help distinguish different various important pieces
of information about the execution of a program such as the file or library a method originates. 

![Colored Flame Graph](https://www.brendangregg.com/FlameGraphs/cpu-mixedmode-vertx.svg)

In this example, Gregg shows a flame graph of a Java application. If we were debugging the performance, the colored
regions be important as they help to highlight what we have direct control over. The green regions represent time spent
by code within our control. Also while we would not be able to directly modify the orange kernel parts of the graph it
may reveal delays that could be avoided by choosing a different approach.

Gregg provides some examples using open source tools which he explains in his post for profiling and building flame
graphs for your applications. That being said, I have found I have found [Intel VTune] to be the easiest and most
straightforward approach for quickly debugging my C/C++/Rust projects as it has an easy installer, and you only need to
provide it with an executable to get started. However, [Intel VTune] does not provide built in functionality to export
these graphs so other projects like this [D3 Flame Graph Library] may also be helpful.

[post by Brendan Gregg]: https://www.brendangregg.com/FlameGraphs/cpuflamegraphs.html
[Intel VTune]: https://www.intel.com/content/www/us/en/developer/tools/oneapi/vtune-profiler.html#gs.mwo5ib
[D3 Flame Graph Library]: https://github.com/spiermar/d3-flame-graph