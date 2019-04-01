How to edit a pull request locally, part 2
================
Joyce Robbins
4/1/2019

#### Push changes

Now that we’ve completed making edits to the PR, and have saved and
committed them, we will push them to GitHub:

``` r
usethis::pr_push()
```

    ## ✔ Setting active project to '/Users/JoyceRobbins/usethis_demos'
    ## ✔ Checking that local branch 'nbrgraphs-patch-1' has the changes in 'nbrgraphs/patch-1'
    ## ✔ Pushing local 'nbrgraphs-patch-1' branch to 'nbrgraphs:patch-1'
    ## ✔ View PR at 'https://github.com/jtr13/usethis_demos/pull/1'

We’ll wrap with `pr_finish()`. (I’m terse here since **usethis**
functions speak for themselves…)

``` r
usethis::pr_finish()
```

    ## ✔ Switching back to 'master' branch
    ## ✔ Pulling changes from GitHub source repo 'origin/master'
    ## ✔ Deleting local 'nbrgraphs-patch-1' branch

Finally, if desired, you can delete the remote that was created:

``` r
git2r::remotes()
```

    ## [1] "nbrgraphs" "origin"

``` r
git2r::remote_remove(name = "nbrgraphs")
git2r::remotes()
```

    ## [1] "origin"

And we are done\! Our edits have been [added as a commit to the pull
request](https://github.com/jtr13/usethis_demos/pull/1). We can leave
the pull request open for additional edits / reviews or go to GitHub and
merge it.
