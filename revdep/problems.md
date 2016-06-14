# Setup

## Platform

|setting  |value                        |
|:--------|:----------------------------|
|version  |R version 3.3.0 (2016-05-03) |
|system   |x86_64, darwin13.4.0         |
|ui       |X11                          |
|language |(EN)                         |
|collate  |en_US.UTF-8                  |
|tz       |America/Chicago              |
|date     |2016-06-10                   |

## Packages

|package   |*  |version    |date       |source                       |
|:---------|:--|:----------|:----------|:----------------------------|
|covr      |   |2.0.1      |2016-04-06 |CRAN (R 3.3.0)               |
|dplyr     |   |0.4.3      |2015-09-01 |cran (@0.4.3)                |
|gapminder |   |0.2.0      |2015-12-31 |CRAN (R 3.3.0)               |
|knitr     |   |1.13       |2016-05-09 |CRAN (R 3.3.0)               |
|lazyeval  |   |0.1.10     |2015-01-02 |cran (@0.1.10)               |
|magrittr  |   |1.5        |2014-11-22 |CRAN (R 3.3.0)               |
|Rcpp      |   |0.12.5     |2016-05-14 |CRAN (R 3.3.0)               |
|rmarkdown |   |0.9.6      |2016-05-01 |CRAN (R 3.3.0)               |
|stringi   |   |1.1.1      |2016-05-27 |cran (@1.1.1)                |
|testthat  |*  |1.0.2.9000 |2016-06-10 |github (hadley/testthat)     |
|tibble    |   |1.0-5      |2016-06-10 |github (hadley/tibble)       |
|tidyr     |   |0.4.1.9000 |2016-06-10 |local (hadley/tidyr@925b0bf) |

# Check results
13 packages with problems

## broom (0.4.0)
Maintainer: David Robinson <admiral.david@gmail.com>  
Bug reports: http://github.com/dgrtwo/broom/issues

2 errors | 0 warnings | 0 notes

```
checking examples ... ERROR
Running examples in ‘broom-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: survfit_tidiers
> ### Title: tidy survival curve fits
> ### Aliases: glance.survfit survfit_tidiers tidy.survfit
> 
> ### ** Examples
... 48 lines ...

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union

Error: Unknown column 'median'
Execution halted

checking tests ... ERROR
Running the tests in ‘tests/test-all.R’ failed.
Last 13 lines of output:
  3: as.expectation(exp, ..., srcref = srcref) at /private/tmp/RtmpLh7b3s/devtools7fec710673af/hadley-testthat-d3e20b9/R/expectation.R:33
  4: identical(as.vector(object), TRUE) at /private/tmp/RtmpLh7b3s/devtools7fec710673af/hadley-testthat-d3e20b9/R/expectation.R:112
  5: as.vector(object)
  6: augmented$disp
  7: `$.tbl_df`(augmented, disp)
  8: stop("Unknown column '", i, "'", call. = FALSE) at /private/tmp/RtmpLh7b3s/devtools7fec5d3614e4/hadley-tibble-64175a8/R/tbl-df.r:47
  
  testthat results ================================================================
  OK: 490 SKIPPED: 0 FAILED: 1
  1. Error: rowwise tidiers can be applied to sub-models (@test-rowwise.R#21) 
  
  Error: testthat unit tests failed
  Execution halted
```

## ezsummary (0.1.9)
Maintainer: Hao Zhu <haozhu@hsl.harvard.edu>

1 error  | 0 warnings | 0 notes

```
checking tests ... ERROR
Running the tests in ‘tests/testthat.R’ failed.
Last 13 lines of output:
  ezsummary_quantitative(df, n = T) not equivalent to `expected_data_frame_N`.
  Different types: x tbl_df, tbl, data.frame, y data.frame
  
  
  testthat results ================================================================
  OK: 47 SKIPPED: 0 FAILED: 4
  1. Failure: ezsummary_categorical can work without grouping data (@test-ezsummary_categorical.R#11) 
  2. Failure: ezsummary_categorical can work without grouping data (@test-ezsummary_categorical.R#12) 
  3. Failure: ezsummary_quantitative can work correctly with 1 variable and no grouping data (@test-ezsummary_quantitative.R#13) 
  4. Failure: ezsummary_quantitative can work correctly with 1 variable and no grouping data (@test-ezsummary_quantitative.R#14) 
  
  Error: testthat unit tests failed
  Execution halted
```

