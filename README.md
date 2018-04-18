# Gitbook python scripts

A few python scripts for generating Gitbook content from existing books hosted on GitHub.

[generateChapters.py](generateChapters.py) downloads markdown files and any images they use into the local repo based on a new book structure specified in a CSV. It also builds the SUMMARY.md file automatically from the CSV.

[slideGeneration.py](SlideGeneration.py) is a work-in-progress script that generates slides from Gitbook markdown. It currently just merges all markdown into one file and moves images into one directory. I've been using [pandoc](https://pandoc.org/) to [generate the slides](https://pandoc.org/MANUAL.html#producing-slide-shows-with-pandoc) after that, but haven't written that into the script yet.
