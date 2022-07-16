#
# MongoDB Dockerfile
#

# Pull base image.
FROM mongo


# Mountable directories.
VOLUME ["/data/db"]

# Working directory.
WORKDIR /data

# Default command.
CMD ["mongod"]

# Expose ports.
EXPOSE 27017