## ggmcmc (1.0)
Maintainer: Xavier Fernández i Marín <xavier.fim@gmail.com>  
Bug reports: https://github.com/xfim/ggmcmc/issues

1 error  | 0 warnings | 0 notes

```
checking examples ... ERROR
Running examples in ‘ggmcmc-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: ggs_caterpillar
> ### Title: Caterpillar plot with thick and thin CI
> ### Aliases: ggs_caterpillar
> 
> ### ** Examples
> 
> data(linear)
> ggs_caterpillar(ggs(s))
> ggs_caterpillar(list(A=ggs(s), B=ggs(s))) # silly example duplicating the same model
Error: Unknown column 'description'
Execution halted
```

## ggRandomForests (1.2.1)
Maintainer: John Ehrlinger <john.ehrlinger@gmail.com>  
Bug reports: https://github.com/ehrlinger/ggRandomForests/issues

2 errors | 0 warnings | 1 note 

```
checking examples ... ERROR
Running examples in ‘ggRandomForests-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: gg_rfsrc.rfsrc
> ### Title: Predicted response data object
> ### Aliases: gg_rfsrc gg_rfsrc.rfsrc
> 
> ### ** Examples
... 19 lines ...
> ##D gg_dta<- gg_rfsrc(rfsrc_airq)
> ##D 
> ##D plot(gg_dta)
> ## End(Not run)
> 
> ## -------- Boston data
> data(rfsrc_Boston, package="ggRandomForests")
> plot(rfsrc_Boston) 
Error in if (x$tree.err == FALSE) { : argument is of length zero
Calls: plot -> plot.rfsrc
Execution halted

checking tests ... ERROR
Running the tests in ‘tests/test-all.R’ failed.
Last 13 lines of output:
  6: sort(randomForestSRC::vimp(object)$importance, decreasing = TRUE)
  7: randomForestSRC::vimp(object)
  8: generic.predict.rfsrc(object, outcome.target = outcome.target, importance = importance, 
         importance.xvar = xvar.names, seed = seed, do.trace = do.trace, membership = FALSE, 
         subset = subset, ...)
  9: stop()
  
  testthat results ================================================================
  OK: 412 SKIPPED: 0 FAILED: 1
  1. Error: gg_vimp survival (@test_gg_vimp.R#139) 
  
  Error: testthat unit tests failed
  Execution halted

checking installed package size ... NOTE
  installed size is  5.9Mb
  sub-directories of 1Mb or more:
    data   2.6Mb
    doc    3.0Mb
```

## glycanr (0.3.0)
Maintainer: Ivo Ugrina <ivo@iugrina.com>  
Bug reports: https://github.com/iugrina/glycanr/issues

2 errors | 0 warnings | 1 note 

```
checking examples ... ERROR
Running examples in ‘glycanr-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: quantilenorm
> ### Title: Quantile Normalization of glycan data
> ### Aliases: quantilenorm
> 
> ### ** Examples
> 
> data(mpiu)
> mpiun <- quantilenorm(mpiu)
Error in quantilenorm(mpiu) : 
  Unable to proceed since package preprocessCore from
        BioConductor is not available on this system. This
        package is a prerequisite to use the quantilenorm function!
Execution halted

checking tests ... ERROR
Running the tests in ‘tests/testthat.R’ failed.
Last 13 lines of output:
  
  The following objects are masked from 'package:base':
  
      intersect, setdiff, setequal, union
  
  Error in quantilenorm(mpiu, transpose = TRUE) : 
    Unable to proceed since package preprocessCore from
          BioConductor is not available on this system. This
          package is a prerequisite to use the quantilenorm function!
  Calls: test_check ... force -> source_file -> eval -> eval -> quantilenorm
  testthat results ================================================================
  OK: 5 SKIPPED: 0 FAILED: 0
  Execution halted

checking package dependencies ... NOTE
Package suggested but not available for checking: ‘preprocessCore’
```

