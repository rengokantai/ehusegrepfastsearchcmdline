# ehusegrepfastsearchcmdline
###4 Search matching files by combining find and grep with xargs
output without new line
```
find text -name "a.js" |xargs
```
is same as
```
find text -name "a.js" |xargs echo
```

####01:45
```
find examples -name "*a.js" | xargs grep "text "
grep -r --include="*a.js" "should " examples
```


###5 Search the contents of a git repository with git grep
```
git grep bind
git -r --color bind .
```

###6 Show context around matches using grep
show line numbers
```
grep -n "#" *.md
```

###7 Search for basic patterns using grep
char:
- . one char
- * 0 or more char

```
grep "http\?" readme.md
grep "http\+" readme.md
grep -E "http?" readme.md
grep -E "http+" readme.md
```


###9 Search for optional patterns with grep OR
```
grep "a\|b"
grep -E "a|b"
```
