FROM dockerbase/tomcat8
ADD run-tomcat.sh /run-tomcat.sh
RUN chmod -v +x /run-tomcat.sh
ENTRYPOINT ["/run-tomcat.sh"]
