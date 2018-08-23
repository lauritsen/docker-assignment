# Dockerfile for The gay border TOIlet application

# Add a base image to build this image of
FROM ubuntu:18.04

# Install curl
RUN apt-get update && apt-get install -y curl

# Download image and extract files
RUN curl -o toilet-0.3.tar.gz http://caca.zoy.org/raw-attachment/wiki/toilet/toilet-0.3.tar.gz
RUN tar xzf toilet-0.3.tar.gz

# Install toilet
RUN apt-get install -y toilet

# Run command
CMD ["toilet", "-F", "border", "--gay"]

