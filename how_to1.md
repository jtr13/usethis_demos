How to edit a pull request locally, part 1
================
Joyce Robbins
4/1/2019

#### Context

This is a demo of using **usethis** functions to modify a pull request
locally. Without these functions, the process is *much more complicated
and error prone*. Note that the preferred workflow is to ask the person
who submitted the changes to make the modifications that you request.
You would only do this editing yourself, following the steps below, in a
situation in which the contributor is not responding, or does not have
the skills to make the changes you need. It will only work (need to test
this) if the contributor has checked the “Allow edits from maintainers.”
box in their pull request.

#### Install **usethis**

Use the dev
    version:

``` r
devtools::install_github("r-lib/usethis")
```

    ## Skipping install of 'usethis' from a github remote, the SHA1 (169b556e) has not changed since last install.
    ##   Use `force = TRUE` to force installation

#### Open local version of repo

Open the local project for the repo and pull changes, either by clicking
on the PULL button in RStudio or as follows:

``` r
git2r::pull()
```

    ## Already up-to-date

#### Find and fetch the pull request

Look for the pull request number in the [list of pull
requests](https://github.com/jtr13/usethis_demos/pulls). We see that the
[pull request we want](https://github.com/jtr13/springishere/pull/1) is
number 1.

``` r
usethis::pr_fetch(1)
```

    ## ✔ Setting active project to '/Users/JoyceRobbins/usethis_demos'
    ## ✔ Checking out PR 'jtr13/usethis_demos/#1' (@nbrgraphs): 'Add line'
    ## ✔ Adding remote 'nbrgraphs' as 'https://github.com/nbrgraphs/usethis_demos.git'
    ## ✔ Creating local branch 'nbrgraphs-patch-1'
    ## ✔ Setting upstream tracking branch for 'nbrgraphs-patch-1' to 'nbrgraphs/patch-1'
    ## ✔ Switching to branch 'nbrgraphs-patch-1'