## heemod (0.3.1)
Maintainer: Antoine Filipovic-Pierucci <pierucci@gmail.com>  
Bug reports: https://github.com/pierucci/heemod/issues

1 error  | 1 warning  | 0 notes

```
checking tests ... ERROR
Running the tests in ‘tests/testthat.R’ failed.
Last 13 lines of output:
  12: compute_icer(normalize_ce(object))
  13: `*tmp*`$.icer
  14: `$.tbl_df`(`*tmp*`, .icer)
  15: stop("Unknown column '", i, "'", call. = FALSE) at /private/tmp/RtmpLh7b3s/devtools7fec5d3614e4/hadley-tibble-64175a8/R/tbl-df.r:47
  
  testthat results ================================================================
  OK: 101 SKIPPED: 0 FAILED: 3
  1. Error: Model evaluation, 2 models (@test_model.R#211) 
  2. Error: run_models behaves as expected (@test_run_model.R#150) 
  3. Error: Discounting (@test_run_model.R#265) 
  
  Error: testthat unit tests failed
  Execution halted

checking re-building of vignette outputs ... WARNING
Error in re-building vignettes:
  ...
Quitting from lines 214-215 (homogeneous.Rmd) 
Error: processing vignette 'homogeneous.Rmd' failed with diagnostics:
Unknown column '.icer'
Execution halted

```

## pixiedust (0.7.0)
Maintainer: Benjamin Nutter <nutter@battelle.org>  
Bug reports: https://github.com/nutterb/pixiedust/issues

0 errors | 1 warning  | 0 notes

```
checking re-building of vignette outputs ... WARNING
Error in re-building vignettes:
  ...
Quitting from lines 173-185 (advancedMagic.Rmd) 
Error: processing vignette 'advancedMagic.Rmd' failed with diagnostics:
Unknown column 'html_row_pos'
Execution halted

```

## pmc (1.0.1)
Maintainer: Carl Boettiger <cboettig@gmail.com>  
Bug reports: https://github.com/cboettig/pmc/issues

1 error  | 0 warnings | 0 notes

```
checking tests ... ERROR
Running the tests in ‘tests/testthat.R’ failed.
Last 13 lines of output:
  > library("testthat")
  > library("pmc")
  > 
  > test_check("pmc")
  Loading required package: ape
  
  Warning message:
  In treedata(geo$phy, geo$dat) :
    The following tips were not found in 'data' and were dropped from 'phy':
  	olivacea
  testthat results ================================================================
  OK: 6 SKIPPED: 0 FAILED: 0
  Execution halted
```

## quickpsy (0.1.2)
Maintainer: Linares Daniel <danilinares@gmail.com>

1 error  | 0 warnings | 0 notes

```
checking examples ... ERROR
Running examples in ‘quickpsy-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: logliks
> ### Title: Calculates the loglikelihoods
> ### Aliases: logliks
> 
> ### ** Examples
> 
> library(MPDiR) # contains the Vernier data
> fit <- quickpsy(Vernier, Phaseshift, NumUpward, N,
+                 grouping = .(Direction, WaveForm, TempFreq), B = 20)
Estimating parameters...
Error: Unknown column 'y'
Execution halted
```

## R6Frame (0.1.0)
Maintainer: Kristian D. Olsen <kristian@doingit.no>

1 error  | 0 warnings | 0 notes

```
checking tests ... ERROR
Running the tests in ‘tests/testthat.R’ failed.
Last 13 lines of output:
  > 
  > test_check("R6Frame")
  1. Failure: spread works with R6 tbl_df (@test-tidyr_reshape.R#86) -------------
  tbl$data not equal to `org`.
  Different types: x tbl_df, tbl, data.frame, y data.frame
  
  
  testthat results ================================================================
  OK: 163 SKIPPED: 0 FAILED: 1
  1. Failure: spread works with R6 tbl_df (@test-tidyr_reshape.R#86) 
  
  Error: testthat unit tests failed
  Execution halted
```

