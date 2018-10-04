SPIRE build on a Centos 7 base images.

To build:

`docker build -t spire .`

To run:

`docker run spire -p 8080 -p 8081`

To override the default SPIRE server configuration, either modify conf/server.conf before building, or run spire to point to a local configuration file at runtime:

`docker run spire -v local_drive/server.conf:/opt/spire/conf/server.conf -p 8080 -p 8081`
