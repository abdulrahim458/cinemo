#
# MongoDB Dockerfile
#

# Pull base image.
FROM ubuntu

# Install MongoDB.
RUN \
  apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10 && \
  echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' > /etc/apt/sources.list.d/mongodb.list && \
  apt-get update && \
  apt-get install -y mongodb-org && \
  rm -rf /var/lib/apt/lists/*

# Mountable directories.
VOLUME ["/data/db"]

# Working directory.
WORKDIR /data

# Default command.
CMD ["mongod"]

# Expose ports.
EXPOSE 27017
