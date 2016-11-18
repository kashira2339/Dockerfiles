FROM openjdk:8

ENV VERSION_ACTIVATOR=1.3.2
RUN curl -O http://downloads.typesafe.com/typesafe-activator/${VERSION_ACTIVATOR}/typesafe-activator-${VERSION_ACTIVATOR}.zip
RUN unzip typesafe-activator-${VERSION_ACTIVATOR}.zip
RUN install -m 755 activator-${VERSION_ACTIVATOR}/activator /usr/local/bin/activator
RUN install -m 644 activator-${VERSION_ACTIVATOR}/activator-launch-${VERSION_ACTIVATOR}.jar /usr/local/bin/activator-launch-${VERSION_ACTIVATOR}.jar
RUN cp -r activator-${VERSION_ACTIVATOR}/repository /usr/local/bin/
RUN cp -r activator-${VERSION_ACTIVATOR}/templates /usr/local/bin/
RUN rm typesafe-activator-${VERSION_ACTIVATOR}.zip
RUN rm -r activator-${VERSION_ACTIVATOR}