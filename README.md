# Usefull commands by miczi
## Rails:
1. **Revert your DB to some state from the past**

```
	rake db:migrate:status
	rake db:migrate VERSION=<migration_id_here>
```

2. **RVM clean unnecessary gemsets(can take a lot of disk space, but provides separation in the environment)**

```
	rvm gemset list
	rvm gemset delete <gemset_name_here>
```
	
## Bash:
1. **Search recursively for a phrase in each file at given path**

```
	grep -r "<phrase_here>" .
```
2. **Open all pdfs which contains given phrase
```
# first install pdfgrep (available in package manager, for sure: apt)
# secondly install evince (also in pm) - it's a pdf viewer appliaction
# Explanation: 
# 1. look for all occurences in given folder
# 2. split the output into columns, where whe treat : as a separator
# 3. take 1st column and redirect the output(pdf names) to evince, which is pdf program
pdfgrep <regex/phrase in double quotes> * | cut -d: -f1 | evince 
```
