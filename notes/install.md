# Installation

Experimenting with <https://github.com/dtkaplan/checkr>.

In particular, I wanted to view the Vignettes for this package.  I was looking
at <http://r-pkgs.had.co.nz/vignettes.html>.

## Installing `checkr`

Unfortunately there is another, unrelated package called `checkr`, that you
get from `install.packages('checkr').  So don't do that (I did, and had to
`remove.package('checkr')`.

Installation instructions have:

```
devtools::install_github("lionel-/redpen")
devtools::install_github("dtkaplan/checkr")
```

Installation of `devtools` was not smooth, on my Mac - I got this error:


```
   The libgit2 library that is required to build git2r was not found.

   Please install:
     libgit2-dev   (package on e.g. Debian and Ubuntu)
     libgit2-devel (package on e.g. Fedora, CentOS and RHEL)
     libgit2       (Homebrew package on macOS)
   and try again.

   If the libgit2 library is installed on your system but the git2r configuration is
   unable to find it, you can specify the include and lib path to libgit2 with:
   R CMD INSTALL git2r --configure-vars='INCLUDE_DIR=path/to/include LIB_DIR=path/to/lib'
```


I did that, and:

```
install.packages('usethis')
library('devtools')
```

after which the install lines above worked without error.

## Running the Vignette

I open the file `vignettes/checkr.Rmd` in RStudio, and run "Knit" from the
menus.  I found I needed the `mosaic` package (from the head of that file).
After installing that, I got the checkr vignette open in an RStudio window.

