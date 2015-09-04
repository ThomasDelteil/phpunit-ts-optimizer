# phpunit-ts-optimizer
Python Command line tool to split one test suite in N suites in a semi-optimal manner based on --log-json output of phpunit

usage: tsg [-h] [-l LOGFILE] [-q] [-s] [-v] [-j SOURCE] [-t TEMPLATE]
           [-i INITIALTESTSUITENAME] [-a GENERATED] [-r RELATIVEPATH]
           [-n SUITESNUMBER] [-o OUTPUT]

optional arguments:
  -h, --help            show this help message and exit
  -l LOGFILE, --logfile LOGFILE
                        log to file (default: log to stdout)
  -q, --quiet           decrease the verbosity
  -s, --silent          only log warnings
  -v, --verbose         raise the verbosity
  -j SOURCE, --sourceJson SOURCE
                        PHPUnit --log-json output
  -t TEMPLATE, --sourceConfig TEMPLATE
                        PHPUnit .xml config file to use as template, it should
                        contain at least one test suite
  -i INITIALTESTSUITENAME, --initialTestSuiteName INITIALTESTSUITENAME
                        Initial test suite Name (to add the excluded file path
                        to, allowing for subsequent tests to be added)
  -a GENERATED, --generatedSuiteSuffix GENERATED
                        Prefix for the generated test suites
  -r RELATIVEPATH, --testRelativePath RELATIVEPATH
                        Relative Path from your config file to your test
                        folder, build/config.xml and tests/ requires ../tests
  -n SUITESNUMBER, --suitesNumber SUITESNUMBER
                        Number of suites to create
  -o OUTPUT, --output OUTPUT
                        Output file
