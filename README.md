# postgrest-heroku-dockerfile

Code is forked from https://github.com/PostgREST/postgrest-heroku

Adds a Dockerfile and a Docker compose file to use PostgREST on Heroku Docker builds directly (without buildpack thus)

Config variables (on Heroku config vars or in your local environnement) should be prexifed by PGRST_DB_

List of fetched variables from environnement to the config file are located in env.list

As on Heroku, the most important is to set the environnement variable $PORT so that listenning port is being transmitted to PostgREST configuration, default to default port 3000 otherwise during build
