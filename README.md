# Linux-commands
All handy Linux commands

## Find
Syntax: $ find /path/to/search -options criteria
```
find ./GFG -name sample.txt
```
> Find a file by the name (case sensitive) sample.txt inside folder GFG

```
find ./GFG -iname '*sample*txt'
```
> Find a file by the name (case insensitive) containing the word 'sample' and 'txt' inside folder GFG

```
find 2022 -type f -iname '*belly*'
```
> Find a file by the name (case insensitive) containing the word 'belly' inside folder 2022. Use *-type d* for directory

## Grep
```
grep 'Sally' phbook.txt > answer.txt
```
> Look for all lines containing text 'Sally' in file phbook.txt and output the result to answer.txt 
