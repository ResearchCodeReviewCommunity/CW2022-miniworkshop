# Code Review During Research

Collaborations Workshop 2022 mini workshop

## Build the slides

The slide show is written in markdown, to be turned into a HTML
slideshow (reveal.js) with pandoc. You'll need
[cmake](https://cmake.org/download/) (3.17+) and
[pandoc](https://pandoc.org/installing.html) (2.10+).


Start by cloning this repository

```
git clone git@github.com:ResearchCodeReviewCommunity/CW2022-miniworkshop.git
```

In the project's root directory, build the slides with

```
mkdir build && cd build
cmake ../slides
make
```
