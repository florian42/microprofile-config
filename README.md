# Build
mvn clean package && docker build -t com.example/config-example .

# RUN

docker rm -f config-example || true && docker run -d -p 8080:8080 --name config-example com.example/config-example