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
> Find a file by the name (case insensitive) containing the word 'belly' inside folder 2022. Use ***-type d*** for directory

## Grep
```
grep 'Sally' phbook.txt > answer.txt
```
> Look for all lines containing text 'Sally' in file phbook.txt and output the result to answer.txt
```
grep -n --color=auto 'the' poem.txt
```
> Look for 'the' in poem.txt with coloured text (--color=auto) and printed line number (-n).

## wc
```
wc 'Sally'
```
> word count. Results in a b c, that is #lines #words #characters respectively.

## cat
> Concatenate ==> to view a file

## head
```
head -n3 abc.log
```
> to view the first 3 lines in abc.log. -nx ==> to specify how many of first lines.

## tail
<> head
```
tail -n4 abc.log
```
> To show last 4 lines of abc.log.

## awk
Extract a specific text from a file

## sed
= stream editor. To modify text in command pipeline.
```
sed s/Orange/Red/ simpletext.txt
```
> Substitutes 'Orange' with 'Red' from simpletext.txt.

## sort
Sort data/file.
```
sort simple.txt
```  
> sort simple.txt  
Example:  
Name  Id  Team  
Barry 3   Blue  
Gwen  12  Orange  
Rob   8   Red  

will become:  

Barry 3   Blu  
Gwen  12  Orange  
Name  Id  Team  
Rob   8   Red  
```
sort -k2 -n simple.txt
```
> sort column 2 (-k2) for numerical sorting (-n). Default k = 1, i.e. first column.  
Example:
Name  Id  Team  
Barry 3   Blue  
Gwen  12  Orange  
Rob   8   Red  

will become (with 2nd column sorted - number goes first):  

Barry 3   Blue  
Rob   8   Red  
Gwen  12  Orange  
Name  Id  Team  

## rev
Print text in reverse order.

## tac
Concatenate/display files in reverse.

## tr
Translate individual characters according to parameters.
