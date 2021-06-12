# FlyntWP Docker Starter

> A starter kit to quickly setup a new Wordpress + FlyntWP project

## Setup

This repository includes multiple docker containers for working locally. **Deployment via Docker is not planned yet but may be considered later**

You can set up this project quickly via `docker-compose` which will spin up the following containers:

- `composer` - includes composer and handles the initial installation of composer files
- `db` - this includes the development database
- `node` - includes node.js and is used to build assets locally while working on the files via a watcher
- `wordpress` - this includes the webserver and wordpress plus handles the initial building of all assets via node 14

To make sure node_module are installed, run `docker-compose exec node yarn install` & `docker-compose ecec composer composer install`.

## After the docker setup

After setting up the project, the website should be available at `http://localhost`.

Make sure to the start the bundler via `docker-compose exec node yarn start`.

## ACF Pro

FlyntWP requires you to use ACF Pro. Make sure to download your ACF Pro plugin and put it into the `wp-content/plugins` folder.
