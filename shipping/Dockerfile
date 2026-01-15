FROM maven:3.9.11
WORKDIR /app
COPY pom.xml .
COPY src ./src
EXPOSE 8080
RUN mvn clean package 
RUN mv target/shipping-1.0.jar shipping.jar
ENV CART_ENDPOINT = "cart:8080"\
    DB_HOST = "mysql"
CMD ["java", "-jar" , "/app/shipping.jar"]

