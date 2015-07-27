# jenkins-slaves
Jenkin swarm slaves with docker installed and accessible to docker slave. 


## Running

To run a Docker container customizing the different tools with your credentials

    docker run \
    -e JENKINS_USERNAME=jenkins \
    -e JENKINS_PASSWORD=jenkins \
    -e JENKINS_MASTER=http://jenkins:8080 \
    techtraits/jenkins-slave
