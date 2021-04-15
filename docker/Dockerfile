FROM confluentinc/cp-kafka-connect:6.1.1

RUN confluent-hub install --no-prompt confluentinc/kafka-connect-jdbc:10.1.0

RUN curl -H "Accept: application/zip" https://repo1.maven.org/maven2/com/oracle/database/jdbc/ojdbc6/11.2.0.4/ojdbc6-11.2.0.4.jar -o ojdbc6.jar
RUN curl -H "Accept: application/zip" https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.23/mysql-connector-java-8.0.23.jar -o mysql.jar
RUN cp ojdbc6.jar /usr/share/confluent-hub-components/confluentinc-kafka-connect-jdbc/lib
RUN cp mysql.jar /usr/share/confluent-hub-components/confluentinc-kafka-connect-jdbc/lib

