## Test environments

* OS X install: R 3.5
* win-builder: R-devel
* travis-ci: R 3.1, R 3.2, R 3.3, R 3.4, R-devel

## R CMD check results

0 errors | 0 warnings | 0 notes

## revdepcheck results

We checked 653 reverse dependencies (581 from CRAN + 72 from BioConductor), comparing R CMD check results across CRAN and dev versions of this package.

 * We saw 8 new problems
 * We failed to check 14 packages

Issues with CRAN packages are summarised below.

### New problems
(This reports the first line of each new failure)

* cutpointr
  checking examples ... ERROR
  checking tests ...
  checking re-building of vignette outputs ... WARNING

* echarts4r
  checking installed package size ... NOTE
  Seems unrelated to tidyr.

* healthcareai
  checking examples ... ERROR
  checking tests ...

* postal
  checking tests ...

* recipes
  checking examples ... ERROR
  checking tests ...
  checking re-building of vignette outputs ... WARNING

* tidyquant
  checking tests ...

* unpivotr
  checking tests ...

* widyr
  checking tests ...

### Failed to check

* anomalyDetection (failed to install)
* circumplex       (failed to install)
* colorednoise     (failed to install)
* dynfrail         (failed to install)
* easyformatr      (failed to install)
* HTSSIP           (check timed out)
* morse            (failed to install)
* phenofit         (failed to install)
* pmc              (check timed out)
* qdap             (failed to install)
* SCORPIUS         (failed to install)
* sf               (failed to install)
* vlad             (failed to install)
* wand             (failed to install)
