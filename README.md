# Artifacts-repository
A Dockerfile for Sonatype Nexus Repository 3, starting with 3.18 the image is based on the Red Hat Universal Base Image while earlier versions used CentOS.


Running
To run, binding the exposed port 8081 to the host, use:

$ docker run -d -p 8081:8081 --name nexus sonatype/nexus3
When stopping, be sure to allow sufficient time for the databases to fully shut down.

docker stop --time=120 <CONTAINER_NAME>
To test:

$ curl http://localhost:8081/
