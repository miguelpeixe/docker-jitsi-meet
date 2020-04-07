ARG JITSI_REPO=jitsi
FROM ${JITSI_REPO}/base-java

RUN	\
	apt-dpkg-wrap apt-get update && \
	apt-dpkg-wrap apt-get install -y git maven openjdk-8-jdk libxml2-utils && \
	apt-cleanup

