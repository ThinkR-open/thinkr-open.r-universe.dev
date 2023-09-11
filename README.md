
# Packages for the ThinkR Universe 

This repo host the `package.json` configuration file used to build the [ThinkR r-universe](//thinkr-open.r-universe.dev/).

## Adding a new package

Make a PR to append an entry to the `package.json` file, such as:

``` json
    {
        "package": "<my-package-name>",
        "url": "https://github.com/<my-package-github-url>"
    }
```

## Installing a package from the ThinkR r-universe

A one-shot example using {golem}:

``` r
install.packages("golem", repos = "https://thinkr-open.r-universe.dev" )

```
Alternatively you can configure your `repos` R option as such:

``` r
options(
    repos = c(
        thinkropen = "https://thinkr-open.r-universe.dev",
        CRAN = "https://cloud.r-project.org"
        )
  )
install.packages("golem")
```
