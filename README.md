# mysql.server-264-kill-No-such-process.-Xampp-ubuntu-16.04
Solution for mysql.server: 264: kill: No such process. Xampp/ubuntu 16.04 error




------Check if the port used by mysql is occupied by a service already

sudo lsof -i :3306


------It will give u the PID

sudo kill -9 <PID>


------and then start the mysql server 

sudo /opt/lampp/lampp startmysql
