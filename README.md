# usethis_demos
tutorials and examples for usethis functions

[How to edit a pull request locally, part 1](https://github.com/jtr13/usethis_demos/blob/master/how_to1.md)

[How to edit a pull request locally, part 2](https://github.com/jtr13/usethis_demos/blob/master/how_to2.md)


Notes for contributors on rendering `.Rmd` files:

1. Update `usethis`.

1. Knit `how_to1.Rmd` with `rmarkdown::render("how_to1.Rmd", "github_document")`

(any uncommitted files will be committed during render)

1. Make a change, save and commit.  Do NOT save and commit `how_to1.md`.

1. `git2r::stash()`

1. Switch to `master` branch

1. `git2r::stash_pop()`  (`how_to1.md` should appear)

1. Knit `how_to2.Rmd` by clicking Knit button (any uncommitted files will be committed during render)

1. Commit, push changes.
