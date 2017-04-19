# Ron Blind App

## Project Description

Ron's blind control server

## Commands

### Install Node, NPM, PM2-Meteor

 * Install Node on Windows, however you do that, this should also install NPM

 * `npm install -g pm2-meteor` install pm2-meteor

### Deploy

  * `meteor create .` -- Create meteor project (this may fail since I check in the .meteor folder into GIT)

  * `meteor add percolate:synced-cron iron:router http` -- Add a few dependencies

  * `meteor npm install` -- Install project NPM dependencies.

  * `cd deploy` -- Move into deploy directory

  * `pm2-meteor deploy` -- Deploy project not using mupx which blows

  * `pm2-meteor start` -- Starts the server

  When you're on the server you can run `pm2 monit` to monitor your app

  More info can be found [here](https://github.com/andruschka/pm2-meteor)