# usethis_demos
tutorials and examples for usethis functions

[How to edit a pull request locally, part 1](https://github.com/jtr13/usethis_demos/blob/master/how_to1.md)

[How to edit a pull request locally, part 2](https://github.com/jtr13/usethis_demos/blob/master/how_to2.md)


Notes on rendering `.Rmd` files for contributors:

1. Update `usethis`.

2. Knit `how_to1.Rmd` (any uncommitted files will be committed during render.)

3. `git2r::stash()`

4. Switch to `master` branch

5. `git2r::stash_pop()`  (`how_to1.md` should appear)

6. Knit `how_to2.Rmd` (any uncommitted files will be committed during render.)

