#Usefull commands by miczi
##Rails:
1. **Revert your DB to some state from the past**

	rake db:migrate:status
	rake db:migrate VERSION=<migration_id_here>
	
2. **RVM clean unnecessary gemsets(can take a lot of disk space, but provides separation in the environment)**

	rvm gemset list
	rvm gemset delete <gemset_name_here>
	
##Bash:
1. **Search recursively for a phrase in each file at given path**
	
	grep -r "<phrase_here>" .