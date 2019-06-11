explore-packages.R
================
karsm933
2019-06-11

``` r
library(tidyverse)
```

    ## Registered S3 methods overwritten by 'ggplot2':
    ##   method         from 
    ##   [.quosures     rlang
    ##   c.quosures     rlang
    ##   print.quosures rlang

    ## ── Attaching packages ───────────────────────────────────────── tidyverse 1.2.1 ──

    ## ✔ ggplot2 3.1.1     ✔ purrr   0.3.2
    ## ✔ tibble  2.1.2     ✔ dplyr   0.8.1
    ## ✔ tidyr   0.8.3     ✔ stringr 1.4.0
    ## ✔ readr   1.3.1     ✔ forcats 0.4.0

    ## ── Conflicts ──────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

``` r
.libPaths()
```

    ## [1] "/Library/Frameworks/R.framework/Versions/3.6/Resources/library"

``` r
ipt <- installed.packages() %>% 
  as_tibble() %>%
  select(Package, LibPath, Version, Priority, Built) 
ipt
```

    ## # A tibble: 193 x 5
    ##    Package     LibPath                               Version Priority Built
    ##    <chr>       <chr>                                 <chr>   <chr>    <chr>
    ##  1 Annotation… /Library/Frameworks/R.framework/Vers… 1.46.0  <NA>     3.6.0
    ##  2 arules      /Library/Frameworks/R.framework/Vers… 1.6-3   <NA>     3.6.0
    ##  3 askpass     /Library/Frameworks/R.framework/Vers… 1.1     <NA>     3.6.0
    ##  4 assertthat  /Library/Frameworks/R.framework/Vers… 0.2.1   <NA>     3.6.0
    ##  5 backports   /Library/Frameworks/R.framework/Vers… 1.1.4   <NA>     3.6.0
    ##  6 base        /Library/Frameworks/R.framework/Vers… 3.6.0   base     3.6.0
    ##  7 base64enc   /Library/Frameworks/R.framework/Vers… 0.1-3   <NA>     3.6.0
    ##  8 BH          /Library/Frameworks/R.framework/Vers… 1.69.0… <NA>     3.6.0
    ##  9 Biobase     /Library/Frameworks/R.framework/Vers… 2.44.0  <NA>     3.6.0
    ## 10 BiocGeneri… /Library/Frameworks/R.framework/Vers… 0.30.0  <NA>     3.6.0
    ## # … with 183 more rows
