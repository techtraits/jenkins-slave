# jenkins-slaves
Jenkin swarm slaves with docker installed and accessible to docker slave. 


## Running

To run a Docker container customizing the different tools with your credentials

    docker run \
    -e JENKINS_USERNAME=jenkins \
    -e JENKINS_PASSWORD=jenkins \
    -e JENKINS_MASTER=http://jenkins:8080 \
    techtraits/jenkins-slave

### Optional Environment Variables

You can specify optional environment variables below when invoking docker run to customize the behavior of the swarm client.

| Parameter       | Default Value       | Description                                                                |
|-----------------|---------------------|----------------------------------------------------------------------------|
| SLAVE_EXECUTORS | number of cpu cores | This value specifies the number of concurrent jobs this worker can process |
