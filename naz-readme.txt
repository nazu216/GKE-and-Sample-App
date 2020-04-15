In the MySQL service, I’ve not specified any type, in that case, type ‘ClusterIP’ will get used, 
which will make sure that MySQL container is exposed to the cluster and the Python app can access it.




If you check the app.py, you can see that I have used “mysql-service.default” as a hostname. 
“Mysql-service.default” is a DNS name of the service. The Python application will refer to that DNS name while accessing the MySQL Database
