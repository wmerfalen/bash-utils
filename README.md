# Bash utils
A collection of scripts written in bash using *mostly* common binaries in modern bash environments

## random-string
```sh
# Usage: ./random-string <LENGTH>

# Example:
./random-string 32

# The utility echoes out the string and uses the `-n` option to the echo command.
# this means that in order to capture the output, you either call it within a sub-shell
# or redirect to your choice of file
RANDOM_STRING=$(./random-string 32)

# or to a file
./random-string 32 > /tmp/my_file
```


## Test scripts
Any script with a suffix of `-test` will run functions to test if the utility passes
all tests.

```sh
./random-string-test
```

# version
1.0.0  - random-string and random-string-test utility

# Author
William Merfalen https://github.com/wmerfalen
