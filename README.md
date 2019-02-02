# Commons

A technical biomedical informatics and computational biology
[knowledge commons][commons] for graduate students and postdocs.

[commons]: https://en.wikipedia.org/wiki/Knowledge_commons

## Project Structure

This project is encapsulated in a `bookdown` document.

There are three key directories:

- `docs/` = where the compiled book belongs; don't edit this manually
- `chapters/` = high level chapters or topics; edit this file to add new
  sub-topics
- `content/` = place to add content; all content can live here, while the files
  in the `chapters/` directory calls from this one place

**Chapters**

The files in `chapters` will determine the order and contents of the Commons.

Each new chapter (i.e, topic) needs to be prefixed with a number, indicating
its order in the Commons. This name should also be
[snake case](https://en.wikipedia.org/wiki/Snake_case) (e.g.
`01_supervised_learning.Rmd`).

From within a chapter, to refer to new sub-topics added to the `content/`
directory, create a code block and refer to the indended file using the `child`
parameter. For example: `{r child="content/shinkage_methods.Rmd"}` (see
https://community.rstudio.com/t/14412/4).
