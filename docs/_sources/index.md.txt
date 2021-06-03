Lab1 Report
================================

Title: Dependency Analysis and Dependency Graph on EnglishPal

Author: 黄文心、朱彩凤、朱倩

Date: 2021/5/20

Inroduction
==================

We want to avoid the Big Ball of Mud antipattern in our software application. In this experiment, we do dependency analysis and draw dependency graph about it and analysis the question about the health status of EnglishPal’s current architecture.

# Materials and Methods

In this lab, we study the dependency relationships among modules (or classes) in the source code of EnglishPal .We use Snakefood[1] tool to generate module level dependency graph, and use Mermaid tool to draw class / function level dependency graph. 

Graphviz (graph visualization), the abbreviation of graph visualization tool, is an open source tool of Bell Labs. The main purpose can be specific language (DSL) script for visual output, support JPEG, PDF and other output styles. And it is very good cross platform, has supported Linux, MAC, window multi platform, binary installation mode, provides Fedora, Ubuntu, RHEL, Solaris, MacOS, windows and other systems.Using graphviz tool, using script output visual graphical interface, rapid graphical thinking.

Mermaid is a library for drawing flow chart, state chart, sequence chart and Gantt chart. It uses JS for local rendering and is widely integrated into many markdown editors.As a JS rendering library, mermaid generates not a "picture", but a piece of HTML code, so it is much safer.

# Results

- The module-level dependency graph of EnglishPal
  - Code: [https://github.com/lqzcf10/lab1/blob/master/source/mermaid.txt]( https://github.com/lqzcf10/lab1/blob/master/source/mermaid.txt)
  - SVG: [https://github.com/lqzcf10/lab1/blob/master/source/graphviz.svg]( https://github.com/lqzcf10/lab1/blob/master/source/graphviz.svg)
- The class/function-level dependency graph of EnglishPal
  - Code: [https://github.com/lqzcf10/lab1/blob/master/source/EnglishPalDependency(Graphviz).txt]( https://github.com/lqzcf10/lab1/blob/master/source/EnglishPalDependency(Graphviz).txt)



# Pros&Cons

- Pros:This project framework is clearly structured, easy to analyze and maintain and improves functions properly
- Cons:Basic functions are fully determined, with low room for further innovation and many places hava to be improved



# Discussions

Using snake food tool, we can analyze the dependencies in project code and generate dependency graph for English pal
Graphviz (graph visualization) is the abbreviation of graph visualization tool, which is an open source tool of Bell Labs.
Using graphviz tool to generate dot file, mermaid draws the input dependency into function level dependency graph,
Through dependency analysis and the drawing of englishpal dependency diagram, we can see the framework structure of the project more clearly and help us understand the question about the health status of EnglishPal‘s current architecture.

# References

[1] [Snakefood User Manual](http://furius.ca/snakefood/doc/snakefood-doc.html)

[2] [Graphviz Online](https://dreampuf.github.io/GraphvizOnline/)

[3] [A Brief Guide How to Write a Computer Science Lab Report](https://thehackpost.com/a-brief-guide-how-to-write-a-computer-science-lab-report.html)

[4] [Read the Docs](https://readthedocs.org/ )`