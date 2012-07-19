This file gives you an overview of your instance directories.

/private	is where you can store private files
/snapshot	is where snapshots of your disk will be available

/lamp0		is your main folder seen as /srv/data from your code
    /tmp	is where temporary file are stored
	/mysql  is where your mysql database is stored
	/var
		/admin		is a Gandi-restricted internal directory
		/log		is where process log file are available (work in progress)
		/php		is the working directory for php (sessions...)
		/mysql		is the working directory for mysql
	/web
		/vhosts		is where vhost directories will be available once configured from your Gandi.net Simple Hosting admin page
			/yourvhost.tld		is where you put private directory for related vhost
			/yourvhost.tld/htdocs/	is where you put your public code for related vhost
		/trash    	is where vhost directories will be move once unconfigured from Gandi.net Simple Hosting admin page
		/includes 	is the default includes_path where you can put your shared PHP librairies

/vhosts		is a symlink to /lamp0/web/vhosts
