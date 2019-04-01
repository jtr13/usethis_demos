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

Use the dev version:

``` r
devtools::install_github("r-lib/usethis")
```

    ## Downloading GitHub repo r-lib/usethis@master

    ## 
    ##   
       checking for file ‘/private/var/folders/my/fzt1bvgd74q24_wx05mw05_c0000gn/T/Rtmpib8UV1/remotes111505d5caa89/r-lib-usethis-169b556/DESCRIPTION’ ...
      
    ✔  checking for file ‘/private/var/folders/my/fzt1bvgd74q24_wx05mw05_c0000gn/T/Rtmpib8UV1/remotes111505d5caa89/r-lib-usethis-169b556/DESCRIPTION’ (454ms)
    ## 
      
    ─  preparing ‘usethis’: (336ms)
    ## 
      
       checking DESCRIPTION meta-information ...
      
    ✔  checking DESCRIPTION meta-information
    ## 
      
    ─  checking for LF line-endings in source and make files and shell scripts
    ## 
      
    ─  checking for empty or unneeded directories
    ## 
      
       Removed empty directory ‘usethis/vignettes’
    ## 
      
    ─  building ‘usethis_1.4.0.9000.tar.gz’
    ## 
      
       
    ## 

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
