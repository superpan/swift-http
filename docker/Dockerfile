FROM ubuntu:latest
EXPOSE 8080
RUN echo "Installing dependencies..."
RUN apt-get update && apt-get install -y --force-yes wget build-essential clang rsync libpython-all-dev libedit-dev libicu52
RUN cd /
RUN wget https://swift.org/builds/ubuntu1404/swift-2.2-SNAPSHOT-2015-12-01-b/swift-2.2-SNAPSHOT-2015-12-01-b-ubuntu14.04.tar.gz
RUN tar xzf swift-2.2-SNAPSHOT-2015-12-01-b-ubuntu14.04.tar.gz
RUN rsync -a -v swift-2.2-SNAPSHOT-2015-12-01-b-ubuntu14.04/usr/ /usr
RUN rm -rf swift-2.2-SNAPSHOT-2015-12-01-b-ubuntu14.04*
