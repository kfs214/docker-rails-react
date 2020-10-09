# summary
An environment to build a new app with react and rails on docker

# get ready to use
docker-compose build
docker-compose run --rm front yarn install
docker-compose run --rm api rails db:create
docker-compose up

# if you're in a trouble in creating a db
docker-compose up -d
docker-compose run --rm api rails db:create
docker-compose down
