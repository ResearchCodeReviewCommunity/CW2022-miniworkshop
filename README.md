# Code Review During Research

Collaborations Workshop 2022 mini workshop

You can view the slides [*here*](https://researchcodereviewcommunity.github.io/CW2022-miniworkshop/slides.html).

## Contributing

The slide show is written in markdown, to be turned into a HTML
slideshow (reveal.js) with pandoc.

Start by cloning this repository

```
git clone git@github.com:ResearchCodeReviewCommunity/CW2022-miniworkshop.git
```

The slideshow is contained in directory `slides`:

```
slides/
    slides.md
	img/
```

The slides are generated and deployed at [CW2022-miniworkshop/slides.html](https://researchcodereviewcommunity.github.io/CW2022-miniworkshop/slides.html) automatically, each time new commits are added to the `main` branch.

To build the slides locally, you'll need
[cmake](https://cmake.org/download/) (3.17+) and
[pandoc](https://pandoc.org/installing.html) (2.10+). In the repo's
root directory:

```
mkdir build && cd build
cmake ../slides
make install
```
