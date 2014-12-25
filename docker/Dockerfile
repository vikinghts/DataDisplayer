from ubuntu:14.04
MAINTAINER kjansen
run echo "create DataDisplayer container"
run ping -c 1 www.google.com
run echo "Network is oke"
run sudo apt-get update
run apt-get -y install openjdk-7-jdk
run echo 'export JAVA_HOME=/usr/lib/jvm/jre-1.7.0-openjdk.x86_64' > /etc/profile.d/java.sh
run apt-get -y install openssh-server
run apt-get -y install tomcat7
run service ssh start

ENV CATALINA_HOME /usr/share/tomcat7
# Launch Tomcat on startup
CMD ${CATALINA_HOME/bin/catalina.sh run


#add DataDisplayer-0.1-shadow.jar /tmp/DataDisplayer-0.1-shadow.jar

#CMD ["java", "-jar", "/tmp/DataDisplayer-0.1-shadow.jar"]

EXPOSE [22,8080]