## rgho (0.0.1)
Maintainer: Antoine Filipovic-Pierucci <pierucci@gmail.com>  
Bug reports: https://github.com/pierucci/rgho/issues

1 error  | 1 warning  | 0 notes

```
checking examples ... ERROR
Running examples in ‘rgho-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: search_gho
> ### Title: Search Codes or Dimensions Labels
> ### Aliases: search_codes search_dimensions search_gho
> 
> ### ** Examples
... 27 lines ...
DEFINITION_XML
DISPLAY_ES
DISPLAY_FR
IMR_ID
RENDERER_ID
> 
> result <- get_gho_codes(dimension = "REGION")
Error in enc2utf8(col_names(col_labels, sep = sep)) : 
  argumemt is not a character vector
Calls: get_gho_codes ... spread_.tbl_df -> as_data_frame -> NextMethod -> spread_.data.frame
Execution halted

checking re-building of vignette outputs ... WARNING
Error in re-building vignettes:
  ...
Quitting from lines 52-54 (intro.Rmd) 
Error: processing vignette 'intro.Rmd' failed with diagnostics:
argumemt is not a character vector
Execution halted

```

## RNeXML (2.0.6)
Maintainer: Carl Boettiger <cboettig@gmail.com>  
Bug reports: https://github.com/ropensci/RNeXML/issues

2 errors | 1 warning  | 1 note 

```
checking examples ... ERROR
Running examples in ‘RNeXML-Ex.R’ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: add_basic_meta
> ### Title: Add basic metadata
> ### Aliases: add_basic_meta
> 
> ### ** Examples
> 
> nex <- add_basic_meta(title = "My test title",
+              description = "A description of my test",
+              creator = "Carl Boettiger <cboettig@gmail.com>",
+              publisher = "unpublished data",
+              pubdate = "2012-04-01")
Error: Unknown column 'content'
Execution halted

checking tests ... ERROR
Running the tests in ‘tests/test-all.R’ failed.
Last 13 lines of output:
  1.  Error: We can serialize the various versions of the ape format (@test_ape.R#40) 
  2.  Error: We can read and write NeXML to phylo and back without edge.lengths (@test_ape.R#52) 
  3.  Error: Rooted trees remain rooted on conversions (@test_ape.R#65) 
  4.  Error: Unrooted trees remain unrooted on conversions (@test_ape.R#74) 
  5.  Error: we can add characters to a nexml file using a data.frame (@test_characters.R#92) 
  6.  Error: We can serialize tree and trait data for a comparative analysis (@test_comp_analysis.R#25) 
  7.  Error: We can generate valid EML with uuid ids on all elements (@test_global_ids.R#11) 
  8.  Error: We can add additional metadata (@test_meta.R#8) 
  9.  Error: We can add R bibentry type metadata (@test_meta.R#28) 
  10. Error: We can add additional metadata (@test_meta.R#42) 
  
  Error: testthat unit tests failed
  Execution halted

checking re-building of vignette outputs ... WARNING
Error in re-building vignettes:
  ...
Loading required package: ape
Quitting from lines 46-67 (metadata.Rmd) 
Error: processing vignette 'metadata.Rmd' failed with diagnostics:
Unknown column 'content'
Execution halted


checking package dependencies ... NOTE
Packages suggested but not available for checking: ‘rrdf’ ‘Sxslt’
```

## tigger (0.2.5)
Maintainer: Daniel Gadala-Maria <daniel.gadala-maria@yale.edu>  
Bug reports: https://bitbucket.org/kleinstein/tigger/issues

0 errors | 1 warning  | 0 notes

```
checking re-building of vignette outputs ... WARNING
Error in re-building vignettes:
  ...
Loading required package: alakazam
Loading required package: ggplot2
Loading required package: shazam

Attaching package: 'dplyr'

The following objects are masked from 'package:stats':

    filter, lag

The following objects are masked from 'package:base':

    intersect, setdiff, setequal, union

Quitting from lines 110-115 (Tigger-Vignette.Rmd) 
Error: processing vignette 'Tigger-Vignette.Rmd' failed with diagnostics:
there is no package called 'snow'
Execution halted

```

