FROM ubuntu:14.04

RUN \
	apt-get update && \
	apt-get install software-properties-common python-software-properties -y && \
	sudo add-apt-repository ppa:webupd8team/java -y && \
	sudo apt-get update -y && \
	echo debconf shared/accepted-oracle-license-v1-1 select true | sudo debconf-set-selections && \
	echo debconf shared/accepted-oracle-license-v1-1 seen true | sudo debconf-set-selections && \
	sudo apt-get install oracle-java8-installer -y
