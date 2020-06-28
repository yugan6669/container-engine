FROM dockerbase/tomcat8
ADD run-tomcat.sh /entrypoint.sh
RUN chmod -v +x /run-tomcat.sh
ENTRYPOINT ["/run-tomcat.sh"]
