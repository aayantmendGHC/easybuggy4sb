FROM tomcat:8.5.84-jdk8-corretto-al2
COPY server.xml /usr/local/tomcat/conf/
COPY index.jsp /usr/local/tomcat/webapps/attacker_app/
COPY brute_force_attack.sh /usr/local/tomcat/
COPY css/ /usr/local/tomcat/webapps/attacker_app/css/
COPY fonts/ /usr/local/tomcat/webapps/attacker_app/fonts/
COPY img/ /usr/local/tomcat/webapps/attacker_app/img/
COPY picture/ /usr/local/tomcat/webapps/attacker_app/picture/
RUN chmod +x /usr/local/tomcat/brute_force_attack.sh
CMD ["catalina.sh", "run"]
