# WordPress development with VSCode and containers/codespaces 


Base scaffolding for WordPress development with VSCode in containers/codespaces. You just need to clone this respository and update a few parameters to begin to develop your plugin/theme or even your full WordPress website.


## Containers and structure

The structure of the containers used to work is:

 - **wordpress**: Based on official image, it contains WPCli, Xdebug, composer, node, nvm... and other usefull tools as git, wget, phpcs and phpcbf.
 - **database**: MariaDB 10.4
 - **phpmyadmin**: PHPMyAdmin latest official image

You can updata almost everything on .devcontainer/docker-compose.yml file. It's usefull to update .devcontainer/Dockerfile to change version of WordPress installed to try other PHP versions.

After mounting all the images, .devcontainer/setup.sh starts to execute and it automatically installs some extras.

## Visual Studio Code configuration

You don't need to do or update anyting. It just may work with next functions installed and configured:

 - PHP Debug by Xdebug (Extension and .launch configuration)

## How to use

- Clone this repo.
- Modify `.devcontainer/.env` with plugin or theme path and the other WordPress params as needed.
- From githtub repo, create codespace
