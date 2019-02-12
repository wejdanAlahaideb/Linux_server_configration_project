# Linux_server_configration_project
1.	The Server IP address: 206.189.143.92
2.	SSH port: 26
3.	The complete URL hosted web application: http://206.189.143.92/ 
4.	A summary of software installed:-
	a)	Installed using apt-get
		•	finger/bionic,now 0.17-15.1 amd64 
		•	python-flask/bionic,now 0.12.2-3 all 
		•	python-flask-sqlalchemy/bionic,now 2.1-3build1 all 
		•	libapache2-mod-wsgi-py3/bionic,now 4.5.17-1 amd64  
		•	postgresql/bionic,now 10+190 all 
		•	postgresql-contrib/bionic,now 10+190 all 
	b)	Installed using pip
		•	Flask (0.12.2)
		•	Flask-SQLAlchemy (2.1)
		•	psycopg2 (2.7.7)
		•	psycopg2-binary (2.7.7)
		•	SQLAlchemy (1.1.11)

5.	A summary of configuration changes made:-
	a)	On firewall: Allow SSH, HTTP, and NTP
	b)	On /etc/ssh/sshd_config
		•	Disable root remote ssh: replace PermitRootLogin yes to PermitRootLogin no 
		•	Change ssh default port: replace  #Port 22 with Port 26
		•	Force authenticate using RSA keys

