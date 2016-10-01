FROM java:8
VOLUME /tmp

ADD . /usr/app
ENV spring.cloud.config.server.git.uri @spring.cloud.config.server.git.uri@
ENV eureka.client.serviceUrl.defaultZone @eureka.client.serviceUrl.defaultZone@

EXPOSE 8888

ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/usr/app/@project.build.finalName@.jar"]
