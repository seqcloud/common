# basejump

[![Repo status: active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![Travis CI build status](https://travis-ci.com/acidgenomics/basejump.svg?branch=master)](https://travis-ci.com/acidgenomics/basejump)
[![AppVeyor CI build status](https://ci.appveyor.com/api/projects/status/007vq15089ukn6ej/branch/master?svg=true)](https://ci.appveyor.com/project/mjsteinbaugh/basejump/branch/master)
[![Anaconda version](https://anaconda.org/bioconda/r-basejump/badges/version.svg) ![Anaconda latest release date](https://anaconda.org/bioconda/r-basejump/badges/latest_release_date.svg) ![Anaconda downloads](https://anaconda.org/bioconda/r-basejump/badges/downloads.svg)](https://anaconda.org/bioconda/r-basejump)

Base functions for bioinformatics and [R][] package development.

## Installation

### [R][] method

```r
if (!requireNamespace("remotes", quietly = TRUE)) {
    install.packages("remotes")
}
Sys.setenv(R_REMOTES_UPGRADE = "always")
# Set `GITHUB_PAT` in `~/.Renviron` if you get a rate limit error.
remotes::install_github("acidgenomics/basejump")
```

Here's how to update to the latest version on GitHub:

```r
Sys.setenv(R_REMOTES_UPGRADE = "always")
remotes::update_packages()
```

Always check that your Bioconductor installation is valid before proceeding.

```r
if (!requireNamespace("BiocManager", quietly = TRUE)) {
    install.packages("BiocManager")
}
BiocManager::valid()
```

### [conda][] method

Configure [conda][] to use the [bioconda][] channels.

```bash
conda install -c bioconda r-basejump
```

## References

The papers and software cited in our workflows are available as a [shared library](https://paperpile.com/shared/agxufd) on [Paperpile][].

[biocmanager]: https://cran.r-project.org/package=BiocManager
[bioconda]: https://bioconda.github.io/
[bioconductor]: https://bioconductor.org/
[conda]: https://conda.io/
[paperpile]: https://paperpile.com/
[r]: https://www.r-project.org/
