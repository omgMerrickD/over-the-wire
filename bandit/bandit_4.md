# My solution
```
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ file ./-file00
./-file00: data
bandit4@bandit:~/inhere$ file ./*.*
./*.*: cannot open `./*.*' (No such file or directory)
bandit4@bandit:~/inhere$ file ./*
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: data
bandit4@bandit:~/inhere$ cat ./-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
bandit4@bandit:~/inhere$
```

## Comments
The hint here is that the password is stored in the only human-readable file in the directory.  You could ```cat filename``` everything one at a time, but that would be silly. The site lists ```file``` as of the useful commands and a quick ```man file``` gets me the info I need.