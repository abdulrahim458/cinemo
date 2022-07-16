#
# MongoDB Dockerfile
#

# Pull base image.
FROM ubuntu

# Install MongoDB.
RUN \
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
