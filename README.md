cd eureka-server
./mvnw clean package -DskipTests
cd .. 
cd ms-productos
./mvnw clean package -DskipTests
cd ..
cd ms-pedidos
./mvnw clean package -DskipTests

docker compose app --build
