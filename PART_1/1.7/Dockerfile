# Start from the Ubuntu image.
FROM ubuntu:22.04

# Update package lists and install curl
RUN apt-get update && apt-get install -y curl

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the script.sh file from this directory to /usr/src/app/ creating /usr/src/app/script.sh
COPY script.sh .

# Add execution permisson to script
RUN chmod u+x script.sh

# When running docker run the command will be ./script.sh
CMD ./script.sh