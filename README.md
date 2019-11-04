drupal8-docker-app
===================

# What is this?

This repo contains a Docker recipe for making a container
running Drupal8, using Linux, Apache, MySQL, Memcache and SSH. 
You can also use it on the Drupal Contribution Sprints for quickly starting
working on your Drupal8 project. 


## 1 - Download and run:
```
git clone https://github.com/dinokov/drupal8-docker.git
sudo chown -vR damir:damir ./drupal-1
cd drupal8-docker
sudo docker-compose up
```

## 3 - Visit Drupal 8 in your browser

[http://localhost:8400/](http://localhost:8400/)

Credentials (user/pass): admin/admin

## Extra - Visualize MySQL tables in your browser

[http://localhost:8400/adminer.php](http://localhost:8400/adminer.php)

### Credentials (will be shown in the output)

## For older Drupal versions check:
https://github.com/ricardoamaro/drupal7-docker-app
https://github.com/ricardoamaro/drupal6-docker-app

