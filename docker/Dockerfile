FROM ubuntu:latest
ENV DEBIAN_FRONTEND=noninteractive
ENV TZ=America/Los_Angeles
RUN apt-get update -y && apt-get upgrade -y
# install tex packages
RUN apt-get install -y texlive-full texlive-extra-utils pandoc
# java needed for arara
RUN apt-get install -y default-jre
WORKDIR /mnt
CMD ["arara"]
