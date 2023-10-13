# Feature-Model Histories

## Contents

This repository containts the evolution history of multiple software product lines, namely

* BusyBox (adapted from [github.com/skrieter/evaluation-mig](http://github.com/skrieter/evaluation-mig))
    * 3,714 models (247 unique)
* FinancialServices01 (adapted from [github.com/skrieter/evaluation-mig](http://github.com/skrieter/evaluation-mig))
    * 10 models (10 unique)
* Fiasco (adapted from [github.com/tubs-isf/fiasco-case-study](http://github.com/tubs-isf/fiasco-case-study))
    * 33 models (31 unique)
* Soletta (adapted from [github.com/tubs-isf/soletta-case-study](http://github.com/tubs-isf/soletta-case-study))
    * 210 models (149 unique)
* Toybox (adapted from [github.com/tubs-isf/toybox-case-study](http://github.com/tubs-isf/toybox-case-study))
    * 80 models (37 unique)
* Uclibc (adapted from [github.com/tubs-isf/uclibc-case-study](http://github.com/tubs-isf/uclibc-case-study))
    * 178 models (137 unique)

*unique*: If two DIMACS files have the same file hash (md5) after preprocessing, only the first one is kept

Each of the repositories contains the following sub directories:

* `./featureide`: The models in the [FeatureIDE](github.io/featureide) XML format
* `./dimacs`: The models in DIMACS format, as produced by FeatureIDE
* `./dimacs_unique`: The models in DIMACS format, which remain the distinct after preprocessing
* `./dimacs_cleaned`: The models from `dimacs_unique` after preprocessing
    * Dead/Core analysis, afterwards dead/core features are substituted in clauses
    * Variable Supersetting, features with the same name have the same ID in all DIMACS files

----

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.