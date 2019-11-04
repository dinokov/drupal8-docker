drupal8-docker-app
===================

# What is this?

This repo contains a Docker recipe for making a container
running Drupal8, using Linux, Apache, MySQL, Memcache and SSH. 
You can also use it on the Drupal Contribution Sprints for quickly starting
working on your Drupal8 project. 

# Quick 3 step instructions for a Drupal 8 Trial Run:

## 1 - Install docker:

https://docs.docker.com/installation/

## 2 - Get the image and run it using port 80:

Open a terminal and run

```
docker run -i -t -p 80:80 ricardoamaro/drupal8
```

That's it!

## 3 - Visit Drupal 8 in your browser

[http://localhost:8400/](http://localhost:8400/)

Credentials (user/pass): admin/admin

## Extra - Visualize MySQL tables in your browser

[http://localhost:8400/adminer.php](http://localhost:8400/adminer.php)


### Credentials (will be shown in the output)

### Example usage for testing:
Using docker exec {ID} {COMMAND}, to run your own commands.
```
~$ docker run --name mydrupal8 -i -t -p 80:80 ricardoamaro/drupal8

~$ docker exec mydrupal8  uptime
 10:02:59 up 16:41,  0 users,  load average: 1.17, 0.92, 0.76

~$ docker exec mydrupal8 drush status | head
 Drupal version         :  8.5.3
 Site URI               :  http://default
 Database driver        :  mysql
 Database hostname      :  localhost
 Database port          :  3306
 Drupal bootstrap       :  Successful
 ```

## For older Drupal versions check:
https://github.com/ricardoamaro/drupal7-docker-app
https://github.com/ricardoamaro/drupal6-docker-app

## You can also clone this repo somewhere and build it,
```
git clone https://github.com/ricardoamaro/drupal8-docker-app.git
cd drupal8-docker-app
sudo docker build -t <yourname>/drupal8 .
```
