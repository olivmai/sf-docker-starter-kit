# Docker starter kit to run Symfony application
Simple stack for local dev purpose. Optimized for docker-sync.

## How it works

### Create Symfony application

Create your Symfony app using Symfony cli
```bash
symfony new project_name --full
```
Then move to your new fresh app
```bash
cd project_name
```

### Copy docker files

Copy the ```.docker``` directory and the ```docker-compose.yml``` and ```docker-sync.yml``` files to your root app directory.

## Few changes to fit your need

In ```docker-sync.yml```, change your project location :
```yml
syncs:
  sf-sync:
    #...
    src: '/Path/to/your/project/root'
```


