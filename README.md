# phpunit-ts-optimizer
Python Command line tool to split one test suite in N suites in a semi-optimal manner based on --log-json output of phpunit

```
usage: tsg [-h] [-l LOGFILE] [-q] [-s] [-v] [-j SOURCE] [-t TEMPLATE]
           [-a GENERATED] [-n SUITESNUMBER] [-o OUTPUT]

optional arguments:
  -h, --help            show this help message and exit
  -l LOGFILE, --logfile LOGFILE
                        log to file (default: log to stdout)
  -q, --quiet           decrease the verbosity
  -s, --silent          only log warnings
  -v, --verbose         raise the verbosity
  -j SOURCE, --sourceJunit SOURCE
                        PHPUnit JUNIT source
  -t TEMPLATE, --sourceConfig TEMPLATE
                        PHPUnit .xml config file to use as template
  -a GENERATED, --generatedSuiteSuffix GENERATED
                        Suffix for the generated test suites
  -n SUITESNUMBER, --suitesNumber SUITESNUMBER
                        Number of suites to create
  -o OUTPUT, --output OUTPUT
                        Output file
```

# Dependencies
`pip install lxml`

`pip install pyCLI`

# Examples

# Usage
```ts-optimizer -j output.xml -t phpunit.xml.dist -n 4 -o phpunit_generated_4.xml```

# Limitations


