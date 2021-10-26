---
title: Code Graveyard
layout: page
#callouts: home_callouts
show_sidebar: false

---

This page contains code snippets that I keep coming back to. (Inspired by [Andy Barry's version.](https://abarry.org/likelytobeforgotten/))

## [Mass-renaming with find and sed](https://unix.stackexchange.com/questions/113746/test-recursive-sed-search-and-replace-before-running)
Dry run:
`find . -iname "*.py" -exec sed -n 's/WorldBBoxRule/WorldFrameBBoxRule/gp' {} \;`

Actually do it:
`find . -iname "*.py" -exec sed -i 's/WorldBBoxRule/WorldFrameBBoxRule/g' {} \;`

## [Watch the most recent log file](https://unix.stackexchange.com/questions/83962/tail-f-the-most-recent-log-file)
```
tail -f `/bin/ls -1td /path/to/logfile/**| /usr/bin/head -n1`
```
