# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

docker build --platform linux/amd64 -t flightloggernico/myrailsapp:latest .
docker push flightloggernico/myrailsapp:latest


docker run -p 3000:80 -e RAILS_MASTER_KEY=$(cat config/master.key) flightloggernico/myrailsapp:latest