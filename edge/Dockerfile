FROM java:8

WORKDIR /

RUN apt-get update && apt-get install -y git wget libgradle-core-java

RUN git clone https://github.com/Netflix/recipes-rss.git

WORKDIR /recipes-rss

ADD convention.gradle ./gradle
ADD check.gradle ./gradle
ADD edge.properties ./rss-edge/src/main/resources

RUN ./gradlew clean build

ENV APP_ENV=dev

CMD ["java","-jar","/recipes-rss/rss-edge/build/libs/rss-edge-0.1.0-SNAPSHOT.jar"]
