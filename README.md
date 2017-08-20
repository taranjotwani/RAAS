# RAAS
Redis as a service

* Use the docker file to create the images.
* Use the following commands to setup redis on the server.
```sh
wget http://download.redis.io/redis-stable.tar.gz
tar xvzf redis-stable.tar.gz
cd redis-stable
make
```
* Copy the redis-server and redis-sentinel to /usr/local/bin/
* Create the below folder for setting the confid and dump files
  * /etc/redis
* Copy the redis-server.conf and redis-sentinel.conf to the /etc/redis folder.
* Use the following services to start the redis-server and redis-sentinel
```sh
service redis-server start
service redis-sentinel start
```

Please post if you find any issues
