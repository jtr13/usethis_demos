# usethis_demos
tutorials and examples for usethis functions

[How to edit a pull request locally, part 1](https://github.com/jtr13/usethis_demos/blob/master/how_to1.md)

[How to edit a pull request locally, part 2](https://github.com/jtr13/usethis_demos/blob/master/how_to2.md)


Notes on rendering `.Rmd` files for contributors:

1. Update `usethis`.

1. Knit `how_to1.Rmd` (any uncommitted files will be committed during render.)

1. Make a change, save and commit.  Leave `how_to1.md` as is.

1. `git2r::stash()`

1. Switch to `master` branch

1. `git2r::stash_pop()`  (`how_to1.md` should appear)

1. Knit `how_to2.Rmd` (any uncommitted files will be committed during render.)

1. Commit, push changes.
