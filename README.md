# PREVTEST19

Tests & utilities for exercising the compiler @ the compiler course at FRI, year 2018/2019.

_Initial version provided by [MatevzFa](https://github.com/MatevzFa/prevtest/)_

# Disclaimer
**Nobody** guarantees that any of the test programs or their output XMLs provided with the test suite are correct. \
Also note that the PREV language specification has changed over the years and so some older tests might not be compliant with the current language.

So, do your work in the prescribed order:

1. engage brain
2. check your results and 
3. If you get errors and you believe that there might be an issue with the tests, report it on the issue tracker [here](https://github.com/RokKos/prevtest/issues).
4. Any other issues pertaining the compiler itself, such as:
     - additional instructions regarding the work
     - ambiguities in the language specification
     - issues with the code template (this has happened in the past, so don't be surprised)
 
    should be reported on the [course forum](https://ucilnica.fri.uni-lj.si/mod/forum/view.php?id=27690) instead - this way you'll have a higher chance that somebody will actually answer it & also more people will benefit from that answer.

# Installation
If you want it to work out of the box, clone this repository into a folder next to your `prev` folder.
```
...
├── prev
└── prevtest
```

You can also clone it somewhere else and provide the path to your compiler source using the `--compiler` argument.

# Usage

```
usage: prevtest.py [-h] [--update-tests] [--verbose] [--no-build]
                   PHASE [FILTER]

positional arguments:
  PHASE           Target phase
  FILTER          Filter for test cases

optional arguments:
  -h, --help      show this help message and exit
  --update-tests  Update tests for some phase
  --verbose       Verbose output
  --no-build      Don't rebuild the compiler
```

# License & Contribution
This software was made by the students of the compiler course in good faith that one might be able to decently test the compiler & see it blow up before the final examination. Nobody holds any particular copyright to the sources and neither should you.

Consider it as beerware.

If you want your tests added to this repository, make a pull request with your tests in an appropriate folder (see current structure).

Feel free to change (or completely rewrite :sweat_smile: ) the [program](prevtest.py).
