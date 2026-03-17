FROM eclipse-temurin:17-jdk

WORKDIR /app

##Instalar un verificador, utilizar los heathChecks en una peticion HTTP
RUN atp-get update && apt-get install y curl && rm -rf /var/lib/apt/lists/*

COPY target/*.jar app.jar
EXPOSE 8082

ENTRYPOINT ["java","-jar","app.jar"]