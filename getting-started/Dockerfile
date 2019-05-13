FROM oracle/graalvm-ce:1.0.0-rc16

# use GMT time in application logs
ENV TZ=GMT
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
ENV GRAALVM_HOME=${JAVA_HOME}

# /opt/app is expected to be volume-mapped to application code
WORKDIR /opt/app
