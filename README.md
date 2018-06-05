# Gitbook python scripts

A few python scripts for generating Gitbook content from existing books hosted on GitHub.

[generateChapters.py](generateChapters.py) downloads markdown files and any images they use into the local repo based on a new book
structure specified in chapters.csv. It also builds the SUMMARY.md file automatically from the CSV.
[ ] make functions out of everything
[ ] define variable names from CSV instead of using row[n]
[ ] add support for UNIX file paths
[ ] add support for multiple repos or branches
[ ] clean up or simplify CSV columns
[ ] automate section numbering
[ ] add error handling

[edits.py](edits.py) makes edits to markdown files based on edits outlined in edits.json. Edits can insert (add a new line) or replace (no new line) an include from ./includes/, or delete lines.

[slideGeneration.py](SlideGeneration.py) is a work-in-progress script that generates slides from Gitbook markdown. It currently just merges all markdown into one file and moves images into one directory. I've been using [pandoc](https://pandoc.org/) to [generate the slides](https://pandoc.org/MANUAL.html#producing-slide-shows-with-pandoc) after that, but haven't written that into the script yet.
[ ] use `subprocess` to automate running `pandoc`
[ ] add error handling
