# Sử dụng Tomcat 9 và Java 11 (hoặc version phù hợp với code của bạn)
FROM tomcat:9.0-jdk11-openjdk

# Xóa các ứng dụng mặc định của Tomcat để nhẹ máy
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy file WAR của bạn vào thư mục chạy web của Tomcat
COPY ROOT.war /usr/local/tomcat/webapps/ROOT.war

# Mở cổng 8080 (Cổng mặc định của Tomcat)
EXPOSE 8080

# Chạy Tomcat
CMD ["catalina.sh", "run"]