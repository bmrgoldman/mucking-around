# Docker
Docker is cool. Why do I have so much trouble getting it to work? Here are some shortcuts I've learned whilst trying to stand up webrecorder using docker:

What's running? What ports are being used? What are the container ids?

    docker ps -a

What's the IP address of all these apps?

    docker inspect -f '{{.Name}} - {{.NetworkSettings.IPAddress }}' $(docker ps -aq)
