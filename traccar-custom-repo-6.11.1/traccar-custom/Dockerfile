FROM eclipse-temurin:17-jdk-alpine

WORKDIR /opt/traccar

# Pobierz najnowszy Traccar (ZIP)
ADD https://github.com/traccar/traccar/releases/download/v6.11.1/traccar-other-6.11.1.zip /tmp/traccar.zip
RUN apk add --no-cache unzip && \
    unzip -o /tmp/traccar.zip -d /opt/traccar && \
    rm /tmp/traccar.zip

EXPOSE 8082
CMD ["./bin/start"]
