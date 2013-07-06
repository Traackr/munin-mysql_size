MySQL Size Munin Plugin
=======================

A Munin plugin to report on MySQL database size (data and index). Inspired by ```http://tripleonard.github.io/blog/2012/02/04/a-simple-munin-plugin-to-track-the-size-of-a-mysql-database/```

Install
-------

To install:

	sudo cp mysql_size /usr/local/share/munin/plugins/
	sudo chmod +x /usr/local/share/munin/plugins/mysql_size
	sudo ln -s /usr/local/share/munin/plugins/mysql_size /etc/munin/plugins/mysql_size



Configuration
-------------

Edit /etc/munin/plugin-conf.d/munin-node

	[mysql_size]
		env.username <database-user>
		env.password <database-password>
		env.database <database-name>
