# bash-seed
A simple seed for generating a bash project with testing support

### Pre requisites
```
brew install watchman     ## a file watching service
brew install shellcheck   ## linter for bash (finds bugs in your shell scripts)
brew install bats-core    ## testing framework
```

### Guidelines
Put the fast tests in directory ```test```

Put the slow tests in directory ```integration_test```

### Useful Scripts...

#### ... during development

```
./watch
```
Watches for changes in ```src``` and ```test``` and then runs the linter (shellcheck) in both directories. After that runs only the fast tests.

#### ... to run all tests
                                                                                  
 ```
./run_all_tests
```
Checks everything by running the linter, the fast tests and the integration tests.
                                                                                  
#### ... to run only the fast tests
                                                                                  
 ```
./run_fast_tests
```   

#### ... to run only the integration tests
                                                                                  
 ```
./run_integration_tests
```


### Links
https://facebook.github.io/watchman

https://www.shellcheck.net

https://github.com/bats-core/bats-core
                                                                               