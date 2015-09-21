FROM nate9/minimaljava8
RUN apk --update add curl tar
ENV JMETER_VERSION 2.13
# Install JMeter
RUN cd /var/lib && \
  curl http://mirror.ox.ac.uk/sites/rsync.apache.org//jmeter/binaries/apache-jmeter-$JMETER_VERSION.tgz -o /var/lib/jmeter-$JMETER_VERSION.tgz && \
  tar xf jmeter-$JMETER_VERSION.tgz && \
  rm -f jmeter-$JMETER_VERSION.tgz

CMD ["user/bin/java", "-version"]