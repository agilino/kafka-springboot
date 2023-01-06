# Running Kafka on the cloud

Usually you run kafka behind a gateway and not let access it from outside.

For testing you can run kafka on a cloud server and allow all clients to access using a proxy. This is usually a very bad idea on production, because anyone can access your server, but you can run this configuration for practice.

In this directory you find a docker-compose.yml with nginx reverse proxy to pass the kafka stream to the client.

DO NOT run with that setting on production, unless you want everybody to access your kafka server and possibly the content of your kafka topics.
